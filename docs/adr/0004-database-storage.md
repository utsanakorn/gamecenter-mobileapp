# Architecture Decision Record: Database Storage

## Summary
* **Issue:** Choosing a method for persistent local data storage.
* **Decision:** **Ionic Storage (Key-Value)**
* **Status:** Accepted

## Details
* **Argument:** We will use **Ionic Storage**, which provides a simple way to store data like high scores and player preferences locally on the Android device. It is more robust than standard Web LocalStorage and fits perfectly within the course **Scope**, as it doesn't require a complex cloud setup.
* **Implications:** Data will be stored in a key-value format using TypeScript interfaces for type safety.
