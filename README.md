# Expo Web Build Error: Third-party library accessing `window` object throws runtime error

This repository demonstrates a bug encountered while building an Expo project for web. A third-party library attempts to access the `window` object, leading to a runtime error when the `window` object is not immediately accessible. The solution involves using conditional rendering and checking for window availability before accessing window-related methods or properties.

## Bug Description

While building an Expo project for web, we encountered an unexpected runtime error. A third-party library was attempting to access the `window` object in a context where it was not available. This caused the web build to fail.  The library functions correctly in native mobile environments.