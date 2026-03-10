# Architecture Decision Record: Database Storage

## Summary
* **Issue:** How to store player data, such as usernames and high scores.
* **Decision:** **Local Storage (Unencrypted)**
* **Status:** Accepted

## Details
* **Assumptions**: Data is non-sensitive and only needs to persist on the user's local device.

* **Constraints**: No requirement for online accounts or cross-device syncing.

* **Positions**: Remote Database (Firebase/SQL), Encrypted Local Storage, No Database.

* **Argument**: Local Storage (specifically Ionic Storage or Web Storage) is the best fit. It is simple to implement and fits perfectly within the course Scope. Since we are not storing passwords or personal data, encryption is unnecessary, reducing complexity while still allowing high scores to be saved after the app is closed.

* **Implications**: Data will be lost if the user clears their app cache or uninstalls the app.

# Related
* Related requirements: Performance and Scope management.
