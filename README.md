Timesheet Management and Project Budget Monitoring System

Student Name: Saketh Narayanam
SRN: PES1UG24CS292
Project Overview
The Timesheet Management and Project Budget Monitoring System is an individual software engineering project focused on managing the working hours of remote developers and the review of their submitted timesheets.
The system provides a structured workflow where a remote developer can log time and submit a timesheet. The submitted timesheet can then be validated and reviewed by an engineering manager, who can approve or reject it.
The system also supports project budget monitoring by calculating project budget consumption and allowing the engineering manager to view budget burn information.
The current system model includes the following actors:
- Remote Developer
- Engineering Manager
- Jira System
Problem Statement
Managing timesheets for remote developers can become difficult when working hours are recorded and reviewed manually.
A manual process can create problems such as:
- Difficulty in recording working hours consistently.
- Delays in submitting and reviewing timesheets.
- Errors in submitted time information.
- Difficulty in validating timesheets.
- Difficulty in tracking approved and rejected timesheets.
- Extra effort for managers while reviewing timesheets.
- Difficulty in calculating project budget consumption.
- Difficulty in monitoring project budget burn.
This project aims to provide a structured and simple workflow for time logging, timesheet submission, validation, review, approval, rejection, and project budget monitoring.
Objectives
The main objectives of the project are:
1. Allow remote developers to record their working hours.
2. Allow developers to submit timesheets.
3. Validate submitted timesheets before review.
4. Allow engineering managers to review submitted timesheets.
5. Allow engineering managers to approve timesheets.
6. Allow engineering managers to reject timesheets.
7. Calculate project budget consumption.
8. Provide a way to view project budget burn.
9. Maintain a clear and simple workflow for timesheet management.
10. Maintain accurate and consistent timesheet information.
Main Actors
Remote Developer
The Remote Developer is responsible for recording work time and submitting timesheets.
Main activities:
- Log Time
- Submit Timesheet
Engineering Manager
The Engineering Manager reviews submitted timesheets and handles approval or rejection.
Main activities:
- Review Timesheet
- Approve Timesheet
- Reject Timesheet
- View Budget Burn
Jira System
The Jira System is represented as an external system in the use-case model and is associated with the time-logging workflow.
Main Use Cases
Use Case	Description
Log Time	Record the time spent on project work.
Submit Timesheet	Submit recorded working hours for review.
Validate Timesheet	Check whether the submitted timesheet is valid.
Review Timesheet	Allow the engineering manager to examine the submitted timesheet.
Approve Timesheet	Approve a timesheet after review.
Reject Timesheet	Reject a timesheet when it does not satisfy the required conditions.
Calculate Project Budget Consumption	Calculate the amount of project budget consumed.
View Budget Burn	Display the current project budget consumption or burn information.


System Workflow
The main timesheet workflow is:
Remote Developer
       |
       v
   Log Time
       |
       v
Submit Timesheet
       |
       v
Validate Timesheet
       |
       v
Review Timesheet
      / \
     /   \
    v     v
Approve  Reject

The budget monitoring workflow is:
Project Data
      |
      v
Calculate Project Budget Consumption
      |
      v
View Budget Burn

Requirements Engineering
Functional Requirements
The Functional Requirements define what the system should do.
The main functional requirements include:
- The system shall allow a remote developer to log working time.
- The system shall allow a remote developer to submit a timesheet.
- The system shall validate submitted timesheet information.
- The system shall allow an engineering manager to review submitted timesheets.
- The system shall allow an engineering manager to approve a timesheet.
- The system shall allow an engineering manager to reject a timesheet.
- The system shall calculate project budget consumption.
- The system shall allow the engineering manager to view budget burn information.
Non-Functional Requirements
The Non-Functional Requirements define how the system should perform.
The project considers:
- Performance
- Security
- Usability
- Reliability
- Maintainability
Examples include:
- The system should respond to normal requests within the defined response time.
- Protected functions should only be accessible to authorized users.
- Timesheet information should be stored securely.
- The interface should be simple and easy to use.
- Timesheet and budget information should remain consistent.
Requirements Traceability Matrix
The Requirements Traceability Matrix connects requirements with their corresponding use cases and test cases.
The basic relationship is:
Requirement
     |
     v
  Use Case
     |
     v
 Test Case

Example:
FR - Submit Timesheet
        |
        v
UC - Submit Timesheet
        |
        v
TC - Submit Timesheet Successfully

