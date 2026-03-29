# AWS Tutorial

## AWS Regions

## AWS Availability Zones (AZs)

## Virtual Machine

- Uses **hypervisor** to run full, separate operating systems.

## Amazon Elastic Compute Cloud (Amazon EC2)

- Virtual machines
- Unmanaged Service: - Provides full control over virtual machines.
- **Customer Responsibility**:
  - Setup
  - Securing
  - OS maintenance
  - Network configurations
  - Applications

## Managed Services

- **Elastic Load Balancing (ELB)**

- **Simple Queue Service (SQS)**

- **Simple Notification Service (SNS)**

## AWS Lambda

- **Serverless**: No access to underlying infrastructure.

## AWS Identity & Access Management (IAM)

- Manage roles and permissions.

## Containers

- Provide a consistent environment to deploy and scale.
- Faster and lighter than Virtual Machines (VMs).

### Docker

- Software platform to build, test, and deploy applications quickly.

### Container Orchestration Services

- Manage the lifecycle of containers.

#### Amazon Elastic Container Service (Amazon ECS)

- Scalable container orchestration service.
- Runs and manages containers; streamlined and integrated.
- Uses a fully managed Docker registry to store container images.
- ECS Launch Types
  1. **ECS with EC2**: Small-to-medium businesses needing full control over infrastructure or specific hardware/networking.
  2. **ECS with Fargate**: For startups or small teams; serverless, auto-scaling, and orchestration for variable traffic.

#### Amazon Elastic Kubernetes Service (Amazon EKS)

- Fully managed service running Kubernetes on AWS.
- Open-source platform; provides more control and flexibility for large-scale or hybrid deployments.
- **EKS Launch Types**:
  1. **EKS with EC2**: Best for enterprises needing full infrastructure control and Kubernetes scalability.
  2. **EKS with Fargate**: Kubernetes flexibility without managing servers; serverless simplicity.

#### Amazon Elastic Container Registry (Amazon ECR)

- Fully managed Docker container registry for storing container images.
- Stores, manages, and deploys Open Container Initiative (OCI)-compliant container images

---

## Two Ways to Run Containers

1. **Amazon EC2**
   - Customer manages the VMs that run containers.
   - Full control, but requires managing underlying infrastructure.
   - container images follow Open Container Initiative (OCI) standards
   - can push, pull, and manage images in your Amazon ECR repositories using standard container tooling and command line interfaces (CLIs)
2. **AWS Fargate**
   - **Serverless**, efficient, and convenient.
   - AWS manages the servers; customer only manages the containers.
   - works with both Amazon ECS and Amazon EKS

---

## Deploying Your Software to the Cloud

1. Configure your application into a container.
2. Upload a container image to **ECR**.
3. Choose an orchestration service (**ECS** or **EKS**).
4. Select a compute option (**EC2** or **Fargate**).

## Additional Compute Services

1. **AWS Elastic Beanstalk**

- simplifed provisioning
- configuration management
- visibility and control
- fully managed service that streamlines the deployment, management, and scaling of web applications.
- automatically handles the provisioning of infrastructure, scaling, load balancing, and application health monitoring.
- supports various programming languages and frameworks, such as Java, .NET, Python, Node.js, Docker, and more.
- provides full control over the underlying AWS resources while automating many operational tasks.
- Good for deploying and managing web applications, RESTful APIs, mobile backend services, and microservices architectures, with automated scaling and simplified infrastructure management

2. **AWS Batch**

- takes care of infrastructure management
- provides parallel processing support
- automatically scales
- fully managed service that you can use to run batch computing workloads on AWS.
- automatically schedules, manages, and scales compute resources for batch jobs, optimizing resource allocation based on job requirements.
- Good for processing large-scale, parallel workloads in areas like scientific computing, financial risk analysis, media transcoding, big data processing, machine learning training, and genomics research

3. **Amazon Lightsail**

- simple
- cost effective
- managed infrastructure
- streamlines web application setup and management without the need for complex infrastructure.
- a cloud service offering virtual private servers (VPSs), storage, databases, and networking at a predictable monthly price.
- ideal for small businesses, basic workloads, and developers seeking a straightforward AWS experience without the complexity of the full AWS Management Console.
- Good for basic web applications, low-traffic websites, development and testing environments, small business websites, blogs, and learning cloud services.

4. **AWS Outposts**

- supports hybrid cloud solutions
- extends AWS services to on-premises environments, supporting hybrid cloud architectures.
- fully managed hybrid cloud solution that extends AWS infrastructure and services to on-premises data centers.
- provides a consistent experience between on premises and the AWS Cloud, offering compute, storage, and networking components.
- Good for low-latency applications, data processing in remote locations, migrating and modernizing legacy applications, and meeting regulatory compliance or data residency requirements
