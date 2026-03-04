## 1. Overview

- Ring Scanner Android SDK is a tool for communication and control with Ring Scanner devices. This SDK is designed so Android application developers can easily integrate Ring Scanner device features.
- This manual provides detailed instructions for installing, configuring, and using the Ring Scanner Android SDK.

## 2. System Requirements

- Android API Level 21 or higher
- Java Development Kit (JDK) 8 or higher
- Java/Kotlin compilation target: JVM 11 or higher

## 3. Adding the Ring_ScanEmul SDK to Your Own Project
To use the Ring ScanEmul SDK in your own app, add the Maven repository and dependency to your Gradle files.

#### 1. Add the Maven repository in your **settings.gradle.kts**
```kotlin
dependencyResolutionManagement {
    repositories {
        google()
        mavenCentral()

        // Ring ScanEmul SDK repository
        maven("https://m3mobile.github.io/ring-scanemul-sdk-maven")
    }
}
```
If you are using **Groovy**

```kotlin
dependencyResolutionManagement {
    repositories {
        google()
        mavenCentral()

        // Ring ScanEmul SDK repository
        maven { url "https://m3mobile.github.io/ring-scanemul-sdk-maven" }
    }
}
```

#### 2. Add the SDK dependency
In your module-level build.gradle or build.gradle.kts
```kotlin
dependencies {
    implementation("com.m3:ring-scanemul-sdk:x.y.z") //Check the latest version in `https://github.com/m3mobile/ring-scanemul-sdk-maven'
}
```

> For more details, please click the [here](https://github.com/m3mobile/wr15-sdk-maven/releases) to visit Ring ScamEmul SDK Repo and refer to the SDK manual.
