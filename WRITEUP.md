# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
Costs:
    + VM: pay for the VM size, storage, and any additional services use
    + App Service: based on the tier choose (Free, Shared, Basic, Standard, Premium)
Scalability:
    + VM: Scaling manual, need to add more VMs or increase the size of existing ones, which can be complex and time-consuming
    + App Service: Automatically scale
Availability:
    + VM: High availability requires setting up multiple VMs in different availability zones, configuring load balancers, and managing failover. This adds complexity and cost.
    + App Service: Provides built-in high availability. Your app is automatically distributed across multiple instances and data centers, ensuring better uptime and reliability.
Workflow:
    + VM: Have full control over the environment. This can be beneficial for complex applications
    + App Service: Easier deployment. It supports deployment (CI/CD) pipeline, easier to deploy updates.
- *Choose the appropriate solution (VM or App Service) for deploying the app*
    + Both VM and App Service are OK for this application, but I choose App Service
- *Justify your choice*
Environment: Fully manage platform, optimized for hosting web applications, RESTful APIs, and mobile backends with built-in features
High Availability: Simplifies deploying applications across multiple regions for geo-redundancy and disaster recovery.
Workflow: Using Github and deployment (CI/CD) pipeline, easier to deploy updates.
Cost: based on tier plan

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
Cost: For small applications, the lower tiers of App Services are usually cheaper than running a VM.
Ease of Use: I only focus on developing my app.