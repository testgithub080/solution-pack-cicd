# Release Notes

## Enhancements

>**IMPORTANT**: This solution pack now requires FortiSOAR version `7.4.0` and later

- Added the tag `CICD` to enhance searchability for the *Continuous Delivery* solution pack on Content Hub

- Aligned the sequence of the task *Setup the Development Environment* with *Setup the Source Control for Production Environment*

- Removed the dependency on the **Attachments** records to create export templates

    - Added *Content and Settings Export Templates* in export template record

- Added a new team *Content Development* to add users involved with content development in FortiSOAR

### Playbook Enhancements

- Added Pull Request (PR) title as an issue comment in *Create Pull Request* playbook

- Pass input record to child playbook in The *Fetch Latest Changes* playbook

- Renamed *Get User Confirmation* step to *Confirm Apply Latest Changes* in *Pull Latest Content from GitHub* playbook

- Removed redundant *Update Import Job* and *Modify Configuration Option* steps from *Setup Development Environment* playbook

- Added *Add Repository Collaborator* step in *Set GitHub Username* playbook

- Following playbooks were added
    - GitHub - Create Issue Comment
    - GitHub - Add Repository Collaborator

- Following playbooks were removed
    - Update Export Templates
    - Synchronize Export Templates
    - Setup Export Templates
    - Setup Export Templates - Content and Settings
    - Push (Export) CR Content to GitHub - Update Export Config Attachment

- Following playbooks were renamed to better communicate their purpose
    - *Push Content* playbook renamed to *Push Content to Source Control*
    - *Push (Initial) Production Environment Content* renamed to *Push Initial Production Environment Content*
    - *Push (Export) CR Content to GitHub - Extract Export Zip File from FortiSOAR* renamed to *Get FortiSOAR Export Templates*

- Following playbooks pass the branch name parameter from the GitHub connector to the solution pack's **GitHub - Clone Repository** playbook:
    - Push Initial Production Environment Content
    - Push Change to Source Control
    - Push Content to Source Control
    - Save FortiSOAR Settings
    - Setup Development Environment
    - Pull Latest Content from GitHub