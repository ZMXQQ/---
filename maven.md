# maven

## 一：Maven简介

### 1:什么是maven?

maven是apache的一个**项目管理和构建**工具,可以帮助我们创建和管理项目

### 2:为什么使用maven?

#### 2.1、项目管理工具 

当你的项目规模很大时，需要将项目进行拆分，将一个项目拆分成多个模块，每一个模块对应一个工程,多个工程之间存在依赖关系。可以采用maven的依赖管理规则，帮助我们在项目和项目之间建立依赖关系

#### 2.2、jar包的管理工具

* 通过仓库管理jar包
* 解决jar包的依赖
* 自动下载jar包

#### 2.3、自动化的构建工具

构建过程:编译主代码----->编译测试代码------>执行单元测试------>生成测试报告--->打包----->部署

### 3:术语

#### 3.1、中央仓库

是一个网络仓库，存储jar包和maven插件

http://repo.maven.apache.org/maven2

http://repo1.maven.org/maven2

#### 3.2、本地仓库

从中央仓库下载的jar包的存放位置，也是一个仓库，只是存放在本地电脑上

#### 3.3、镜像仓库

对某一个仓库进行镜像

阿里云提供的镜像仓库：

http://maven.aliyun.com/nexus/content/groups/public/

#### 3.4、私服

局域网内部搭建的maven服务器

#### 3.5、各个仓库之间的关系

![1](pic/1.jpg)

## 二：安装maven

apache-maven-3.2.5,要求jdk1.6即可,其后的版本jdk至少1.7

* 配置环境变量

  maven依赖JAVA_HOME

  ```
  echo %JAVA_HOME%  --windows
  echo $JAVA_HOME    ---linux
  ```

  需要配置M2_HOME,path

  M2_HOME=D:\maven\apache-maven-3.2.5

  path=原path;%M2_HOME%/bin

* 测试

  在控制台输入：mvn -version

  输出结果：

  Apache Maven 3.2.5 (12a6b3acb947671f09b81f49094c53f426d8cea1; 2014-12-15T01:29:23+08:00)
  Maven home: D:\maven\apache-maven-3.2.5
  Java version: 1.8.0_171, vendor: Oracle Corporation
  Java home: C:\Program Files\Java\jdk1.8.0_171\jre
  Default locale: zh_CN, platform encoding: GBK
  OS name: "windows 7", version: "6.1", arch: "amd64", family: "dos"
  C:\Users\hellboy>

  表示maven安装成功

  ​





























