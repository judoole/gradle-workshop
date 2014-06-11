# Gradle init
To start off a Gradle project with a bang, move to the folder of your choice and issue the command:

```gradle init```

This will generate a folder structure like this

```zsh
build.gradle
gradle/
gradlew*
gradlew.bat
settings.gradle
```
**All of this should be commited to version control.**

**build.gradle** - This is where the magic happens. Your source so to speak.

**gradle/** - In here lies files needed for the gradlew (wrapper) scripts. This includes a small jar-file and some wrapper properties. You'll probably never edit the gradle/wrapper folder yourself, but the gradle/ folder is a nice place to put files to import in your build.gradle.

**gradlew* and gradle.bat** - These to nice scripts ensures that everyone that wants to build your project only need JAVA_HOME set. The scripts will download the proper version of gradle and the happy programmers are ready to roll. Proper version means that if you, the owner, decided to use version 1.9 of Gradle, *even if last version is 1.12*, gradlew ensures that 1.9 will be used throughout. Awesome!

**settings.gradle** - In here you specify name of the project and any submodules if need be.
