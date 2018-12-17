# Spring
## IoC 容器 Inversion of Controller (反转控制)
其思想就是反转资源控制的方向。我们一般的编程当中都是由组件自身去获取自己想要的对象（方式一），反转控制指的就是由 IoC 容器来管理所有的对象（组件）的生成，并将组件依赖的资源推送给组件（方式二）。
1. 方式一，组件自身获取依赖的时候，知道自己获取的是什么对象；
2. 方式二，容器向组件推送资源的时候，组件并不知道容器会把什么对象推送给它。

**例子** IoC 容器的一个小例子
```
Travel travel = new Travel();
travel.setTranport(new Airplane());
travel.doTravel();
```

## DI Dependency Injection 依赖注入
DI 是 IoC 实现的一种方式，也是 IoC 的别称
依赖注入的方式有很多：
1. setter 方法
2. contruct
3. 反射

依赖的配置方式：
1. xml 传统的配置方式，也是程序员最痛恨的一种方式
2. annotation 流行的方式

**练习** 是用 Spring 实现我们上面的小例子

## Maven
```
ant -> ivy -> maven -> gradle
```
一个项目管理工具和自动构建工具
1. 简化项目构建（编译）过程，（我们往往只需要一个命令就可以完成项目的构建，而在Eclipse中需要点击很多的选项才能完成构建到处war）
2. 提供一个统一的构建系统
3. 提供完善的项目信息，包括项目依赖等等

### 配置文件 pom.xml
```
mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false
```
## spring boot

<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzNTA0OTYyNzUsMTI1MjA5MjY3Nl19
-->