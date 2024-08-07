
# Kubernetes Cluster Setup and Autoscaling Project

## Overview

This project demonstrates the setup of a Kubernetes cluster and showcases the deployment and management of a sample application. Key features include automated scaling, resource management, and load balancing, reflecting real-world Kubernetes use cases.

## Achievements

1. **Cluster Setup**

   - **Kubernetes Cluster**: Successfully set up a Kubernetes cluster using `kops`, with one master node and two worker nodes, simulating a production-like environment.
   - **Tools Installed**: Configured essential tools including `kops` and `kubectl`.
   - **Backup Configuration**: Implemented an S3 bucket for backup and exported the cluster state to S3, ensuring reliable recovery and management.

2. **Deployment**

   - **Application Deployment**: Deployed a sample application using a deployment file with one replica. Managed the deployment with selectors and labels.
   - **Resource Management**: Configured resource quotas to regulate resource usage, ensuring efficient operation within the cluster.

3. **Service Exposure**

   - **Load Balancing**: Created a service file to expose the application through a LoadBalancer, providing external access and ensuring high availability.

4. **Autoscaling**

   - **Horizontal Pod Autoscaler (HPA)**: Implemented an HPA to automatically adjust the number of replicas based on CPU utilization. Set target scaling at 50% average CPU utilization, with a minimum of 1 replica and a maximum of 5 replicas.
   - **Stress Testing**: Conducted stress testing to verify Kubernetes’ ability to scale the application automatically in response to increased load.

## Real-World Relevance

This project reflects real-world Kubernetes practices by simulating a production environment where scalability, resource management, and high availability are critical. The setup mimics scenarios encountered in cloud-native applications, including:

- **Cluster Management**: Similar to setting up production clusters with automated backups and reliable recovery.
- **Resource Optimization**: Demonstrates effective resource management and quota enforcement, which are crucial in managing application performance and cost in real-world deployments.
- **Load Balancing and Scaling**: Highlights the importance of load balancing and autoscaling in handling varying loads and maintaining application availability, reflecting real-world needs for dynamic scaling and reliability.

By achieving these goals, this project provides a solid foundation in Kubernetes that is directly applicable to managing and scaling applications in a real-world cloud-native environment.

