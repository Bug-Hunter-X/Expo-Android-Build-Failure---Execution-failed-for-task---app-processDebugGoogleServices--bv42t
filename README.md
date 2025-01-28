# Expo Android Build Failure: `processDebugGoogleServices`

This repository demonstrates a common but elusive bug encountered when building Android apps using Expo CLI. The build process fails with an error message involving `Execution failed for task ':app:processDebugGoogleServices`. This issue typically arises from misconfigurations or conflicts within the project's Gradle setup, specifically concerning the Google Services Gradle plugin.

## Reproduction

The `bug.js` file shows a basic Expo app structure.  Attempting to build this app (under specific conditions detailed in the `bug.js` comments) will likely trigger the error.

## Solution

The `bugSolution.js` file demonstrates solutions to resolve the issue. This includes steps for checking:

*   Correct `google-services.json` placement and contents.
*   Gradle dependency conflicts.
*   Cleaning and rebuilding the project.
*   Checking Android SDK and build tools versions.

This solution focuses on diagnosing and resolving conflicts related to `google-services.json` and Gradle dependencies, covering the most common causes of the error.