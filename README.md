# JayjayTestJava
## Background Project

Create a Simple Gradle Task and add libraries on gradle.build

## Function Project

- To Understand how to create a simple Gradle task to receive CLI parameters and print them with a greeting message
- The Gradle script project should be created in a different repository and pushed to GitHub

## How to Run Project

```bash
# create a new gradle
gradle init --type java-library

# open file gradle
build.gradle

# Add script code on build.gradle file
Task greetingTask() {
 doLast {
   String nama = project.hasProperty('nama') ? project.property('nama') : 'Gradle User'
   println "Hello, $nama! Welcome to Gradle World!"
   }
}

# Add libraries depedencies
implementation 'com.google.guava:guava:29.0-jre'
testImplementation 'junit:junit:4.13'

# Run Task
./gradlew greetingTask -Pname=YourName"
```

## ScreenShoot Project
This is result run Project
![ss test_gradle](https://github.com/yuliantisimatupang/JayjayTestJava/assets/45448710/56d3a18c-7299-4cb3-9fb8-e1b2e678f43c)
