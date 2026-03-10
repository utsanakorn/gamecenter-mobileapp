# Architecture Decision Record: Hardware Access

## Summary
* **Issue:** Which Android hardware features are needed and how to access them in React Native.
* **Decision:** **Speaker (Audio) and Vibration (Haptics)**
* **Status:** Accepted

## Details
* **Assumptions:** Audio and haptic feedback are essential for an immersive gaming experience.
* **Constraints:** Accessing hardware must be done via React Native bridge or libraries like Expo (if used) or React Native Community packages.
* **Positions:** GPS, Camera, Accelerometer.
* **Argument:** For "GameCenter", we prioritize **Speaker** access for game sound effects and **Vibration** for tactile feedback during key game events (e.g., losing a life). These are achieved through stable libraries like `react-native-sound` and the built-in `Vibration` API.
* **Implications:** We must ensure the correct permissions are added to the `AndroidManifest.xml` file.

## Related
* **Related requirements:** Target Device: Android.
