# Expo CLI Android Build Error: AGP Version Mismatch

This repository demonstrates a common issue encountered when building Android apps with the Expo CLI: an incompatibility between the project's Android Gradle Plugin (AGP) version and Expo's requirements.  The problem typically surfaces as a cascade of dependency resolution failures, making it difficult to pinpoint the root cause.

## Problem
The `android/gradle/wrapper/gradle-wrapper.properties` file might specify an AGP version that conflicts with the version Expo needs. This leads to a series of errors during the build process, often obscuring the actual cause.

## Solution
The solution involves updating the `gradle-wrapper.properties` file to use an AGP version compatible with Expo.  This typically requires checking the Expo documentation for the recommended or supported AGP version for your Expo SDK version.  Sometimes, simply updating the Gradle wrapper might be sufficient to resolve the incompatibility.

## Setup
1. Clone this repository.
2. Examine the `bug.gradle` file (simulating a problematic configuration).
3. Observe the build errors.
4. Apply the fix in `bugSolution.gradle` to see the resolution.