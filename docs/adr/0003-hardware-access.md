# Architecture Decision Record: Hardware Access

## Summary
* **Issue:** Selecting hardware features for game feedback.
* **Decision:** **Capacitor Haptics and Native Audio**
* **Status:** Accepted

## Details
* **Argument:** To enhance the user experience in "GameCenter," we will use **Capacitor Plugins**. We will implement **Haptics** (Vibration) to alert players of wrong moves or game overs, and **Native Audio** to play background music and sound effects (SFX) through the Android **Speaker**.
* **Implications:** We need to install `@capacitor/haptics` and `@capacitor-community/native-audio`.
