# spring-boot-build

[![Maven Central](https://img.shields.io/maven-central/v/app.myoss.cloud/spring-boot-build.svg)](https://maven-badges.herokuapp.com/maven-central/app.myoss.cloud/spring-boot-build/)
[![GitHub release](https://img.shields.io/github/release/myoss-cloud/spring-boot-build.svg)](https://github.com/myoss-cloud/spring-boot-build/releases)
[![License](https://img.shields.io/badge/license-Apache%202-4EB1BA.svg)](https://www.apache.org/licenses/LICENSE-2.0.html)

## Documentation

- [Documentation Home](https://cloud-docs.myoss.app/artifact-version/manage-dependencies.html)

## Download

- [maven][1]
- [the latest JAR][2]  

[1]: http://repo1.maven.org/maven2/app/myoss/cloud/spring-boot-build/  
[2]: https://search.maven.org/remote_content?g=app.myoss.cloud&a=spring-boot-build&v=LATEST

## Maven

```xml
<dependency>
    <groupId>app.myoss.cloud</groupId>
    <artifactId>spring-boot-build</artifactId>
    <version>2.1.16.RELEASE</version>
</dependency>
```

```xml
<dependency>
    <groupId>app.myoss.cloud</groupId>
    <artifactId>myoss-spring-boot-parent</artifactId>
    <version>2.1.16.RELEASE</version>
</dependency>
```

```xml
<dependency>
    <groupId>app.myoss.cloud</groupId>
    <artifactId>myoss-cloud-dependencies</artifactId>
    <version>2.1.16.RELEASE</version>
</dependency>
```

## Usage

1. `pom.xml` 继承的方式

    ```xml
        <parent>
            <groupId>app.myoss.cloud</groupId>
            <artifactId>myoss-spring-boot-parent</artifactId>
            <version>2.1.16.RELEASE</version>
        </parent>
    ```

2. `pom.xml` 使用 `import` 的方式

    ```xml
        <dependencyManagement>
            <dependencies>
                <dependency>
                    <groupId>app.myoss.cloud</groupId>
                    <artifactId>myoss-cloud-dependencies</artifactId>
                    <version>${myoss-cloud-dependencies.version}</version>
                    <type>pom</type>
                    <scope>import</scope>
                </dependency>
            </dependencies>
        </dependencyManagement>
    ```