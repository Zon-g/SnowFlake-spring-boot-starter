## SnowFlake-spring-boot-starter

#### 介绍（Description）

> SnowFlake-spring-boot-starter是笔者编写的一个starter, 主要是为了能够将SnowFlake算法应用在spring boot项目中，并遵循约定大于配置。

> SnowFlake-spring-boot-starter is a starter which can apply SnowFlake algorithm proposed by twitter in sprint boot application, following the rule: Convention Over Configuration.

***

#### 更新（Update）

> SnowFlake-spring-boot-autoconfigure和SnowFlake-spring-boot-starter全部迁移至[github:SnowFlake](https://github.com/Zon-g/SnowFlake)或者[gitee:SnowFlake](https://gitee.com/lemonpy/SnowFlake)。

> SnowFlake-spring-boot-autoconfigure and SnowFlake-spring-boot-starter are migrated to [github:SnowFlake](https://github.com/Zon-g/SnowFlake)或者[gitee:SnowFlake](https://gitee.com/lemonpy/SnowFlake).

***

#### 使用说明（Instructions）

> 1. 在项目的pom.xml文件中导入该starter，例如 
>
>    ```xml
>    <dependency>
>        <groupId>com.github.zong</groupId>
>        <artifactId>SnowFlake-spring-boot-starter</artifactId>
>        <version>1.0.0</version>
>    </dependency>
>    ```
>
> 2. 在项目任何想生成id的地方，首先使用
>
>    ```java
>    @Autowired
>    private Generator generator;
>    ```
>
>    注入一个generator对象，然后调用该对象的`nextId()`方法即可获取一个全局唯一id。

>1. You need to import this starter in pom.xml like
>
>   ```xml
>   <dependency>
>       <groupId>com.github.zong</groupId>
>       <artifactId>SnowFlake-spring-boot-starter</artifactId>
>       <version>1.0.0</version>
>   </dependency>
>   ```
>
>2. At anywhere you wanna generate a global unique id, you should inject an instance of interface Generator using
>
>   ```java
>   @Autowired
>   private Generator generator;
>   ```
>
>   and then invoke the method `nextId()`, the only method of interface Generator, to aquire a global unique id.

***

#### 参与贡献（Contribution）

> 1.  Fork 本仓库。
> 2.  新建 Feat_xxx 分支。
> 3.  提交代码。
> 4.  新建 Pull Request。

> 1.  Fork the repository.
> 2.  Create Feat_xxx branch.
> 3.  Commit your code.
> 4.  Create Pull Request.

***

#### 致谢（Thanks）

> 感谢 Jetbrains 提供的学生版全家桶。

> Here, I appreciate that Jetbrains provides product pack for student.

***

