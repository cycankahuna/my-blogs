---
title: "Part 23: Load Balancing in Plain English"
datePublished: Thu Jan 11 2024 18:05:49 GMT+0000 (Coordinated Universal Time)
cuid: clr9isyue000009i7gtkbbzqk
slug: part-23-load-balancing-in-plain-english
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1704996095155/bebb3e2b-292d-4264-ae51-2bcda9425c8b.png
tags: cloud, aws, cloud-computing, devops, 90daysofdevops

---

## **Introduction 🚀**

Navigating the intricacies of Load Balancing can be a bit like orchestrating a grand symphony with multiple musicians (servers) playing in harmony. In this non-tech guide, we'll decipher the wonders of Elastic Load Balancers, demystify health checks, and explore the various types of load balancers available in the AWS cloud – all in plain English!

## **Load Balancing: A Brief Overview 🔄🚢**

Load Balancers are like maestros for servers, distributing the incoming traffic among multiple downstream servers (think EC2 instances). But why use them?

* **Spread the Load:** Imagine a traffic cop directing cars to multiple lanes, ensuring smooth flow.
    
* **Single Point of Access:** Load Balancers offer a central entry point (DNS) to your application, simplifying access.
    
* **Handle Failures Gracefully:** Like a safety net, Load Balancers seamlessly manage failures of downstream instances, ensuring uninterrupted service.
    
* **Health Checks:** Regular health checks are performed to ensure servers are ready to respond to requests.
    
* **SSL Termination:** Load Balancers can handle the encryption and decryption (HTTPS) for your websites.
    
* **Stickiness with Cookies:** Think of it as your favorite café remembering your favorite table.
    
* **High Availability:** Load Balancers ensure your application stays afloat even if one server encounters stormy weather.
    

## **Elastic Load Balancer: The Maestro of Load Balancers 🎻🚢**

Why choose an Elastic Load Balancer (ELB)?

* **Managed Convenience:** ELB is a managed load balancer; AWS takes care of upgrades, maintenance, and high availability, minimizing your effort.
    
* **Integration Magic:** It seamlessly integrates with various AWS services like EC2, Auto Scaling Groups, ECS, Certificate Manager, CloudWatch, Route 53, WAF, and Global Accelerator.
    

## **The Heartbeat: Health Checks 💓🔍**

Health Checks are the pulse of Load Balancers. They ensure the servers are fit and ready to handle requests.

* **Critical Checks:** Load Balancers regularly inquire about the health of instances on a specific port and route.
    
* **Unhealthy Instances:** If an instance fails to respond with a healthy status (200 OK), it's considered unfit.
    

## **Types of Load Balancers on AWS 🔄🌐**

AWS offers four types of managed Load Balancers. Let's glance at them:

1. **Classic Load Balancer (CLB):** The old guard, supporting TCP, HTTP, HTTPS, and SSL.
    
2. **Application Load Balancer (ALB):** The modern maestro for Layer 7 (HTTP) applications, perfect for microservices and containers.
    
3. **Network Load Balancer (NLB):** Swift and efficient for handling extreme TCP and UDP traffic.
    
4. **Gateway Load Balancer:** A multitasker operating at Layer 3, handling transparent network gateways, load balancing, and more.
    

## **Security in Harmony: Load Balancer Security Groups 🛡️🚢**

Load Balancer Security Groups act like vigilant bouncers, controlling the traffic flow.

* **Restricted Access:** Limiting access to the Load Balancer ensures a secure environment.
    
* **Secure Communication:** Load Balancers ensure secure communication between users and applications.
    

## **Conclusion 🎉**

In this symphony of server orchestration, Load Balancers play a pivotal role in harmonizing traffic, ensuring the reliability and availability of your applications. So, whether you're managing a bustling website or orchestrating a cloud-based extravaganza, Load Balancers keep the show running smoothly! 🌟🚀