# Release Information

- **Version**:  2.0.0
- **Certified**: Yes
- **Publisher**: Fortinet
- **Compatible Version**: FortiSOAR v7.4.0 and later
- [**Release Notes**](./release_notes.md)

# Overview

FortiSOAR Continuous Delivery solution pack helps automate your content development workflows and deploy better quality code using a continuous and iterative process to build, test, and deploy content through Source Control.

With Continuous Integration (CI) you can integrate all your code changes into the main branch of a shared source code repository early and often, automatically testing each change when you commit or merge them. FortiSOAR Continuous Delivery helps you create a development source control where you can merge your changes and test them until you are confident that the changes are ready to be pushed to production.

Continuous Delivery (CD) takes over during the final stages to ensure that the code can be pushed to a production environment (or a staging environment if you so choose) at any time. For more granular control, you can review the code changes before pulling them from development into production or staging. Even then you can wait until you are ready to apply the changes to a production or staging environment.

The following diagram simplifies how FortiSOAR's Continuous Delivery works:

![Continuous Delivery Flowchart](./docs/res/ci-cd-flow.svg)

## Intended Audience

This document is meant for content developers and FortiSOAR administrators who build FortiSOAR content to suit their daily requirements. Customizations to FortiSOAR content can be pushed to source control in the development environment. After ironing out any issues with customizations and when confident about the custom content, the same can be pushed to the production source control to be delivered/deployed on the production FortiSOAR instance.

# Terminology

This section provides a comprehensive list of specialized terms and definitions used in this document. It serves as a reference guide to ensure that any communication regarding FortiSOAR's **Continuous Delivery** solution pack is clear and consistent. The section may include definitions, abbreviations, acronyms, and jargon that are unique to this solution pack.

This terminology section may be regularly updated to reflect any changes or additions to the terms used throughout this document.

1. **Content**: Content or FortiSOAR content includes customizable components like playbooks, connectors, roles, and module schemas to name a few.

2. **Production Settings**: Production settings are system views, application configuration, environment variables, account configuration, LDAP, SSO, and RADIUS configuration in a production environment.

3. **Development Settings**: Development settings are system views, application configuration, environment variables, account configuration, LDAP, SSO, and RADIUS configuration in a development environment.

4. **FortiSOAR Admin**: A FortiSOAR admin has administrative rights on any FortiSOAR instance. For more information on users and roles, refer to [Tasks & Permissions](https://docs.fortinet.com/document/fortisoar/7.3.1/administration-guide/249178/overview#Tasks_and_Permissions) in  FortiSOAR Administration Guide.

5. **Source Control**: Source control (or version control) is the practice of tracking and managing changes to code. Source control management (SCM) systems provide a running history of code development and help resolve conflicts when merging contributions from multiple sources. A common example of source control is **GitHub** <img src="./docs/res/github.png" width="20">.

6. **Source Control Production Admin**: A source control administrator has the rights to create users, assign permissions, create, and manage repositories in an organization. Refer to the following article on GitHub detailing various user roles and access: [Roles in an organization](https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization).

# Initial Configuration

This section explains setting up initial configurations for GitHub source control.

1. **Setup a GitHub organization**: Creating a GitHub organization helps keep all repositories and users under a single umbrella.
    Refer to this article for [Creating new organizations](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/creating-a-new-organization-from-scratch).

2. **Create users with admin access**: Once an organization is set up, users with administrative access are required for creating private repositories and other users with different access.

    Refer to this article for creating and assigning [Roles in an organization](https://docs.github.com/en/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization).

3. **Create Repositories**: Repositories can contain folders and files, images, videos, spreadsheets, and data sets – anything your project needs. The Setup Source Control process in FortiSOAR's Continuous Delivery creates repositories for you. However, you can create repositories and map them with FortiSOAR's Continuous Delivery to store and collaborate on your content customizations.
    
    Refer to this article for [Creating and working with repositories](https://docs.github.com/en/get-started/quickstart/create-a-repo).

4. **Branching**: You can create branches so your changes do not affect the production content, and when ready can be merged into the main branch.

    Refer to this article on [Creating branches in a repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository).

5. **Staging, Committing, and pushing changes in GitHub**

    Refer to this article on [Contributing and collaborating on GitHub using GitHub Desktop](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop).

6. **Working with Personal Access Tokens**: Personal access tokens help avoid entering sensitive information like passwords. You can assign only relevant rights to your access token. GitHub connector in FortiSOAR requires a personal access token (classic) to be entered during configuration.

    Refer to this article for [Accessing GitHub using Personal Access Token (Classic)](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token#personal-access-tokens-classic.).


# Next Steps 
 
| [Installation](./docs/setup.md#installation) | [Configuration](./docs/setup.md#configuration) | [Usage](./docs/usage.md) | [Contents](./docs/contents.md) |
|----------------------------------------------|------------------------------------------------|--------------------------|--------------------------------|
