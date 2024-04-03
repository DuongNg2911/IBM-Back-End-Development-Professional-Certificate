## Azure Virtual Machines
- What is Azure Virtual Network
  - Azure Virtual Network is a service that provides the fundamental building block for your private network in Azure which enables many types of resources to securely communicate with each other, the internet, and on-premises networks. These Azure resources include virtual machines (VMs). For example, you have 2 virtual machines, one hosting a web application, and one hosting the database, they can communicate with each other in a securely environment inside a virtual network. 

<img width="639" alt="Screenshot 2024-04-03 at 1 24 23 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/fefb68b2-2f0c-4531-b243-31db3f4b2be3">

  - You can also create a subnet, which means generate a virtual network for each virtual machine for better security. For example, you have 2 virtual machines, one hosting a web application, and one hosting the database, they can communicate with each other in the same virtual network but it only allows public internet traffic to access web application server without accessing database server. 

<img width="1380" alt="Screenshot 2024-04-03 at 1 31 29 PM" src="https://github.com/DuongNg2911/IBM-Back-End-Development-Professional-Certificate/assets/127082369/9bb99de4-0795-40db-aa44-0e7089bb7f01">

## Azure Deployment Options 
- SQL Server on Azure Virtual Machines
  - Tương đồng với infrastructure as a service (IaaS).
  - Với IaaS, bạn có thể:
    - Cập nhật và sửa đổi OS và SQL server.
    - Bao gồm các tính năng quản lý tự động cho SQL server 
   
- Azure SQL platform, Azure SQL managed instance, Azure SQL database
  - Tương đồng với (PaaS).
  - Với PaaS, bạn có thể:
    - Quản lý hoàn toàn hệ thống cơ sở dữ liệu. Những hệ thống dữ liệu này sẽ tự động hoá các hàm trong cơ sở dữ liệu

  - SQL Managed Instance: 
    - Người dùng không thể truy cập hay sửa đổi OS và SQL server. Tuy nhiên nếu người dùng muốn sử dụng các tính năng instance-scoped liên quan đến SQL server ví dụ như (SQL Server Agent, Service Broker, common language runtime (CLR), Database Mail, linked servers, distributed transactions (preview), and Machine Learning Services). thì nên sử dụng phương án này.
   
  - SQL Database:
    - Người dùng không thể truy cập hay sửa đổi OS và SQL server.
    - Đây cũng là phương án triển khai duy nhất khi mà người dùng yêu cầu nơi lưu trữ cơ sở dữ liệu không giới hạn (hyperscale) và (autoscaling) khi không kiểm soát được khối lượng công việc (serverless)

  - Elastic database pool:
    - Chỉ áp dụng với (SQL database và SQL managed instance)
    - Cho phép bạn chia sẻ tài nguyên cho các instances và databases khác.
    - Sử dụng (SQL database elastic pool) cho (SaaS) khi nó yêu cầu nhiều cơ sở dữ liệu.
     - 
- Điểm khác biệt chính giữ IaaS và PaaS là "versionless" SQL. Trong khi IaaS phải gắn với một phiên bản SQL server nhất định, thì PaaS cho phép Microsoft Azure được cập nhật liên tục các phiên bản của cơ sở dữ liệu SQL
