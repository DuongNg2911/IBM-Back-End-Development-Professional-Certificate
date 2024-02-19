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
    - Establishes benchmarks / service-levels for performance, capacity estimation
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
- It includes a definition of which elements and components need to be in the system, which components need to interact with each other, and what type of environment the software needs to operate. 
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
- Software design happens once the software architecture finished.
- Software design is the process to document structural components and behavioral attributes
- Software design focuses on how the individual modules and components will be designed
- Models express software design using:
  - Diagrams and flowcharts
  - UML (Unified modeling language)

- Structural patterns are design patterns that deal with the composition and organization of classes and objects. They help you define how different components of your system interact and relate to each other. Structural patterns can simplify your code by reducing the number of classes, hiding the complexity of the internal structure, or providing a common interface for different implementations.

- Behavioral patterns are design patterns that deal with the communication and cooperation of classes and objects. They help you define how different components of your system behave and respond to each other. Behavioral patterns can improve your code by enhancing the flexibility, modularity, and reusability of your algorithms, strategies, and commands.

<img width="622" alt="Screenshot 2024-02-17 at 5 17 00 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/44e925c1-44d9-43f8-bea5-7969452b55e4">

## Application architecture
- Component:
  - An individual unit of encapsulated functionality
  - Serves as a part of an application in conjunction with (liên kết với) other components
  - Component characteristics:
    - Reusable: reused in different applications
    - Replacable: easily replaced with another component
    - Independent: doesn't have dependencies on other components
    - Extensible: add behavior without changing other components
    - Encapsulated: doesn't expose its specific implementation
    - Non-context specific: operates in different environments
  - Component examples:

<img width="635" alt="Screenshot 2024-02-18 at 6 23 07 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/7c921d8d-12f9-4fd2-ab88-d33c92fcafdd">

- Component-based architecture
  - Decomposes design into logical components
  - Higher level abstraction than objects
  - Defines, composes, and implements loosly coupled independent components so they work together to create an application

- Services:
  - Also an individual unit of functionality 
  - Designed to be deployed independently and reused by multiple systems
  - Focused on solution to a business need
  - The key difference between services and component is that services has one unique, always running instance with whom multiple clients communicate

- NOTE: A service can be made up of several components and components consist of objects. Usually a service provides one complete feature that is made up by combining different components.

- Services-oriented architecture (SOA):
  - A Loosely coupled services that communicate over a network
  - Support building distributed systems that deliver services to other applications through the communication protocol
  
## Distributed system 
- Even though multiple services located on diffrent machines. They interact with each other via a communication protocol such as HTTP and appears to the end-user as a single coherent system
- Distributed system characteristics:
  - Shares resources: hardware, data, ..
  - Fault-tolerant: if a node or a service fails, the system continues to run without service interruption
  - Mutiple activities run concurrently (at the same time)
  - Scalable as the number of users increases
  - Runs on a variety of computers: The computers running the distributed system do not need to use the same kind of hardware or OS
  - Programmed in a variety of programming languages.

## Architectural patterns
- An architectural pattern is a repeatable solution to a problem in software architecture
- Peer-to-peer: An architecture consists of nodes that behave both as client and as server without using a central server 
  - Example: Cryptocurrency 
<img width="394" alt="Screenshot 2024-02-17 at 5 25 07 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/35de6eec-789a-402e-9e09-7598217bd256">

- Microservices: An architecture has applications composed of several loosely coupled services that communicate using APIs
  - An orchestration handles communication between these services
  - Example: Social Media 
<img width="452" alt="Screenshot 2024-02-17 at 5 24 55 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/aa61f56f-933f-4648-9498-5d7c42c1eb44">

- Event-driven: An architecture has consumers that send requests to producers where ingestion = routing
  - Example: Ride sharing 

<img width="438" alt="Screenshot 2024-02-17 at 5 25 32 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/7f4e852d-de2a-4c68-a474-82a1f5db5a46">

