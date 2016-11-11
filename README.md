#Issue

When using version 2.3.0-alpha1 of the Android gradle plugin enabling databinding on a module annotation processing no longer works and or it doesn't generate and code

###To Reproduce
1. Checkout Project
2. Build from commandline using **./gradlew clean assembleDebug**
3. Look at generated code in **app/build/generated/source/apt/debug**
4. Notice that only databinding code is generated
5. open **app/build.gradle** and disable databinding
6. Rebuild project using **./gradlew clean assembleDebug**
7. Look at generated code again in **app/build/generated/source/apt/debug**
8. Notice that Dagger code is now being generated.