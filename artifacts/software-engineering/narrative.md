Milestone Two: Narrative (Enhancement One) – Software Design and Engineering
Artifact Description
The artifact is the Guardian Path Safety Dashboard, a C++ application built using the Qt Framework. Originally conceptualized as a UI/UX mockup in Module One of this capstone course—building upon foundational design concepts from CS-319—it has been significantly enhanced into a modular, high-performance desktop application. The current version serves as a centralized safety hub for caregivers, featuring a integrated dashboard, real-time location tracking, appliance monitoring, and a "Care Ring" contact system.

Justification for Inclusion
I selected this artifact because it demonstrates the critical transition from a "design concept" to a professional "functional system". By refactoring the original basic mockup into this advanced iteration, I have showcased several industry-standard software engineering skills:

Refactoring & Architectural Transition: I moved from a "flat," monolithic file structure where logic was tightly coupled with the UI to a modular directory-based architecture. Each feature (Care Ring, Monitor Appliance, Track Location) now resides in its own dedicated .h and .cpp files. This ensures Separation of Concerns, allowing for feature-specific updates without impacting the stability of the rest of the application.

Object-Oriented Best Practices: By assigning each window and functional area its own class (e.g., TrackLocationWindow or MonitorApplianceWindow), I moved from a "scripting" mindset to a Software Engineering mindset, treating each component as an independent, encapsulated object.

Scalability: The new structure is designed to handle increased complexity, mirroring how professional C++ projects are organized to manage large-scale codebases.

Technical Refinement & Memory Management
A major component of this enhancement was the implementation of robust Software Engineering principles within the C++ environment:

QStackedWidget Implementation: I utilized a QStackedWidget for page navigation. By refactoring the architecture to a "stacked" model, I created a seamless, state-persistent user experience that separates the navigation logic (createSidebar) from the content logic (createPages).

Signal-Slot Refactoring: The transition from basic function calls to Qt’s Signal-Slot mechanism (e.g., connect(btnDashboard, &QPushButton::clicked, this, &MainWindow::navigateToDashboard);) illustrates a modern event-driven approach. This decouples UI buttons from the logic that handles page switching, making the codebase easier to maintain and test.

Memory Management (Qt Object Trees): I leveraged Qt’s Parent-Child Ownership System to handle memory. By passing the parent pointer (this) to the constructors of my widgets (e.g., pageStack = new QStackedWidget(this);), I ensured that when the MainWindow is destroyed, the object tree automatically cleans up all child widgets. This prevents memory leaks without the overhead of manual delete calls.

UI Polish & Styling: I implemented custom property-based styling using setProperty("active", ...) and dynamic style polishing (unpolish/polish). This allows the UI to react visually to user input in real-time, ensuring the application is intuitive for the target audience of caregivers.

Course Outcome Coverage
This enhancement specifically meets several Computer Science program outcomes:

Outcome 2: I designed and delivered visual communications (the Dashboard UI) that are technically sound and appropriately adapted for the caregiver audience, ensuring a professional and coherent user interface.

Outcome 4: By utilizing the Visual Studio environment and standard C++ class structures, I implemented a solution using well-founded techniques that deliver value through organized and maintainable code.

Reflection on the Process
The transition from the Module One mockup to a functional C++ application was a pivotal learning experience. While the mockup established the visual requirements, the actual implementation required a complete architectural overhaul to ensure the software was robust.

The greatest challenge was refactoring the main.cpp and mainwindow.cpp to handle multiple independent windows while maintaining a clean memory footprint. I learned that planning the file hierarchy and object ownership before coding is essential; failure to do so results in significant time lost to "include" errors and circular dependencies.

This process taught me that software engineering is as much about the structural architecture of the system as it is about the logical code within the functions. Facing the challenges of implementation—such as the transition to an event-driven architecture and the dynamic polishing of styles—allowed me to bridge the gap between UI/UX design and backend systems integration.