The complete RTM is maintained in the 01_RE folder.
Architecture and Design
The architecture section explains how the system is organized and how the main parts communicate.
The architecture documentation includes:
- Architecture Diagram
- Architecture Pattern
- Component Diagram
- UML Use Case Diagram
- Sequence Diagrams
- API Design
- Error Handling Design
The system is planned using separate layers for the user interface, application logic, and data management so that the project remains easier to understand, develop, test, and maintain.
Software Requirements Specification
The SRS describes the expected behavior and requirements of the system.
The SRS contains:
- Introduction
- Problem Statement
- Objectives
- Scope
- Actors
- Functional Requirements
- Non-Functional Requirements
- Security Requirements
- Use Cases
- Constraints
- Assumptions
The SRS is maintained in the 04_SRS_WBS folder.
Work Breakdown Structure
The Work Breakdown Structure divides the project into smaller activities.
Timesheet Management and Project Budget Monitoring System
│
├── 1. Requirements
│   ├── Problem Statement
│   ├── Functional Requirements
│   ├── Non-Functional Requirements
│   ├── Security Requirements
│   └── Use Cases
│
├── 2. Design
│   ├── Architecture
│   ├── Component Diagram
│   ├── UML Use Case Diagram
│   ├── Sequence Diagrams
│   └── API Design
│
├── 3. Development
│   ├── User Interface
│   ├── Application Logic
│   ├── Database
│   └── Integration
│
├── 4. Testing
│   ├── Test Cases
│   ├── Bug Identification
│   ├── Bug Fix
│   ├── Patch
│   └── Retesting
│
└── 5. Deployment
    ├── Environment Setup
    └── Deployment

The detailed WBS is maintained in the 04_SRS_WBS folder.
Project Creation and Management Evidence
The repository will contain evidence showing how the project was created and managed.
GitHub Evidence
The GitHub section should contain screenshots showing relevant project activity such as:
- Repository creation
- Repository structure
- Commits
- Branches, if used
- Project activity
Jira Evidence
The Jira section should contain screenshots showing:
- Jira project
- Backlog
- Scrum board
- Sprint
- Tasks or issues
- Task status
These screenshots are maintained in the 03_Project_Creation folder.
GitHub Copilot
GitHub Copilot is included as part of the project development evidence.
The Copilot section should contain:
- Screenshots of GitHub Copilot being used.
- Evidence of generated or suggested project code.
- Evidence of reviewing or modifying the generated code.
- Repository or project link related to the work.
The purpose of this section is to show the use of AI-assisted coding during development.
These materials are maintained in the 05_GitHub_Copilot folder.
Software Testing Tools and Bug Fixing
The project includes a software testing activity that demonstrates the complete bug-fixing process.
The process is:
Bug Found
    |
    v
Test Fails
    |
    v
AI / Copilot Assistance
    |
    v
Code Fix / Patch
    |
    v
Retest
    |
    v
Test Passes

The testing-tools folder should contain evidence for:
1. The bug before fixing.
2. The failing test or incorrect behavior.
3. AI/Copilot assistance used for the fix.
4. The code patch or corrected implementation.
5. Retesting after the fix.
6. The final test result.
The related evidence is maintained in the 06_Software_Testing_Tools folder.
Testing
Testing is based on the system requirements.
Functional Testing
Functional testing covers:
- Logging time
- Submitting timesheets
- Validating timesheets
- Reviewing timesheets
- Approving timesheets
- Rejecting timesheets
- Calculating budget consumption
- Viewing budget burn
Non-Functional Testing
The project also considers:
- Performance
- Security
- Usability
- Reliability
- Maintainability
Bug Fixing and Retesting
A selected defect is tested before and after the fix to demonstrate the complete process from bug identification to successful retesting.
Scope
In Scope
- Time logging
- Timesheet submission
- Timesheet validation
- Timesheet review
- Timesheet approval
- Timesheet rejection
- Project budget consumption calculation
- Budget burn viewing
External System
- Jira System
Additional features, if implemented later, will be documented in the SRS and related design documents.
Repository Structure
The individual project repository follows the required structure.
MyProject_ShortName/
│
├── README.md
│
├── 01_RE/
│   ├── Functional Requirements
│   ├── Non-Functional Requirements
│   └── Requirements Traceability Matrix
│
├── 02_Architectural_Diagram/
│   └── Architecture and design diagrams
│
├── 03_Project_Creation/
│   ├── GitHub/
│   └── Jira/
│
├── 04_SRS_WBS/
│   ├── Software Requirements Specification
│   └── Work Breakdown Structure
│
├── 05_GitHub_Copilot/
│   ├── Screenshots/
│   └── README.md
│
└── 06_Software_Testing_Tools/
    ├── Bug_Before_Fix/
    ├── AI_Fix/
    ├── Patch/
    ├── Retest/
    └── README.md

Tools and Technologies
The project may use software engineering and development tools such as:
- GitHub
- GitHub Copilot
- Jira
- Git
- Frontend technologies
- Backend technologies
- Database technologies
The final technology list will be updated according to the actual implementation.
Project Status
The project is currently being developed and documented as an individual Software Engineering project.
The repository is being maintained with the required:
- Requirements documentation
- Architecture and design
- SRS
- Work Breakdown Structure
- GitHub and Jira evidence
- GitHub Copilot evidence
- Software testing evidence
- Bug-fixing and retesting evidence
The repository will be updated as development and testing progress.
Student Details
Name: Saketh Narayanam
SRN: PES1UG24CS292
Conclusion
The Timesheet Management and Project Budget Monitoring System is designed to provide a structured workflow for recording working hours, submitting and validating timesheets, reviewing them, and handling approval or rejection.
The project also supports project budget monitoring through budget consumption calculation and budget burn viewing.
The individual repository is organized to contain the required Requirements Engineering, Architectural Diagram, Project Creation evidence, SRS and Work Breakdown Structure, GitHub Copilot evidence, and Software Testing Tools activities.
