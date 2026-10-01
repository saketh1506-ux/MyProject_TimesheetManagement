# Timesheet Management and Project Budget Monitoring System

**Student:** Saketh Narayanam
**SRN:** PES1UG24CS292

An individual software engineering project for managing remote developers' working hours, reviewing submitted timesheets, and monitoring project budget burn.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [Actors](#actors)
- [Use Cases](#use-cases)
- [System Workflow](#system-workflow)
- [Requirements Engineering](#requirements-engineering)
- [Architecture and Design](#architecture-and-design)
- [Software Requirements Specification](#software-requirements-specification)
- [Work Breakdown Structure](#work-breakdown-structure)
- [Project Creation and Management Evidence](#project-creation-and-management-evidence)
- [GitHub Copilot](#github-copilot)
- [Software Testing Tools and Bug Fixing](#software-testing-tools-and-bug-fixing)
- [Testing](#testing)
- [Scope](#scope)
- [Repository Structure](#repository-structure)
- [Tools and Technologies](#tools-and-technologies)
- [Project Status](#project-status)
- [Conclusion](#conclusion)

---

## Project Overview

A remote developer logs time and submits a timesheet. An engineering manager validates and reviews it, then approves or rejects it. The system also calculates project budget consumption and lets the engineering manager view budget burn.

## Problem Statement

Managing timesheets for remote developers is difficult when hours are recorded and reviewed manually. Common problems:

- Inconsistent recording of working hours
- Delays in submitting and reviewing timesheets
- Errors in submitted time information
- Difficulty validating timesheets
- Difficulty tracking approved and rejected timesheets
- Extra effort for managers during review
- Difficulty calculating project budget consumption
- Difficulty monitoring project budget burn

This project provides a structured, simple workflow for time logging, submission, validation, review, approval, rejection, and budget monitoring.

## Objectives

1. Allow remote developers to record their working hours
2. Allow developers to submit timesheets
3. Validate submitted timesheets before review
4. Allow engineering managers to review submitted timesheets
5. Allow engineering managers to approve timesheets
6. Allow engineering managers to reject timesheets
7. Calculate project budget consumption
8. Provide a way to view project budget burn
9. Maintain a clear and simple workflow for timesheet management
10. Maintain accurate and consistent timesheet information

## Actors

| Actor | Role | Main Activities |
|---|---|---|
| **Remote Developer** | Records work time and submits timesheets | Log Time, Submit Timesheet |
| **Engineering Manager** | Reviews submitted timesheets and handles approval or rejection | Review, Approve, Reject, View Budget Burn |
| **Jira System** | External system associated with the time-logging workflow | - |

## Use Cases

| Use Case | Description |
|---|---|
| Log Time | Record the time spent on project work |
| Submit Timesheet | Submit recorded working hours for review |
| Validate Timesheet | Check whether the submitted timesheet is valid |
| Review Timesheet | Allow the engineering manager to examine the submitted timesheet |
| Approve Timesheet | Approve a timesheet after review |
| Reject Timesheet | Reject a timesheet that does not satisfy the required conditions |
| Calculate Project Budget Consumption | Calculate the amount of project budget consumed |
| View Budget Burn | Display current project budget consumption or burn information |

## System Workflow

**Timesheet workflow**

~~~text
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
~~~

**Budget monitoring workflow**

~~~text
Project Data
      |
      v
Calculate Project Budget Consumption
      |
      v
View Budget Burn
~~~

## Requirements Engineering

### Functional Requirements

- The system shall allow a remote developer to log working time.
- The system shall allow a remote developer to submit a timesheet.
- The system shall validate submitted timesheet information.
- The system shall allow an engineering manager to review submitted timesheets.
- The system shall allow an engineering manager to approve a timesheet.
- The system shall allow an engineering manager to reject a timesheet.
- The system shall calculate project budget consumption.
- The system shall allow the engineering manager to view budget burn information.

### Non-Functional Requirements

Categories considered: Performance, Security, Usability, Reliability, Maintainability.

- The system should respond to normal requests within the defined response time.
- Protected functions should only be accessible to authorized users.
- Timesheet information should be stored securely.
- The interface should be simple and easy to use.
- Timesheet and budget information should remain consistent.

### Requirements Traceability Matrix

The RTM links requirements to use cases and test cases.

~~~text
Requirement -> Use Case -> Test Case

FR - Submit Timesheet
        |
        v
UC - Submit Timesheet
        |
        v
TC - Submit Timesheet Successfully
~~~

The complete RTM is in the `01_RE` folder.

## Architecture and Design

The system is organized into separate layers for the user interface, application logic, and data management, to keep it easy to understand, develop, test, and maintain.

Documentation includes:

- Architecture Diagram
- Architecture Pattern
- Component Diagram
- UML Use Case Diagram
- Sequence Diagrams
- API Design
- Error Handling Design

## Software Requirements Specification

The SRS (in `04_SRS_WBS`) contains: Introduction, Problem Statement, Objectives, Scope, Actors, Functional Requirements, Non-Functional Requirements, Security Requirements, Use Cases, Constraints, and Assumptions.

## Work Breakdown Structure

~~~text
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
~~~

The detailed WBS is in `04_SRS_WBS`.

## Project Creation and Management Evidence

Screenshots are kept in `03_Project_Creation`.

**GitHub:** repository creation, repository structure, commits, branches (if used), project activity.

**Jira:** Jira project, backlog, scrum board, sprint, tasks/issues, task status.

## GitHub Copilot

Included as evidence of AI-assisted development (folder `05_GitHub_Copilot`):

- Screenshots of Copilot in use
- Generated or suggested project code
- Evidence of reviewing or modifying the generated code
- Repository or project link related to the work

## Software Testing Tools and Bug Fixing

Demonstrates the full bug-fixing process:

~~~text
Bug Found -> Test Fails -> AI / Copilot Assistance -> Code Fix / Patch -> Retest -> Test Passes
~~~

The `06_Software_Testing_Tools` folder holds evidence of:

1. The bug before fixing
2. The failing test or incorrect behavior
3. AI/Copilot assistance used for the fix
4. The code patch or corrected implementation
5. Retesting after the fix
6. The final test result

## Testing

Testing is based on the system requirements.

**Functional testing:** logging time, submitting, validating, reviewing, approving and rejecting timesheets, calculating budget consumption, viewing budget burn.

**Non-functional testing:** performance, security, usability, reliability, maintainability.

**Bug fixing and retesting:** a selected defect is tested before and after the fix, from identification through successful retesting.

## Scope

**In scope**

- Time logging
- Timesheet submission, validation, review, approval, and rejection
- Project budget consumption calculation
- Budget burn viewing

**External system**

- Jira System

Any features added later will be documented in the SRS and related design documents.

## Repository Structure

~~~text
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
~~~

## Tools and Technologies

- GitHub, GitHub Copilot, Git
- Jira
- Frontend, backend, and database technologies

The final technology list will be updated to match the actual implementation.

## Project Status

Currently being developed and documented as an individual Software Engineering project. The repository is maintained with requirements documentation, architecture and design, SRS, WBS, GitHub and Jira evidence, Copilot evidence, and software testing, bug-fixing, and retesting evidence. It will be updated as development and testing progress.

## Conclusion

The system provides a structured workflow for recording working hours, submitting and validating timesheets, and handling approval or rejection, along with project budget monitoring through consumption calculation and budget burn viewing. The repository is organized to hold the required Requirements Engineering, Architectural Diagram, Project Creation evidence, SRS and WBS, GitHub Copilot evidence, and Software Testing Tools activities.
