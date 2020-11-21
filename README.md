# scala-gradle
scala 프로젝트 빌드를 gradle로 하는 예제 입니다.

기존 프로젝트에 gradle을 추가하기 위해서는 다음 프로세스를 따라하시면 됩니다.
```
> sdk (or brew) i gradle

# 프로젝트 폴더 root에서
> gradle init

Select type of project to generate:
  1: basic
  2: application
  3: library
  4: Gradle plugin
Enter selection (default: basic) [1..4] 2

Select implementation language:
  1: C++
  2: Groovy
  3: Java
  4: Kotlin
  5: Scala
  6: Swift
Enter selection (default: Java) [1..6] 5

Select build script DSL:
  1: Groovy
  2: Kotlin
Enter selection (default: Groovy) [1..2] 1

Project name (default: demo):
Source package (default: demo):


BUILD SUCCESSFUL
2 actionable tasks: 2 executed
```

프로젝트 루트가 다음과 같은 폴더 구조를 가지게 됩니다.
```
[Project Name]
├── gradle 
│   └── wrapper
│       ├── gradle-wrapper.jar
│       └── gradle-wrapper.properties
├── gradlew 
├── gradlew.bat 
├── settings.gradle.kts 
└── app
    ├── build.gradle.kts 
    └── src
        ├── main
        │   └── scala 
        │       └── demo
        │           └── App.scala
        └── test
            └── scala 
                └── demo
                    └── AppSuite.scala
```
