---
title: "Part 25: EFS – Elastic File System 🌐📁"
seoTitle: "Part 25: EFS – Elastic File System 🌐📁"
seoDescription: "Part 25: EFS – Elastic File System 🌐📁"
datePublished: Thu Jan 11 2024 18:25:49 GMT+0000 (Coordinated Universal Time)
cuid: clr9jip5l000208l30xqva3at
slug: part-25-efs-elastic-file-system
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1704997488118/23558b63-29ed-42ad-9861-c35f8c16c5ff.png
tags: cloud, aws, cloud-computing, devops, 90daysofdevops

---

## **Amazon EFS - A Glimpse into Elastic File Harmony 🚀🔍**

### **1\. EFS Essentials 🌐🔄**

* **NFS Marvel:**
    
    * Managed NFS (Network File System) compatible with multiple EC2 instances.
        
    * Multitude of EC2 instances across multi-AZ for enhanced availability.
        
    * Offers high availability, scalability, with costs 3x that of gp2 (EBS).
        

### **2\. Architectural View 🏰🚀**

* **Multi-AZ Ecosystem:**
    
    * Presence across us-east-1a, us-east-1b, us-east-1c.
        
    * EC2 instances harmoniously interacting with EFS.
        

## **Navigating EFS Use Cases and Protocol 🚀🎭**

### **1\. Versatility in Use Cases 🌐💡**

* **Adaptable Scenarios:**
    
    * Optimal for content management, web serving, data sharing, and WordPress.
        
* **Protocol Harmony:**
    
    * Leveraging NFSv4.1 protocol.
        
    * Integration with security groups for EFS access control.
        

### **2\. Key Features and Characteristics 🌟🔐**

* **Linux Compatibility:**
    
    * Primarily compatible with Linux-based AMIs (Not Windows).
        
    * Data encryption at rest fortified by KMS.
        
    * Adheres to POSIX file system standards.
        
    * Dynamic scalability, pay-per-use, eliminating the need for capacity planning.
        

## **EFS Performance Unveiled 🚀📈**

### **1\. Performance Dynamics 🔄🚀**

* **Scaling Horizons:**
    
    * Accommodates thousands of concurrent NFS clients.
        
    * Achieves throughput exceeding 10 GB/s.
        
* **Performance Modes:**
    
    * **General Purpose:**
        
        * Suited for latency-sensitive tasks like web servers and CMS.
            
    * **Max I/O:**
        
        * Catering to high-latency, high-throughput, and parallel workloads.
            
* **Throughput Modes:**
    
    * **Bursting:**
        
        * 1 TB provides 50 MiB/s with bursts up to 100 MiB/s.
            
    * **Provisioned:**
        
        * Settable throughput, irrespective of storage size (e.g., 1 GiB/s for 1 TB).
            
    * **Elastic:**
        
        * Auto-scales throughput based on workload demands, reaching up to 3 GiB/s for reads and 1 GiB/s for writes.
            

## **EFS Storage Classes - Architecting Efficiency 🚀🗃️**

### **1\. Storage Class Spectrum 🌈🗄️**

* **Lifecycles at Play:**
    
    * Storage tiers governed by lifecycle management (file movement after N days).
        
* **Standard vs. Infrequent Access (IA):**
    
    * **Standard:**
        
        * Tailored for frequently accessed files.
            
    * **Infrequent Access (IA):**
        
        * Cost-efficient for storing with lower retrieval costs.
            
        * Activate EFS-IA via Lifecycle Policy.
            

## **EFS vs. EBS - A Comparative Odyssey 🔄🔍**

### **1\. Elastic Block Storage (EBS) Insights 📊💽**

* **EBS Volumes:**
    
    * Exclusive attachment to one instance (excluding multi-attach io1/io2).
        
    * Locked at the Availability Zone (AZ) level.
        
    * gp2: IO scales with disk size; gp3 & io1 can independently increase IO.
        
* **AZ Migration Tactics:**
    
    * To migrate EBS across AZs: Snapshot creation followed by restoration.
        
* **EBS vs. EFS Dynamics:**
    
    * EBS for single-instance scenarios; EFS for multi-instance ecosystems.
        
    * EFS tailored for Linux instances leveraging NFS.
        
    * EFS boasts higher pricing, alleviated by EFS-IA for cost efficiency.
        

📚 Elevate your understanding: EFS vs. EBS vs. Instance Store—where each piece fits in the AWS puzzle. Explore the file system intricacies, and architect your storage strategy with wisdom. 🚀🔗