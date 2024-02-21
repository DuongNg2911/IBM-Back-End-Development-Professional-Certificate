## Twelve-Factor App Methodology

- In morden software development, the software often delivered as a service
- The kind of Software that centrally hosted and accessed through the internet is often called web apps or Software-as-a-service (SaaS)
- Twelve-factor app methodology is suited for web apps
  - Frequently used with microservices

- The twelve factors can be grouped according to the following phrases of the SDLC

<img width="522" alt="Screenshot 2024-02-21 at 12 21 28 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/8b547604-1c5a-41e9-aa17-1c7e06e6dcec">

- Code factors:
  - Factor 1: Codebase
    - Usually track an application in a verion control system (VCS) such as Git
    - Maintain one-to-one relationship between codebase and app
    - Deploy multiple instances of the app
    - Develop different versions of the codebase in each deploy
  - Factor 5: Build, release, run
    - This phrase demonstrates how a codebase becomes a production deployment
    - Build: Compiles the code, gather dependencies and then transforms the codebase into an executable unit called a Build.
    - Release: Combine Build with the deployment's current configuration so that the code is ready to run
    - Run: Run the application
  - Factor 10: Dev/Prod parity
    - Minimizes differences between developments and production environments which reduces the chance the code runs appropriately in one env but not in another
    - Parity means use the same backend services across environments which helps catch failures earlier in the development process
  - Factor 2: Dependencies
    - Explicitly declare all dependencies as it simplifies setup for developers new to the app.

- Deploy factors:
  - Factor 3: Config
    - The configuration is everything that can differ between deployments such as backend service credentials and locations in config
    - Keep seperate from code and store config in environment variables which are easy to change across deployments without changing the code.
  - Factor 4: Backend services
    - Do not disinguish between local and third-party services
    - All services should be accessible via a URL and credentials so that they can be swapped without changing the code. For example, if an existance database experiences problems, a new database can be spun up and substituded without changing code.
  - Factor 6: Processes
    - Processes are launched via the command line (for example, python my_script.py)
    - An app executes in an environment as one or more processes. Processes should be stateless and share nothing
    - You should store persistent data in a backend service like a database since memory and filesystems aren't shared across processs.
    - Data needs to be centrally stored so it can be accessed by all transaction.
  - Factor 7: Port binding
    - HTTP: a protocol that allows transfering information between network devices.
    - A web server should not be injected into an application at runtime
    - The web app should export HTTP and other services by binding to a port and listening to incoming requests on that port
    - Binding a port is generally done in the code by declaring a web server library as a dependency
    - Because these apps are accessible via a URL, they can become a backend service for other app

- Operate factors
  - Factor 8: concurrency
    - An application runs concurrent processes to handle the increasing load and since processes are stateless and share nothing, an application can scale the processes horizontally and handle additional incoming requests without creating interdependencies among processes.
  
<img width="339" alt="Screenshot 2024-02-21 at 1 01 00 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/f3b211ac-c148-481f-bc75-864cf8b7f3d4">

  - Factor 9: Disposability (being not essential or not serious)
    - It specifies that application processes require minimal startup time and should end gracefully when terminated
    - Quick startup allows quickly deploy changes to code or config
    - Easily scale apps because new deploys start quickly.
  - Factor 11: Logs
    - Logs give visibility into application performance so an app should not concern itself with storing logs
    - An application env should handle logs as an event stream with standard output
    - Execution env can capture the log streams for all running apps, aggregate them and route them to their destination

   - Factor 12: Admin processes
     - Admin processes are one-off (thực hiện 1 lần) processes for managing an app such as a database migration
     - Run against a release, using same codebase and config
     - Additionally, the application code should include admin processes so that they remain synchronized with the app 

## What are microservices 

- An approach to create a single application composed of:
  - Many loosely coupled and independently deployable smaller services

- Characteristics of microservices:
  - Each application component (service) have its own technology stack, inclusive (including) of the database and data management model.
  - Microservices components communicate with one another over a combination of REST APIs, event streaming and meassage brokers and they are segregated and organized by business functionality referred to as a bounded context

- Benifits of microservices:
  - Because it is no interdependency between services => update code more easily to add new features or functionality
  - Different service can use different technology stack => varied expertise
  - Smaller components can be scaled independently of one another, reducing the waste and cost associated
 
- Scaling microservices
  - Usually horizontal scalling (adding additional resources such as ram, cpu, gpu)
  - With microservices, individual services can be individually deployed and scaled therefore it require less infrastructure because they enable precise scaling of only the components that require it
  - Can use Event drivent instead of API calls 

## Monolith vs SOA vs Microservices 
- Monolith:
  - Has all or most of its functionality within a single process or server 
  - The application is managed in internal layers or libraries for:
    - Security
    - Reporting
    - Analytics
    - UI
    - Data access
  - The layers are tightly connected and dependent on each other

  - Benefits:
    - It is simple and less cross-cutting of features and functionalities since everything is in the same code base.
  - Drawbacks:
    - The design becomes more complex and difficult to modify
    - Less flexibility to adapt to new technology which mean rewriting the whole application

  <img width="605" alt="Screenshot 2024-02-21 at 1 50 59 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/d3861f6a-dc0a-4f6e-b4a0-350fc09b5433">

