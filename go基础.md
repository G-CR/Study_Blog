## 变量和常量

### 变量声明

**标准声明**

变量声明以关键字var开头，变量类型放在变量的后面，行尾不需要分号

```go
var name string
var age int
var isOk bool
```

**批量声明**

```go
var (
		a string
)
```



### 变量初始化

```go
var name string = "xiaoming"
var sex int = 1
```

或者一次初始化多个变量

```go
var name, sex = "xiaoming", 1
```



**类型推导**

有时候可以将后面的类型省略，通过对等号右边的值推导变量的类型

```go
var name = "xiaoming"
var sex = 1
```



**短变量声明**

在函数内部，可以使用 `:=` 的方式初始化变量

```go
func main() {
		n := 1
		m := 10
}
```



**匿名变量**

_ 变量不占用命名空间，不分配内存，不存在重复声明，当需要接收不使用的值时，可以用 _表示忽略值

```go
func fun()(int, string) {
	return 1, "xiaoming"
}

func main() {
	x, _ := fun()
	_, y := fun()
	
	fmt.Println(x, y)
}
```



### 常量

```go
const pi = 3.1415
e = 2.7182
```



放在一起声明

```go
const (
		pi = 3.1415
		e = 2.7182
)
```

同时声明多个常量时，如果忽略了值则表示和上面一行的值相同

```
const (
		a = 1
		b
		c
)
```

a、b、c 的值都是 100



### **iota**

`iota`是`go`语言的常量计数器，只能在常量的表达式中使用。`iota`在 `const` 关键字出现时被重置为0。 `const`中每一行常量将使用`iota`计数一次 (`iota`可理解为`const`语句块中的行索引)，使用 `iota`能简化定义。

```go
const (
		a = iota // 0
		b        // 1
		c        // 2
		d        // 3
		e        // 4
)
```



#### **常见的iota示例**

**使用_跳过某些值**

```go
const (
		a = iota // 0
		b        // 1
		_
		c        // 3
)
```

**`iota` 声明中间插队**

```go
const (
		a = iota // 0
  	b = 100  // 100
  	c = iota // 2
  	d        // 3
)
const e = iota // 0
```



**定义数量级**

```go
const (
		_ = iota
  KB = 1 << (10 * iota)
  MB = 1 << (10 * iota)
  GB = 1 << (10 * iota)
  TB = 1 << (10 * iota)
  PB = 1 << (10 * iota)
)
```



**多个 `iota` 定义在一行**

```go
const (
		a, b = iota + 1, iota + 2 // 1, 2
		c, d                      // 2, 3
		e, f                      // 3, 4
)
```



## 数据类型

**多行字符串**

```go
s1 := `123
456
789
`
```

**字符串常用操作**

|                方法                 |      介绍      |
| :---------------------------------: | :------------: |
|              len(str)               |     求长度     |
|           +或fmt.Sprintf            |   拼接字符串   |
|            string.Split             |      分割      |
|          strings.Contains           |  判断是否包含  |
| string.HasPrefix, strings.HasSuffix | 前缀/后缀判断  |
| strings.Index(),strings.LastIndex() | 子串出现的位置 |
| strings.Join(a[]string, sep string) |    join操作    |

```go
package main
import (
	"fmt"
	"strings"
)

func main() {
	s := "123456789"
    fmt.Println(s)
    
    fmt.Println(s+s)
    
	a := strings.Split(s, "4")
	fmt.Println(a)
    
    fmt.Println(strings.Contains(s, "456"))
    fmt.Println(strings.Contains(s, "457"))
    
    
    fmt.Println(strings.HasPrefix(s, "12345"))
    fmt.Println(strings.HasSuffix(s, "789"))
    
    
    fmt.Println(strings.Index(s, "345"))
    
    
    test := make([]string, 0)
    for i:= 0; i < 10; i++ {
        test = append(test, "hello world")
    }
    
    res := strings.Join(test, " ")
    print(res)
}
```



**修改字符串**

对于有中文的字符串 `string` 转换成 `rune` 进行操作，只用 简答字符构成的转换成 `byte` 操作就可以了，之后转换回`string`和转成数组操作都是需要额外的时间和空间开销的

```go
package main

import "fmt"

func main() {
	s := "hello"
	s1 := []byte(s)
	s1[0] = 'H'
	fmt.Println(string(s1))
	
	t := "你好"
	t1 := []rune(t)
	t1[0] = '我'
	fmt.Println(string(t1))
}
```



## 数组

### **一维数组**

```go
全局:
var arr0 [5]int  = [5]int{1,2,3}
var arr1 = [5]int{1,2,3,4,5}
var arr2 = [...]int{1,2,3,4,5,6}
var str = [5]string{3: "hello world", 4: "tom"}

局部:
a := [3]int{1,2}
b := [...]int{1,2,3,4}
c := [5]int{2:100, 4:200}
d := [...]struct {
  name string
  age uint8
}{
  {"user1", 10},
  {"user2", 20},
}
```



### 多维数组

```go
全局:
var arr0 [5][3]int
var arr1 [2][3]int = [...][3]int{{1,2,3}, {7,8,9}}
局部:
a := [2][3]int{{1,2,3}, {4,5,6}}
b := [...][2]int{{1,1}, {2,2}, {3,3}}
```



## 切片

```go
全局:
var arr = [...]int{0,1,2,3,4,5,6,7,8,9}
var slice0 []int = arr[start:end]
var slice1 []int = arr[:end]
var slice2 []int = arr[start:]
var slice3 []int = arr[:]
var slice4 = arr[:len(arr)-1] // 去掉切片的最后一个元素

局部:
arr2 = [...]int{9,8,7,6,5,4,3,2,1,0}
slice5 := arr2[start:end]
slice6 := arr2[:end]
slice7 := arr2[start:]
slice8 := arr2[:]
slice9 := arr2[:len(arr)-1]
```



|      操作       |                             含义                             |
| :-------------: | :----------------------------------------------------------: |
|      s[n]       |                    切片s中索引位置为n的项                    |
|      s[:]       |          从切片s的索引位置0到len(s)-1处所得到的切片          |
|     s[low:]     |         从切片s的索引位置low到len(s)-1处所得到的切片         |
|    s[:high]     |           从切片s的索引位置0到high-1处所获得的切片           |
|   s[low:high]   |          从切片s的索引位置low到high-1处多得到的切片          |
| s[low:high:max] | 从切片s的索引位置low到high-1处所获得的切片，len=high-low，cap=max-low |
|     len(s)      |                   切片s的长度，总是≤cap(s)                   |
|     cap(s)      |                   切片s的容量，总是≥len(s)                   |



### 通过make来创建切片

```go
var slice []type = make([]type, len)
slice := make([]type, len)
slice := make([]type, len, cap)
```