- Two-tier: An architecture has clients that communicate with a server
  - The server hosts, delivers, and manages most of the resources and services delivered to the client
  - Example: Messaging apps
  
<img width="341" alt="Screenshot 2024-02-17 at 5 25 19 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/3caeb35b-e88c-4b3b-83ce-98c51c5bc641">

- Three-tier: An architecture consists of three-tiers (presentation (UI), application (business logic), and data (data storage))
  - Example: Web apps, presentation layer presents UI, application layer processes user inputs and a database server handles data management

<img width="279" alt="Screenshot 2024-02-17 at 5 25 45 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/40184891-7bde-44dc-9797-cf3c377703fa">

- Combining patterns:
  - Some patterns can be combined in a single system while some cannot.
  - Example: 3-tier with microservices, peer-to-peer with event-driven, peer-to-peer cannot combine with two-tier

## Application Deployment Environments
- An application environments is the combination of the hardware and software resources required to run an application
- Including:
  - Application code for its various components or modules
  - Software stack requires for running the application (libraries, apps, middleware, OS)
  - Networking infrastructure
  - Hardware (computing, memory and storage)

- Pre-production environments are those platforms that the application resides on in various forms as it gets prepared for production
  - Common pre-production environments are development, QA, and staging
  - Development: developer's workstation
  - QA: QA team tests the application's components
  - Staging: replicating the production environment but not meant for general users
- Production environment
  - Including the entire solution stack
  - Intended for all users
  - Other non-functional requirements:
    - Security
    - Reliability
    - Scalability
  - More complex than pre-production environments

- Options for deploying application environments
  - On-premises deployment
    - System and infrastructure reside in-house within organization's hardware, often behind a firewall. Firewalls prevent access to or from a private network
    - Offers greater security or control of an application and the data in-use for that application
    - An organization is responsible for the system, hardware related infrastructure and maintenance required to run the application
    - More expensive than cloud deployment
  - Cloud deployment:
    - Public: Shared infrastructure with other companies over internet and hardware owned by the cloud provider. For example, AWS, Microsoft Azure, Google Cloud or IBM Cloud. Most common due to its scalability and cost.
    - Private: Infrastructure is provisioned (cung cấp) for a single organization. The main advantage is it not only increases security but also allows for more flexibility because it can be fully customized.
    - Hybrid: Optimize the advantages of both private and public cloud

## Production Deloyment Components

<img width="660" alt="Screenshot 2024-02-18 at 9 31 49 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/6cc338b8-26cd-4a73-817a-3112917d0035">

- Not necessary have all these components in one infrastructure.
- Firewall:
  - Monitors traffic between an interior and an exterior network
  - Permits or blocks data based on a set of security rules
  - Acts as a barrier between networks to block viruses and hackers from accessing the internal network

- Load balancers:
  - Purpose: distributes traffic efficiently amongst multiple servers
  - Functions:
    - Load balancers are used to prevent server traffic overload and are located between clients
    - Maximizes server capabilities and responsiveness
    - Ensures no one server is overworked
    - Manages concurrent requests fast and reliably 

- Web and application servers
  - Servers:
    - Provide services, resources, data, or applications to a client
    - Store, process, and manage network data, devices, and systems
  - Web servers:
    - Delivers web pages, files, images, and videos to the client
    - Responds to HTTP requests from a web browser
  - App servers:
    - Runs the business logic and provides the app to the client or the web server
    - Its primary job is to enable interaction between the end-user and the server-side application code
    - The application code represents the bussiness logic that determines how data can be created, stored, or changed
  - Proxy server:
    - An intermediate server that sits in between two tiers and handles requests between those tiers
    - A proxy server can be used for load balancing, system optimization, caching, as a firewall, obscuring the source of a request, encrypting messages, scanning for malware, and more
    - Can improve efficiency, privacy, and security of data flowing through a network
  - Databases server:
    - Control the flow and storage of data
