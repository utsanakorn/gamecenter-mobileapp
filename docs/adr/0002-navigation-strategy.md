# Architecture Decision Record: Navigation Strategy

## Summary
* **Issue:** **How users will navigate between different games and menus within GameCenter.**
* **Decision:** **Tab Bar with Stack Navigation**
* **Status:** Accepted

## Details
* **Argument:** A Tab Bar (Bottom Navigation) provides quick access to core sections: "Home", "Games", and "Scores". Inside each game, Stack Navigation will be used to allow users to go "into" a game and "back" to the main list. This is the industry standard for mobile gaming hubs.
* **Implications:** We need to implement a routing system (like Ionic Router) to manage the history of the "back" button on Android.

* **Related** Related decisions: Development Framework (Ionic Router).
