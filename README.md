# IBM-Back-End-Development-Professional-Certificate

## SDLC 
- SDLC is a systematic process to develop a software

- Phases of SDLC

<img width="323" alt="Screenshot 2024-02-14 at 9 05 31 AM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/dc8a892f-a5ad-4a15-a9dd-00f5a0be22b0">

- Phase 1: Planning
  - When planning a software solution, the following factors must be considered: users of the solution the overall purpose of the solution, data inputs and outputs, legal and regulatory compliance, risk identification, quality assurance requirements, allocation of human and financial resources, and project scheduling.
  - All the factors should be documented in a file called SRS (Software Requirements Specification).

<img width="634" alt="Screenshot 2024-02-15 at 6 15 57 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/b9a9a93c-4d65-4de1-bddc-1cacbff94851">

- Phrase 2: Design
  - Requirements are gathered from the SRS to develop architecture and documented into a design document, which will be used to assign the coding tasks.

- Phrase 3: Development
  - This is where the developers start the coding process once the design document is completed.

- Phrase 4: Testing
  - Once the coding is completed. Code is tested to ensure stability, security and that it meets requirements from the SRS.
  - Bugs reported, tracked, fixed, and retested until the software is stable.
  - There are four types of testing:
    - Unit Testing
    - Integration Testing
    - System Testing
    - User Acceptance Testing (UAT)
   
- Phrase 5: Deployment
  - Used for making software available on a website, mobile device app store , or a software distribution server on a corporate network
 
<img width="641" alt="Screenshot 2024-02-15 at 6 25 24 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/6154c594-7392-4e2d-b715-b561aa382253">

- Phrase 6: Maintenance
  - The maintenance phase happens once the code has been deployed into a production environment. This phase helps to find any other bugs, identify user interface issues, or UI for short, and identify other requirements that may not have been listed in the SRS.
  - If bugs are discovered in this phase that were missed during testing, these errors may need to be fixed for high-priority issues or incorporated into the requirements as part of a future software release and the process can start over again.

<img width="632" alt="Screenshot 2024-02-15 at 6 28 24 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/2101eff9-ec39-44a2-a509-557641c9373e">

## Bulding Quality Software 
- Common software engineering processes
  - Requirements gathering: It may include a set of use cases, user flows that the software must implement. Software requirements can be classified into four broad categories (functional, external & user interface, non-functional, system features)
  - Design: Transforming requirements into code, application logic.
  - Coding for quality: Refers to the characteristics of the code including attributes such as maintainability, readability, testability, and security.
  - Testing: The process of verifying that the software matches established requirements and is free of bugs
    - Unit testing: often done by the developer and tests the smallest component of code
    - Integration test: occured when the components are integrated into the larger product
    - System testing: After the larger product is deemed (gần như) completed
    - UAT (beta testing): The software is tested by the intended end user. 
  - Releases
  - Documenting
    - System documentation: README files, inline comments, architecture and design documents, verification information and maintenance guides
    - User documentation: User guides, instructional videos, manuals, online and inline help

## Requirements
- Requirements documentation:
  - SRS:
    - Captures functionalities the software should perform
    - Establishes benchmarks / service-levels for performance
    - Purpose and scope (Who has access to the SRS, how it should be used, software benefit)
    - Constraints, assumptions, dependencies (how the software must operate under given conditions, required OS or hardware, other software products)
    - Requirements (function of the software, users and interactions with other hardware or software, functions of the system, performance, safety, security, quality)
  - URS (User requirements specification)
    - Describe business need and end-user expectations
    - Confirmed during UAT
    - Oftern covered in SRS
  - SysRS (System requirements specification)
    - Broader than an SRS
    - Contains: (System capabilities, Interfaces, Policy, Regulation, Personnel, Performance, Security, System acceptance criteria, Hardware expectations

## Common development methodologies
- A process is needed to clarify where and when communication and facilitate information sharing among team members
- Sequential methodologies:
  - Waterfall method: output of the previous step is the input of the next step
  
<img width="652" alt="Screenshot 2024-02-15 at 9 43 14 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/fa465219-f5c3-46ab-a350-0fefada220fe">

  - V-shape model:
    - The phases going down the left side of the V are called “verification". Then, going up the right side of the V, those phases are called, "validation."
    - The tests are written during the verification phases on the left and executed during the validation stages on the right.
  
<img width="687" alt="Screenshot 2024-02-15 at 9 47 00 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/e7047095-06ad-4be9-8d55-dd07e238722c">

- Iterative:
  - Agile: Rather than the “maintenance” stage of the SDLC, the final stage of the sprint is a feedback stage. At the end of each sprint, a chunk of working code is released at a meeting called the “sprint demo” where stakeholders can see the new functionality and provide feedback. After the sprint demo, the entire process is repeated for every sprint cycle.
 
<img width="664" alt="Screenshot 2024-02-16 at 11 42 24 AM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/d216cd1a-0b5b-45fd-8a2d-aeaecc4d708e">

## Back-end development 
- APIs, Routes, and Endpoints process requests from the front-end
  - API is a code that works with data
  - Route is a path to a website or page
  - Endpoint can be an API or route
- Back-end developers create routes to direct requests to the correct service
- APIs provide a way for cloud apps to access resources from the back-end 

## Software architecture and design
- Software architecture is the organization of the system
- Software architecture list all components and elements that the software must implement
- Comprised of fundamental structures and behaviors
- Software architecture guides technology stack choice
- Technology stacks include:
  - software
  - Programming language
  - Libraries
  - Frameworks

- Architecture drives production environment choices
- Production environment is the infrastructure that runs and delivers the software such as:
  - Servers
  - Load Balancers
  - Databases
 
## Software Design and modeling 
- Software design is the process to document structural components and behavioral attributes
- Models express software design using:
  - Diagrams and flowcharts
  - UML (Unified modeling language)

- Structured design breaks down a software problem into well-organized solution elements
- Structural diagram has modules and sub-modules
- Behavioral models describe the behavior of a system

<img width="622" alt="Screenshot 2024-02-17 at 5 17 00 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/44e925c1-44d9-43f8-bea5-7969452b55e4">

- Peer-to-peer: An architecture consists of nodes that behave both as client and as server

<img width="394" alt="Screenshot 2024-02-17 at 5 25 07 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/35de6eec-789a-402e-9e09-7598217bd256">

- Microservices: An architecture has applications composed of several loosely coupled services that communicate using APIs

<img width="452" alt="Screenshot 2024-02-17 at 5 24 55 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/aa61f56f-933f-4648-9498-5d7c42c1eb44">

- Event-driven: An architecture has consumers that send requests to producers

<img width="438" alt="Screenshot 2024-02-17 at 5 25 32 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/7f4e852d-de2a-4c68-a474-82a1f5db5a46">

- Two-tier: An architecture has clients that communicate with a server

<img width="341" alt="Screenshot 2024-02-17 at 5 25 19 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/3caeb35b-e88c-4b3b-83ce-98c51c5bc641">

- Three-tier: An architecture consists of three-tiers (presentation, application, and data)

<img width="279" alt="Screenshot 2024-02-17 at 5 25 45 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/40184891-7bde-44dc-9797-cf3c377703fa">

