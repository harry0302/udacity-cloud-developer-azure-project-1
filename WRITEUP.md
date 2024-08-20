# Write-up Template

### Analysis, Selection, and Justification of the Appropriate Resource Option for Deploying the App

*For both VM and App Service solutions for the CMS app:*
- **Costs:** App Service generally incurs lower costs compared to VMs for similar workloads.
- **Scalability:** VMs offer extensive scalability but require manual configuration. In contrast, App Service simplifies scalability through auto-scaling options.
- **Availability:** App Service is inherently designed for high availability without much manual configuration. On the other hand, achieving high availability with VMs requires manual setup but offers more control.
- **Workflow:** App Service is ideal for hosting web applications, APIs, and microservices that don't need direct access to the underlying OS. Deploying an app on VMs is more complex, but it provides greater control over the OS and configuration.

*Selected solution for deploying the app:* App Service

*Justification for the choice:* The current CMS is a small web application with simple APIs (such as view, create, edit). Since we don’t need control over the infrastructure or custom software installations, App Service is chosen for its simplicity, cost-effectiveness, and the ability to avoid the time-consuming manual configuration process.

### Assessment of Future App Changes That Could Alter the Decision

In the future, if the app grows and becomes more complex, requiring advanced software dependencies, legacy components, custom networking, hardware access, or specialized resources, the VM solution would be more appropriate. VMs offer better performance and scalability in such scenarios.
