# Architecture Decision Record: Development Framework

## Summary
* **Issue:** Selecting a mobile framework for "GameCenter" that supports React, TypeScript, and Bootstrap.
* **Decision:** **Ionic Framework (React + TypeScript)**
* **Status:** Accepted

## Details
* **Assumptions:** The team will use React and TypeScript as taught in class, while needing to integrate Bootstrap CSS for the UI.
* **Constraints:** Must be a functional Android app and use the Bootstrap framework.
* **Positions:** React Native, Cordova, Flutter.
* **Argument:** We selected **Ionic** because it is a hybrid framework that allows us to write standard **React and TypeScript** code while fully supporting **Bootstrap CSS**. Unlike React Native, Ionic uses web standards, meaning we can import the official Bootstrap library directly without any compatibility issues. This ensures we meet all project requirements efficiently.
* **Implications:** We will use Capacitor to deploy the app to Android devices.

## Related
* **Related requirements:** Android Target, Bootstrap CSS Framework, TypeScript.
