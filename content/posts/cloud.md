---
title: "Cloud Computing"
date: 2023-04-30
showToc: false
TocOpen: false
draft: false
weight: 4
hidemeta: false
comments: false
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: true
hideSummary: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowWordCount: true
ShowRssButtonInSectionTermList: false
UseHugoToc: false
ShowPostNavLinks: false
---

## What is cloud computing

Cloud computing refers to the delivery of computing services over the internet, including servers, storage, databases, networking, software, analytics, and intelligence.

{{< youtube i9x0UO8MY0g >}}

---

## Cloud Computing Models

- Infrastructure as a Service (IaaS)
- Platform as a Service (PaaS)
- Software as a Service (SaaS
- Function as a Service (FaaS)

---

## What are Cloud Native Applications?

Cloud native applications are applications that are built and designed to leverage cloud computing frameworks. They are developed with modern methodologies to provide flexibility, efficiency, and robustness in the cloud environment. These applications are rapidly becoming the new normal in the world of software development due to their numerous advantages.

## Key Features of Cloud Native Applications

- **Microservices Architecture**: This allows developers to break down applications into smaller, manageable services that can function independently.

- **Containerization**: Cloud native applications often use containers for deployment. Containers bundle up the code and its dependencies so the application runs quickly and reliably from one computing environment to another.

- **Continuous Delivery**: Cloud native applications support the principles of continuous integration and continuous delivery, making it easier to adapt to changes.

- **Scalability**: These applications can automatically scale up and down depending on the need, thus optimizing resources and reducing costs.

- **Resiliency**: Cloud native applications are designed to anticipate failure. They can quickly recover from any failure, ensuring a higher level of service availability.

## FAQs

1. **What is the difference between cloud-based and cloud-native applications?**

   Cloud-based applications are only hosted on a cloud infrastructure. However, cloud-native applications are not only hosted on the cloud but also specifically designed to leverage the cloud's unique properties.

2. **Why should my business consider moving to cloud-native applications?**

   Cloud-native applications provide numerous benefits such as faster time to market, improved scalability, and reduced operational costs. These attributes make them an excellent choice for businesses looking to stay competitive in today's digital landscape.

3. **What skills are needed to develop cloud-native applications?**

   Developers need a strong understanding of cloud computing concepts, experience with microservices architecture, knowledge of container technologies like Docker and Kubernetes, and familiarity with DevOps practices.

4. **What skills are the most valuable for cloud computing**

   My answer the this questions would be Cloud-native development - since more and more applications are being developed specifically for the cloud, cloud engineers will need to have a deep understanding of cloud-native development frameworks and tools, such as Kubernetes, Docker, and serverless computing.

## When and when not to use FaaS

Faas is great because it can save you money as you dont have to always have your servers turned on, but at the same time there are times when you need a persistent state that these functions are not meant to be good with.

First lets look at what exactly is FaaS

Function-as-a-Service (FaaS) is a specific kind of cloud service that lets you run individual functions or blocks of code in response to events, such as HTTP requests or file changes. These functions are typically small, focused tasks like processing an image, handling an API request, or reacting to a database change. You don't manage any servers; you just deploy your function, and the cloud provider takes care of running it when triggered.

Examples of FaaS:
AWS Lambda
Azure Functions
Google Cloud Functions

Why Use FaaS?
Simplicity: You focus solely on your code and don't worry about infrastructure.
Cost-Efficiency: You pay only for the compute time your function takes.
Scalability: Automatically scales with the number of requests.

A persistent environment or always-on infrastructure is needed when you have services that need to be continuously running and can't be initiated or terminated on-demand. This contrasts with FaaS where functions are stateless, short-lived, and initiated based on events.

Why Do You Need a Persistent Environment?

Stateful Applications: Some applications need to maintain state between different sessions or operations, which might require databases or caching services that are always online.
Low Latency: Always-on services can offer quicker response times compared to event-driven, serverless functions, which may need to "warm up."
Resource-Intensive Operations: Long-running data computations, batch processing, or real-time streaming can't be easily broken down into short-lived, stateless tasks.
Complex Networking: Applications with intricate networking rules or those needing a VPN, private network, or dedicated IP often require always-on infrastructure.

## When to Use and When Not to Use FaaS

Function-as-a-Service (FaaS) is a cost-efficient and scalable solution for executing specific tasks or functions in a cloud-based environment. While it offers various advantages, it's essential to understand its limitations, especially when it comes to persistent state requirements.

### What Exactly is FaaS?

FaaS, short for Function-as-a-Service, is a category of cloud computing services that allows you to run functions in response to specified events. These triggers could range from HTTP requests to changes in a database. The function usually perform highly focused tasks such as image processing, API request handling, or database modifications. The beauty of FaaS lies in its serverless architecture—you deploy your function, and the cloud provider takes responsibility for its execution when triggered.

#### Examples of FaaS Providers:

- AWS Lambda
- Azure Functions
- Google Cloud Functions

### The Need for a Persistent Environment

FaaS is not suitable for all use cases though (for example. situations that may require an always-on infrastructure). Below are some scenarios where a persistent environment is more appropriate:

1. **Stateful Applications**: Applications that must maintain state between different user sessions or operations often rely on databases or caching services that need to remain online continuously.

2. **Low Latency Requirements**: Always-on services can deliver faster response times, avoiding the "warm-up" time sometimes needed by serverless functions.

3. **Resource-Intensive Operations**: Tasks involving long data processing, batch jobs, or streaming are challenging to put into a into short-lived, stateless functions.

4. **Complex Networking**: If your application requires specialized networking configurations, such as a VPN, a private network, or a dedicated IP, a persistent environment is more suitable.
