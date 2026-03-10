# Architecture Decision Record: Database Storage

## Summary
* **Issue:** How to store high scores and user settings locally in React Native.
* **Decision:** **AsyncStorage**
* **Status:** Accepted

## Details
* **Assumptions:** Data is simple, non-sensitive, and needs to be saved locally on the device.
* **Constraints:** Must be easy to implement within the project scope without a complex database engine.
* **Positions:** SQLite, Realm, Firebase (Remote).
* **Argument:** **AsyncStorage** is the standard for simple key-value storage in React Native. It is perfect for saving high scores and usernames locally. It fits our project's **Scope** perfectly as it doesn't require setting up a heavy database or an external server.
* **Implications:** Data is stored as strings, so we will need to use `JSON.stringify` and `JSON.parse` for object data.

## Related
* **Related decisions:** Development Framework (React Native).
