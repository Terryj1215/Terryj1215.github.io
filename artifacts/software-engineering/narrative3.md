Milestone Four: Narrative (Enhancement Three) – Databases
Artifact Description
The artifact is the Care Ring and Dashboard synchronization system within the Guardian Path Dashboard, a C++ application built using the Qt Framework. Originally conceptualized as a UI/UX mockup with hardcoded sample data, it was significantly enhanced in February 2026 to include a persistent, cloud-based data layer. The current version features a fully integrated MongoDB backend that manages emergency contacts and system status in real-time, ensuring that critical safety information persists across user sessions.


Justification for Inclusion
I selected this artifact for my ePortfolio because it demonstrates the critical transition from "volatile local memory" to "persistent cloud-based storage." By bridging the gap between a high-performance C++ frontend and a NoSQL database, I have showcased several industry-standard skills in Databases and Software Engineering:

NoSQL Implementation (CRUD): I implemented full Create, Read, Update, and Delete functionality using the MongoDB C++ driver, allowing caregivers to manage "Care Ring" members dynamically rather than relying on static code.

Data Structure Refactoring: I refactored the core Contact data model to handle MongoDB ObjectIDs (OIDs) by transitioning from integer-based IDs to QString identifiers. This demonstrates my ability to adapt local data structures to meet the requirements of external database schemas.

Architectural Data Integration: By implementing a "Clear-and-Reload" strategy, I ensured the UI strictly pulls from the database "source of truth," eliminating data desynchronization errors, often referred to as the "Double-Add" bug.

Technical Refinement & Concrete Outcomes
A major focus of this enhancement was moving from a "design concept" to a "functional system" that can handle real-world data persistence:

Persistent Emergency Profiles: In previous versions, adding a contact was a temporary action that vanished upon closing the app. The new version ensures that every emergency contact added to the "Care Ring" is immediately saved to the MongoDB contacts collection.

State-Persistent Dashboard: I synchronized the main Dashboard with the database so that "Quick Contacts" are dynamically generated based on the current database state. This ensures that when a caregiver marks a contact as "Primary," that change is reflected across all modules of the application instantly.

Asynchronous Connection Handling: During integration, I developed logic to handle database latency. By implementing a status-check system, I ensured the application remains responsive while waiting for the MongoDB handshake, providing a seamless user experience for the caregiver.

Course Outcome Coverage
This enhancement specifically meets several Computer Science program outcomes:


Outcome 3 (Databases): I designed and implemented a computing solution that utilizes a NoSQL database (MongoDB) to manage complex data relationships, ensuring information persistence and accessibility.


Outcome 4 (Software Engineering/Tools): By utilizing the vcpkg package manager to integrate the MongoDB C++ driver and maintaining a modular directory-based architecture, I implemented a solution using professional-grade tools and maintainable code structures.


Reflection on the Process
The process of enhancing this artifact provided a deep dive into the complexities of State Management and Persistence. While Enhancement One established the "skeleton" and Enhancement Two provided the "mathematical intelligence", this phase provided the "memory" of the Guardian Path system.


One of the most significant challenges was refactoring the file hierarchy to avoid circular dependencies when sharing the database manager instance across multiple independent windows. I learned that planning the data flow and object ownership before coding is essential to prevent "include" errors and system instability. Facing the challenges of implementation—such as translating MongoDB BSON documents into Qt-compatible JSON objects—allowed me to bridge the gap between high-level UI design and professional backend systems integration.
