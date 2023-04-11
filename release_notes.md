| [Home](./README.md) |
|----------------------|

# Release Notes

## Enhancements

>**IMPORTANT**: This solution pack now requires FortiSOAR version `7.4.0` and later

- Added the tag `CICD` to enhance searchability for the *Continuous Delivery* solution pack on Content Hub

- Aligned the sequence of the task *Setup the Development Environment* with *Setup the Source Control for Production Environment*

- Removed the dependency on the **Attachments** records to create export templates

    - Added *Content and Settings Export Templates* in export template record

- Added a new team *Content Development* to add users involved with content development in FortiSOAR

- Option to invite collaborators with write permissions available during mapping GitHub users.

### Playbook Enhancements

- Added Pull Request (PR) title as an issue comment in *Create Pull Request* playbook

- Pass input record to child playbook in The *Fetch Latest Changes* playbook

- Renamed *Get User Confirmation* step to *Confirm Apply Latest Changes* in *Pull Latest Content from GitHub* playbook

- Removed redundant *Update Import Job* and *Modify Configuration Option* steps from *Setup Development Environment* playbook

- Added *Add Repository Collaborator* step in *Set GitHub Username* playbook

- *GitHub - Clone Repository* action uses the Codeload service that speeds up the subsequent push and pull operations

- Following playbooks were added
    - GitHub - Create Issue Comment
    - GitHub - Add Repository Collaborator
    - GitHub - List Repository Collaborator
    - Add GitHub Repository Collaborator
    - Push Content to Source Control
    - Push Initial Production Environment Content
    - Get FortiSOAR Export Templates

- Following playbooks were removed
    - Update Export Templates
    - Synchronize Export Templates
    - Setup Export Templates
    - Setup Export Templates - Content and Settings
    - Push (Export) CR Content to GitHub - Update Export Config Attachment
    - Push Content
    - Push (Initial) Production Environment Content
    - Push (Export) CR Content to GitHub - Extract Export Zip File from FortiSOAR

- Following playbooks pass the branch name parameter to the **GitHub - Clone Repository** playbook:
    - Push Initial Production Environment Content
    - Push Change to Source Control
    - Push Content to Source Control
    - Save FortiSOAR Settings
    - Setup Development Environment
    - Pull Latest Content from GitHub
