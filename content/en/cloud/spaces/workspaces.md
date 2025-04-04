---
title: Workspaces
description: >
  Meshery Workspaces serve as a virtual space for your team-based work.
weight: 6
categories: [Spaces]
---

Meshery Workspaces serve as a virtual space for your team-based work. Create a Workspace to organize your work and to serve as the central point of collaboration for you and your teams and a central point of access control to Environments and their resources.

You may create Workspaces to organize project-based work or to create domains of responsibility for your teams or segregate Designs and Environments and track team activity.

## Summary

Workspaces facilitate collaboration between you and your teams, allow you to control access to resources, and track activity and report on related events.

## Key Features

- **Resource Sharing** Workspaces allow for seamless resource sharing among team members, fostering collaboration.
- **Logical Grouping** Within Workspaces, you can group related components such as environments and infrastructure designs.
- **Flexibility**: Workspaces support various resources like Kubernetes, Prometheus, Jaeger, Nginx, and more.
- **Simplified Management** Managing and deploying resources is made easy within Workspaces.
- **Access Control** Workspaces allow you to control access to resources by granting permissions to users and teams.

### Workspace Relationships and Restrictions

- Access to Workspaces may be granted to one or more teams.
- As a point of collaboration to facilitate work, Workspaces may have zero or more Environments associated.
- A Workspace is closely associated with Teams in Meshery. Teams are groups of users with varying permissions, and they are at the center of resource access and management within a Workspace.
- One ore more teams can be assigned to a workspace.
- Same team can be assigned to multiple workspaces.
- A team can be assigned to a workspace only if the team is not already assigned to another workspace.

After creating a Workspace, of your next steps is to resource that Workspace. Like a shared drive (or or shared collection of files). Workspaces are your Google Drive, while Meshery Designs are your Google Docs.

## Key Workspace Components

### Environments

- Environments are a central part of a workspace. They serve as a logical grouping for managing connections. A connection, in this context, can be either managed or discovered by Meshery. Examples of connections include Kubernetes clusters, Prometheus instances, Jaeger traces, Nginx servers, and more.
- One or more environments can be assigned to a workspace.
- Same environment can be assigned to multiple workspaces.

{{< alert type="info" >}}
Assign any number of Environments to one or more Workspaces. See [Environments](https://docs.meshery.io/concepts/environments) section for more information.
{{< /alert >}}

### Designs

- Infrastructure Designs are essential for creating reusable deployment templates. Users belonging to teams with access to a workspace can utilize these designs to deploy resources in the Kubernetes clusters associated with that workspace.
- Like a shared drive (or or shared collection of files), Workspaces are your Google Drive, while Meshery Designs are your Google Docs.
- One ore more designs can be assigned to a workspace.
- Same design can be assigned to multiple workspaces.

{{< alert type="info" >}}
Designs belong to only one Workspace at any given time. See [Meshery Designs](https://docs.meshery.io/concepts/designs) section for more information.
{{< /alert >}}

### Teams 
- A Workspace is closely associated with Teams in Meshery. Teams are groups of users with varying permissions, and they are at the center of resource access and management within a Workspace.
- One ore more teams can be assigned to a workspace.
- Same team can be assigned to multiple workspaces.

{{< alert type="info" >}}
Teams offer control access to workspaces and to workspace resources such as environments and managed and unmanaged connections, See [Teams](/cloud/identity/teams).
{{< /alert >}}

### Connections

- Connections in Meshery refer to various resources that can be either managed or unmanaged, but are discovered and made accessible for use. Examples of Connections include Kubernetes clusters, Prometheus instances, Jaeger services, Nginx deployments, and more. These Connections serve as a fundamental part of Workspaces, as users can deploy infrastructure designs within the context of these Connections.
- Connections can be assigned to one or more environments.
- Same connection can be assigned to multiple environments.

{{< alert type="info" >}}
See [Connections](https://docs.meshery.io/concepts/logical/connections) section for more information.
{{< /alert >}}

## Best Practices

To make the most of Meshery Workspaces, here are some best practices:

- Clearly define permissions in the form of team assignment to ensure proper access control.
- Use Infrastructure Designs to standardize resource deployments.
- Regularly review and update your Workspace's resources and configurations.

Meshery Workspaces enhance collaboration within your teams, providing a structured environment for sharing and managing resources. By following best practices and understanding the core components of Workspaces, you can maximize the benefits of this feature in Meshery.
