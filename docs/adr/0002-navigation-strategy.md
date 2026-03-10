# Architecture Decision Record: Navigation Strategy

## Summary
* **Issue:** How users will navigate between game modules and menus in a React Native environment.
* **Decision:** **React Navigation (Tab and Stack)**
* **Status:** Accepted

## Details
* **Assumptions:** The app requires a smooth transition between the game library and individual gameplay screens.
* **Constraints:** Must follow the standard Android back-button behavior.
* **Positions:** Drawer Navigation, Single-page state switching.
* **Argument:** We will use the **React Navigation** library, specifically combining **Bottom Tab Navigation** for the main sections (Home, Games, Scores) and **Stack Navigation** for moving between the game list and the active game session. This provides the most "native" user experience on Android.
* **Implications:** Requires installation of `@react-navigation/native` and associated dependencies.

## Related
* **Related decisions:** Development Framework (React Native).
