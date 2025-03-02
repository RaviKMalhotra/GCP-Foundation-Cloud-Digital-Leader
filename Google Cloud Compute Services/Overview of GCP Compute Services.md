![image](https://github.com/user-attachments/assets/11c72803-3594-40b4-be92-24800eb25465)
- Author: Ravi K Malhotra
- ravikmalhotra.com                                           

# Overview of Google Cloud Compute Services
These are the compute services available in the GCP cloud:
- Compute services are the most critical and highly used components in any cloud platform.
- Compute instances are also referred as workloads, as you can host any website or any custom application on top of a compute instances.
- Compute instance, simply means a virtual machine in Microsoft Azure Cloud and EC2 instance in AWS cloud.
- GCP offers a wide range of compute services. Here is a list
    - GCP Compute Engine
    - GCP App Engine
    - GCP Kubernetes Engine
    - GCP Cloud Run
    - GCP Cloud Run Functions
    - GCP Bare Metal
   -   
## 1. App Engine

### These are the Key Features of an App Engine:
✅ Fully managed runtime environments (Python, Java, Go, Node.js, PHP, Ruby, etc.).
✅ Automatic scaling & load balancing.
✅ Integrated monitoring with Cloud Logging & Trace.
✅ Traffic Splitting (A/B testing for different versions).
✅ Built-in security & compliance.

## 2. Compute Engine

- Compute Engine is an Infrastructure as a Service (IaaS) offering that provides scalable virtual machines (VMs) on Google's infrastructure.
- Compute Engine was launched in year 2012
- It supports both Windows and Linux operating systems.
- you can create compute engine using the GCP console, and CLI. 
- It offers various machine types to suit different workloads.
- As this being an IaaS offerings, users or consumers have full control over VM configurations, including CPU, memory and storage options.
#### Primary use cases of Compute Engine: Web hosting, databases, big data processing, and enterprise applications.
 
### These are the Key Features of Compute Engine:
✅ Fully customizable VMs (CPU, RAM, disk, and GPU).

✅ Preemptible and Spot VMs (cost-saving for non-critical workloads).

✅ Live Migration (keeps VMs running during maintenance).

✅ Autoscaling & Load Balancing (optimizes performance).

✅ Confidential Computing (encrypts data in use).


## 3. Google Kubernetes Engine (GKE) (Managed Kubernetes)
- GKE is a managed Kubernetes service that simplifies deploying, managing, and scaling containerized applications using Google's infrastructure. 
- It offers automated operations, integrated security, and enterprise-grade support.
- Kubernetes Engine was launched and introduced by Google in year 2015. 

#### Primary use cases of Google Kubernetes Engine: Microservices, hybrid/multi-cloud applictions, and container orchestration.

### Key Features of Google Kubernetes Engine:
✅ Auto-scaling (automatically adjusts compute resources).
✅ GKE Autopilot (fully managed mode where Google handles cluster operations).
✅ Multi-cluster & Multi-region support.
✅ Built-in security features (IAM, encryption, and vulnerability scanning).
✅ Hybrid and Multi-cloud Support (via Anthos).

## 4. Cloud Functions (FaaS - Event-driven serverless

### Key Features of Cloud Functions (FaaS)
✅ Fully serverless (only pay for execution time).

✅ Triggers from GCP services (Cloud Storage, Pub/Sub, Firestore, etc.).

✅ Autoscaling from 0 to N requests.

✅ Built-in security & monitoring.

✅ Supports multiple runtimes (Node.js, Python, Go, Java, .NET, Ruby, PHP).

## 4. Cloud Run

### Key Features of Cloud Functions (FaaS)

✅ Deploy any containerized app (supports Docker & OCI-compliant containers).

✅ Scales to zero when idle (cost savings).

✅ Fully managed or Anthos-managed (for hybrid/multi-cloud).

✅ Supports HTTP-based workloads & WebSockets.

✅ Integrated with GCP IAM & Cloud Logging.

## 5. Cloud Run Functions
## 6. Bare Metal Solution


