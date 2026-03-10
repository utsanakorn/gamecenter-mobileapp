# Architecture Decision Record: Development Framework

## Summary
* **Issue:** Selecting a mobile development framework for "GameCenter" that supports Android and fits the team's skillset.
* **Decision:** **React Native**
* **Status:** Accepted

## Details
* **Assumptions:** The team wants to build a high-performance app with a native feel and has an interest in the React ecosystem.
* **Constraints:** Must be compatible with Android OS and allow for the integration of styling libraries.
* **Positions:** Ionic, Cordova, Framework7, Native Script.
* **Argument:** **React Native** is selected because it provides a "Learn once, write anywhere" advantage and offers superior performance by rendering native components instead of web views. While the project requires Bootstrap, we will use libraries like `react-native-bootstrap` or styled-components to mirror the Bootstrap design language effectively on a native platform.
* **Implications:** The team will need to manage the React state efficiently and ensure that native modules are correctly linked for Android.

## Related
* **Related decisions:** Navigation Strategy, Hardware Access.
* **Related requirements:** Target Device: Android, CSS Framework: Bootstrap (Implementation via React Native styling).
