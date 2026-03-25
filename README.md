# AWS Tutorial

## Virtual Machine

- Uses **hypervisor** to run full, separate operating systems.

## Amazon Elastic Compute Cloud (Amazon EC2)

- Virtual machines.
- **Unmanaged service**: Provides full control over virtual machines.
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

## AWS Identity and Access Management (IAM)

- Manage roles and permissions.

---

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
- **ECS Launch Types**:
  1. **ECS with EC2**: Small-to-medium businesses needing full control over infrastructure or specific hardware/networking.
  2. **ECS with Fargate**: For startups or small teams; serverless, auto-scaling, and orchestration for variable traffic.

#### Amazon Elastic Kubernetes Service (Amazon EKS)

- Fully managed service for running **Kubernetes** on AWS.
- Open-source platform; provides more control and flexibility for large-scale or hybrid deployments.
- **EKS Launch Types**:
  1. **EKS with EC2**: Best for enterprises needing full infrastructure control and Kubernetes scalability.
  2. **EKS with Fargate**: Kubernetes flexibility without managing servers; serverless simplicity.

#### Amazon Elastic Container Registry (Amazon ECR)

- Fully managed Docker container registry for storing container images.

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

## Orchestration Tools

- **AWS Elastic Beanstalk**
