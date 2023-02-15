# Installation

1. To install this solution pack, click **Content Hub** > **Discover**.
2. From the list of solution packs that appear, search for **CICD - Change Management** solution pack.
3. Click the **CICD - Change Management** solution pack card.
4. Click the **Install** button on the bottom to begin the installation.

## Prerequisites

**CICD - Change Management** has no dependency on any of the solution packs. However, it has following prerequisites:

1. **Organizational account**: A GitHub organization account is a type of account that represents an organization, instead of an individual user. It allows multiple users to collaborate on projects and manage access to repositories and teams.

    Refer to this article to know more about [types of GitHub Accounts](https://docs.github.com/en/get-started/learning-about-github/types-of-github-accounts#organization-accounts).

2. **GitHub User Account**: Users must have their GitHub accounts. You can then use their usernames to invite them to your organization.

    Refer to this article to know more about [creating accounts for people in your organization](https://docs.github.com/en/organizations/managing-membership-in-your-organization/can-i-create-accounts-for-people-in-my-organization#adding-users-to-your-organization).

3. **GitHub User Roles**: To use the wizard for setting up source control and creating repositories through playbooks, FortiSOAR admin must have appropriate rights to create repositories on GitHub.

    Refer to this article to know more about [assigning roles and permissions on GitHub](https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/repository-roles-for-an-organization#permissions-for-each-role).

4. **GitHub Repositories**: You may need to create GitHub repositories if you prefer to link existing repositories with this solution pack instead of letting this solution pack's playbooks create repositories for you.
    For mapping repositories with content changes on the FortiSOAR instance, there must be the following three repositories:
    1. **Content repository**: Production content, dev, staging and test changes should reside on multiple, aptly named branches on the *same* repository.

    2. **Production Settings Repository**: Production settings containing system views, application configuration, environment variables, account configuration, LDAP, SSO, and RADIUS configuration of a production environment are backed up or synced on this repository.

    3. **Development Settings Repository**: Development settings containing system views, application configuration, environment variables, account configuration, LDAP, SSO, and RADIUS configuration of a development environment are backed up or synced on this repository.

    > **NOTE**: GitHub users who are setting up production environment in CICD - Change Management and creating repositories, must have permissions to create private repositories on GitHub. For more information, refer to Restricting repository creation in your organization.

# Configurations

This section details the required configurations for optimal performance of the **CICD - Change Management** solution pack.

- A source control connector for tracking and managing changes to code:
    -	To configure and use the GitHub connector to track and manage changes through GitHub, refer to [Configuring GitHub](https://docs.fortinet.com/document/fortisoar/1.0.0/github/344/github-v1-0-0#Configuration_parameters).

>**NOTE**: FortiSOAR users directly interacting with GitHub must be appropriately mapped with corresponding usernames in their GitHub connector configurations.