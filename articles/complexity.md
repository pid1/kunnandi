# Complexity

Complexity has to live somewhere and the real consideration is constraints.

Your organization needs some AWS resources spun up. In an organization with existing expertise in Terraform, Packer, and GitHub Actions, a CI/CD pipeline for this would be reasonable to create and maintain.

With no organizational understanding of these tools, the ability to make modifications within the UI, follow the upstream AWS documentation, and lean on AWS Support may be preferable until we can perform some cross-training and up-skill the team to where Terraform maintenance is reasonable. Given a team who has never maintained a Kubernetes cluster or containerized an app, would it be simple, or even responsible, to run this on EKS?

Is the "simple" solution consuming third-party cloud services? If the organization is too financially constrained for that, but person-hours, technological familiarity, and on-prem servers are all available to deploy an equivalent open source solution, is it then wrong to accept the operational complexity of maintaining that service rather than consuming it?

Understanding constraints and risk are deeply intertwined. See [Leadership -> Enabling high performers -> Understand and communicate risk](leadership.md#understand-and-communicate-risk).
