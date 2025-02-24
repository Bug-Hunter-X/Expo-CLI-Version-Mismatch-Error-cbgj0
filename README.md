# Expo CLI Version Mismatch

This repository demonstrates a common error encountered when using the Expo CLI: a version mismatch between the globally installed CLI and the version specified in the project's `package.json`.

## Problem

The `expoBug.js` file showcases a project where the locally specified Expo CLI version doesn't match the globally installed version.  Attempting to run `expo start` or `expo build` will often result in an error, indicating a version conflict.

## Solution

The `expoBugSolution.js` file provides a solution.  This involves ensuring both the global and local versions of the Expo CLI are identical. Use `npm install -g expo-cli@<version>` to update the global version,  where <version> is the version required by your project.  You can also update your local version in `package.json` and run `npm install`.