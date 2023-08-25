# Report DAT250: Software Technology Experiment Assignment 1

I'm currently working on Mac OS

## Getting the software development enviroment up and running 
Following the instrunctions provided, I installed the following programs:
 - Java Development Enviroment (JDK)
 - An Integrated Development Enviroment (IDE)
 - Gradle build tool
 - Git
 - Podman or Docker

### Java 
I began with intalling SDKman. I first had to intall homebrew, which I then used to install SDKman.
The installation seemed to be successful.
![output when checking the version of sdkman](bilder/sdkman_version.png)

I then installed the latest version of java with SDKman, and verified that the version indeed was >= 11:
![output when checking the version of java] (bilder/java_version.png)

### IDE
I chose to download the JetBrains IntelliJ IDE.
The download was pretty straight forward, installing it from JetBrains pages. 
I let all settings be set to default. 

### Gradle
Gradle installation:
```
sdk install gradle 
```
![gradle download successful] (bilder/gradle_downloaded.png)

### Git
I already have git installed om my computer:

![](bilder/git.png)

### Containers
I installed podman on my machine and created an account on DockerHub

## The Exercise
### Step 3 Fix compilation errors
As expected, there are a few errors occuring when trying to run the application
![](bilder/error_app.png)

I fixed the dependency error by adding the missing dependency in the build.gradle.kts file:
```dependencies {
    implementation("io.javalin:javalin:3.13.6")
    // Andre avhengigheter kan også være her
}
```
After rebuilding the project, I tried to run
```/gradlew run```
and got the following error
![](bilder/error_app2.png)
The error indicated that a greetings method is expected, when running the Tests. I then added a quick greetings method:
```
public String getGreeting() {
    return "Welcome to the Unit Converter App!";
}
```
and tried once again to run
```/gradlew run``` 
![](bilder/successful_build.png)

This time the run was successful.

## Step 4 Quality Assurance 

## Step 5: Package Application



https://hub.docker.com/repository/docker/veronicha/dat250/
