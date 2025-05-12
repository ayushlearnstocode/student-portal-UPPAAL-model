# student-portal-UPPAAL-model
Formal system model of a student portal using UPPAAL, representing component interactions like authentication, transcript fetching, and scholarship applications. Includes verification queries to ensure system correctness.


# Student Portal System Model (UPPAAL)

This project contains a formal system model of a student portal designed using **UPPAAL**, a tool for modeling, simulation, and verification of real-time systems.

##  Components Modeled
- **Student**: Logs in, views information, applies for scholarships.
- **Portal**: Handles authentication, routing, and interaction logic.
- **Server**: Fetches student transcripts.
- **Committee**: Approves or rejects scholarship applications based on CGPA.
- **Information System**: Sends student data upon request.

##  Features
- **Channel synchronization** between components (e.g., `authStart`, `transcriptFetch`, `applyscholarship`).
- **Global and local variables** for system state (e.g., `validCredentials`, `cg`, `approved`, `applied`).
- **Formal verification queries** included:
  - Deadlock freedom: `A[] not deadlock`
  - Correct transitions and safety checks using CTL logic

##  Files
- `student_portal_model.xml`: The UPPAAL system model.
- `queries.xml`: Verification queries demonstrating system correctness.

##  Notes
This model was built as part of a university course project to explore formal methods and system verification.

##  Requirements
- UPPAAL installed: [https://uppaal.org](https://uppaal.org)

---

