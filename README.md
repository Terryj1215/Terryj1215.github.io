# Terry Johnson | Computer Science ePortfolio
## Full-Stack & DevOps Professional

Welcome to my professional ePortfolio. I have been in the SNHU Computer Science program since August 2022. This site serves as a showcase for my technical growth, bridging my 3 years of experience in IT/Networking with advanced software engineering practices.

Professional Self-Assessment: 

[Read Self-Assessment](./artifacts/software-engineering/Professional%20Self-Assessment.md)

Code Review
https://youtu.be/DuH-HScd0bM

Original Code
https://github.com/Terryj1215/Guardian_Path_Application/tree/8558443590361873466ab6f8090d39af01d926fd/GuardianPath

Enahnced Code
https://github.com/Terryj1215/Guardian_Path_Application/tree/main/resources

### Current Project: Guardian Path

* **Software Engineering (Enhancement One):** [Read Narrative](./artifacts/software-engineering/narrative.md) | [View Source Code](https://github.com/Terryj1215/Guardian_Path_Application)
    * Successfully transitioned from a paper prototype to a modular C++ architecture using Visual Studio and the Qt Framework.
    * Implemented a centralized safety hub featuring real-time location tracking and appliance monitoring.
    * Utilized Qt’s Signal-Slot mechanism for event-driven navigation and managed memory via Qt Object Trees to prevent leaks.

![Guardian Path Dashboard](./assets/Screenshot%202026-01-25%20192904.png) 
*Caption: The enhanced modular Dashboard featuring the Emergency SOS system.*

* **Algorithms and Data Structure (Enhancement Two):** [Read Narrative](./artifacts/software-engineering/narrative2.md) | [View Source Code](https://github.com/Terryj1215/Guardian_Path_Application/tree/main/src)
    * Developed a dynamic geospatial engine by implementing the **Haversine Formula** to calculate great-circle distances for real-time geofence validation.
    * Integrated an **Asynchronous Geocoding Search Algorithm** to transform string-based user input into precise geographic coordinates ($Latitude, Longitude$).
    * Engineered a **Cross-Platform Data Bridge** between C++ backend logic and a QML frontend to maintain state-persistence across the mapping layer.
    * Optimized spatial data structures to support user-defined safety parameters, allowing for dynamic real-time updates to the geofence boundary.

![Guardian Path Map Enhancement](./assets/Screenshot%202026-02-01%20150608.png)
*Caption: The interactive mapping interface featuring the Geocoding search bar and dynamic Geofence circle.*

* **Databases (Enhancement Three):** [Read Narrative](./artifacts/software-engineering/narrative3.md) | [View Source Code](https://github.com/Terryj1215/Guardian_Path_Application)
    * Integrated a professional **MongoDB NoSQL backend** to move from volatile local memory to a persistent cloud-based data layer.
    * Implemented full **CRUD functionality** using the MongoDB C++ driver, enabling dynamic management of "Care Ring" emergency contacts.
    * Refactored core data models to utilize **QString identifiers**, mapping UI elements directly to MongoDB ObjectIDs (OIDs) for precise data targeting.
    * Engineered a synchronization logic that ensures the Dashboard and Care Ring views maintain state-persistence and parity with the database "source of truth."

![Guardian Path Care Ring Enhancement](./assets/Screenshot%202026-02-08%20142332.png)
*Caption: The persistent Care Ring system integrated with MongoDB, featuring real-time contact synchronization and primary member assignment.*
