# 常量

#### 2.1 枚举常量

使用枚举来关联一组integer常量  

枚举常量和typedef遵循函数的命名规范，下面的例子是 NSMatrix.h

```objectivec
typedef enum _NSMatrixMode {
    NSRadioModeMatrix            = 0,
    NSHighlightModeMatrix       = 1,           
    NSListModeMatrix            = 2,
    NSTrackModeMatrix           = 3
} NSMatrixMode;
```

你可以为bit masks之类的东西创建一个匿名枚举 

```objectivec
enum {
    NSBorderlessWindowMask       = 0,
    NSTitledWindowMask           = 1 << 0,
    NSClosableWindowMask         = 1 << 1,
    NSMiniaturizableWindowMask   = 1 << 2,
    NSResizableWindowMask         = 1 << 3
};
```

**2.2 使用const关键字的常量 **

使用const关键字来创建一个float常量

你可以使用const关键字来创建一个与其他常量不相关的integer常量，否则，使用枚举

使用const关键字的常量也遵循函数的命名规则 

```objectivec
const float NSLightGray;
```



#### 2.3 其他常量类型

- 通常不应使用 #define 预编译指令来创建常量

- - integer常量，使用枚举
  - float常量，使用 const 修饰符

- 对 #define 预编译指令，大写所有字母

- - 比如 DEBUG 判断

- ```objectivec
  #ifdef DEBUG
  ```

- ​


- 注意宏命令的字首和字尾都有双下划线 

```objectivec
__MACH__
```



- 定义NSString常量来作为Notification和Key值

- - 这样做可以有效防止拼写错误

```objectivec
APPKIT_EXTERN NSString *NSPrintCopies;
```





{% include links.html %}