- SOA:
  - SOA is designed and built in a service provider and consumer approach
  - Provides services that are:
    - Seamless integration (liền mạch)
    - Reusable
  - Each service should consist of three components:
    - Interface: defines how a service provider will execute requests from a service consumer
    - Contract: defines how the service provider and service consumer should interact
    - Implementation: the service code

  - Benefits of having these three separated components:
    - Increases reliability
    - Support paralell development

  - Drawbacks of having these requirements:
    - An SOA can become complex and obstruct (block) rapid application development
    - Expensive investment

<img width="652" alt="Screenshot 2024-02-21 at 2 19 56 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/0df6c8f9-1060-4bed-ae6e-09eab6990455">

- Microservices:
  - Drawbacks:
    - Security requirement as each service will need its own security paradigm
    - Debugging is a challenge as each service run independently meaning it is more difficult to locate the root cause
  
<img width="648" alt="Screenshot 2024-02-21 at 2 26 32 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/e61ef31a-3d1e-42ff-be75-7c9f04cdedb8">

## Microservices Patterns

- Single page application (SPA)
  - Enabled by more powerful browsers, faster networks and client-side languages
  - The user enters through one interface that never reloads the landing page or navigates away from that initial experience
  - Built with HTML, CSS and JS
  - Respond to user input through dynamic service calls to backend REST-based services that update portions of the screen instead of redirecting to an entirely new page
  - Simplifies the front-end experience with the tradeoff of more responsibility on the backend services
  - It delivers poor results across user experiences through different channels, like mobile and web
  
- Backend for Frontend (BFF)
  - Provides superior support compared to a generic backend
  - It inserts a layer between user experience and the resources which is a backend specifically for the mobile/web application 
  - Enables customized UX for different channels
  - Supports one backend type per user interface
  - For example, the mobile backend will retrieve small amount of data compared with desktop backend due to screen sizes.
  
<img width="666" alt="Screenshot 2024-02-21 at 2 44 20 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/f0297c08-13f7-4925-8160-5bbdfaacf451">

## Strangler pattern 

- Strangler pattern helps manage the refractoring (thay đổi cấu trúc mà không làm thay đổi chức năng và giá trị) of a monolithic application in stages.
- Use the structure of a web application to split an application to functional domains and replace those domains with a new microservices-based implemetation of one domain at a time.
- These two aspects form separate applications that exist side-by-side in the same URL space

<img width="681" alt="Screenshot 2024-02-21 at 2 57 03 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/ca4e4303-f2e3-4026-acdd-178562fb658e">

## Service discovery

- This pattern helps applications and services discover each other which provides flexibility as in Microservices, service instances change dynamically due to scaling, upgrades, service failure, and even service termination
- Could be used by a load balancers to perform health checks and rebalance traffic on service failures

## Microservices Anti-Patterns 

- Rule 1: Don’t build microservices
  - Don't start with microservices
  - When you determine that the monolithic application's complexity negatively affects application development and maintenance, consider refactoring that application into smaller services.
  - When the application becomes too large to update and maintain easily, these microservices will become ideal for breaking down the complexity and making the application more manageable.

- Rule 2: Not taking automation seriously
  - If you have a monolith application, you only need to deploy one piece of software. Once you move to a microservices architecture, you will have more than one application with each having different code, test, and deploy cycles.
  - Attempting to build microservices without either:
    - Proper deployment and monitoring automation, or 
    - Managed cloud services to support your now sprawling (​spreading in an untidy way), heterogenous (diverse in content) infrastructure
  - So, when you are building microservices, always use DevOps or cloud services.

- Rule 3: Don’t build nanoservices
  - If you go too far with the micro in microservices, you could easily find yourself building nanoservices! The complexity of which will outweigh the overall gains of microservices architecture.
  - Lean toward creating larger services and create smaller services when:
    - Deploying changes becomes difficult
    - The common data model becomes overly complex
    - Loading and scaling requirements no longer synchronize and affect application performance  

- Rule 4: Don’t turn into SOA
  - The two concepts; microservices and service-oriented architecture (SOA) are often confused with one another because, at their most basic level, both build reusable individual components that can be consumed by other applications.
  - However, microservices are fine-grained with independent data storage for each, that is, the bounded context.
  - A microservices project that morphs into an SOA project will likely buckle under (Bị ảnh hưởng bởi) its own weight.

- Rule 5: Don’t build a gateway for each service
  - Instead of implementing end-user authentication, throttle, orchestrate, transform, route, and analytics in each service, you should use an API Gateway.
  - An API gateway is an API management tool that sits between a client and your collection of backend services.
  - This will become central to the above-mentioned non-functional concerns and will avoid re-engineering them with each service.
