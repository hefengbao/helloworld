# Learning Kotlin: 接口


`interface`

```kotlin
interface DemoInterface {
    //抽象方法的声明
    fun bar()
    
    //声明及实现
    fun foo() {
        //可选的方法体
    }
}
```



接口无法保存状态。它可以有属性但必须声明为抽象或提供访问器实现。



接口中的属性

