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
    - Explicitly declare all dependencies

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
