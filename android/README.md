## SDK Setup Guide
## Android
To integrate the SDK into your Android project, please follow the steps outlined below:

Download the SDK artifact (AAR file) from the provided source.

Place the downloaded artifact in a directory named libs within your project.

Open your project's build.gradle file and ensure that the following repositories are included:

```groovy
repositories {
    google()
    mavenCentral()
    flatDir {
        dirs 'libs'
    }
}
```
The google() and mavenCentral() repositories are standard repositories for Android projects, while the flatDir repository is used to include the local AAR file.

Add the SDK as a dependency in your project's build.gradle file:

Copy code
```groovy
dependencies {
    implementation(name: 'povium_stream-0.0.1', ext: 'aar')
}
```
Replace 'povium_stream-0.0.1' with the actual name of the downloaded AAR file (without the file extension).

Sync your project with the Gradle files to apply the changes.

Congratulations! You have successfully set up the SDK in your Android project. You can now proceed with utilizing the SDK's functionalities in your application code.

If you encounter any issues or require further assistance, please refer to the SDK documentation or reach out to the SDK provider for support.
