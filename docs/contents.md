# Contents

The **Continuous Delivery** solution pack installs the following resources:

## Roles

|Role|Description|
|:-|:-|
|Production Administrator|Responsible for change request administration in Continuous Integration and Continuous Delivery (CICD)|
|Full App Permissions|Essentially the root user, use carefully|
|Content Developer|Responsible for change request development in Continuous Integration and Continuous Delivery (CICD)|

## System Views

|System View|Description|
|:-|:-|
|Continuous Delivery|A menu option that launches the Continuous Delivery user interface for setting up development and production environment subsequent interactions with source control.|

## Module Schemas

|Module Schema|Description|
|:-|:-|
|People|Adds fields to people schema to help organize information specific to users interacting with GitHub like their names and GitHub usernames.|
|Change Management|A schema or framework that helps organize information specific to Continuous Delivery like issue, title, description, and environment.|

## Widgets

|Widgets|Description|
|:-|:-|
|JSON to Grid|Renders the JSON playbook results in grid view and performs various operations on the grid.|
|CICD Configuration Wizard|Launches a wizard that walks a user through the process of setting up source control for Continuous Delivery.|
|Record CTA Tile|Displays the details of a module record, in Tile form, when the containing button is clicked; and also shows a Call To Action Button to Launch the Record Details Panel|
|Record Card|Displays the module records in a card format.|

## Playbook Collections

|02 - Use Case - CICD|
|:-|

|Playbook Name|Description|
|:-|:-|
|Update Export Templates|Update the export templates using the import files from source control|
|Synchronize Export Templates|Synchronize export template with latest source control data|
|Setup Production Environment|Execute Setup Production Environment Task on specified record|
|Setup Export Templates|Generates an initial template for exporting the content, such as playbooks, module definitions, etc to source control.|
|Setup Export Templates - Content and Settings|Synchronize Content and Settings Export Template in export wizard|
|Setup Development Environment|Setup the FortiSOAR Prod Content, FortiSOAR Dev Settings source control repositories|
|Setup CICD Environment|Update the SVT of Change Management module as per the environment selected in CICD Configuration wizard|
|Set Logged in GitHub Username|Update the GitHub Usernames in FortiSOAR  logged in user record|
|Set GitHub Username|Update the GitHub Usernames in FortiSOAR User record|
|Save FortiSOAR Settings|Backup connector configurations, SSO settings, user configurations, etc, into GitHub|
|Push Content|Clone the specified repository, apply the export template content and push to source control|
|Push Change to Source Control|Push (Export) specified change request content into the GitHub content repository|
|Push (Initial) Production Environment Content|Push initial Production Environment Content into GitHub main branch|
|Push (Export) CR Content to GitHub - Update Export Config Attachment|Update the "Export Template Configuration" attachment|
|Push (Export) CR Content to GitHub - Extract Export Zip File from FortiSOAR|Extract "FortiSOAR Production Environment" exported Zip File from FortiSOAR|
|Pull Latest Content from GitHub|Pull latest content from GitHub and apply it on production environment or development environment|
|Merge Pull Request|Marge the specified Pull Request if Pull Request is Approved.|
|GitHub - Update Remote Repository|Applies changes made in a FortiSOAR file to the specified remote repository that is cloned from GitHub based on the file IRI and cloned repository path you have specified|
|GitHub - Update Issue|Update an issues for the specified repository or user on GitHub based on the repository name, and other input parameters you have specified|
|GitHub - Push Changes|Commits the local repository changes to the specified repository in GitHub based on the repository name, cloned repository path, and other input parameters you have specified|
|GitHub - Merge Pull Request|Merges the specified pull request on GitHub based on the repository name, repository owner, pull request number, and other input parameters you have specified|
|GitHub - List Repository Issue|List an issues for the specified repository or user on GitHub based on the repository name, and other input parameters you have specified|
|GitHub - List Pull Request|Lists pull requests for the specified repository on GitHub based on the repository name, repository owner, and other input parameters you have specified|
|GitHub - List Pull Request Reviews|Lists the reviews associated with the specified pull request on GitHub based on the repository name, repository owner, pull request number, and other input parameters you have specified|
|GitHub - Fetch Release|Fetches Release from the Repo|
|GitHub - Delete Branch|Delete a new branch in GitHub based on the repository name, branch name, repository owner, and other input parameters you have specified|
|GitHub - Create or Update File Content|Creates a new repository using a repository template based on the template repository, repository name, and other input parameters you have specified|
|GitHub - Create Repository|Creates a new organization or authenticated user repository based on the repository name, organization name, base branch name, and other input parameters you have specified|
|GitHub - Create Release|Create a new release|
|GitHub - Create Pull Request|Creates a pull request for the specified repository on GitHub based on the repository name, repository owner, and other input parameters you have specified|
|GitHub - Create Issue|Creates an issue for the specified repository or user on GitHub based on the repository name, and other input parameters you have specified|
|GitHub - Create Branch|Creates a new branch in GitHub based on the repository name, base branch type, repository owner, and other input parameters you have specified|
|GitHub - Clone Repository|Clone the github repository|
|GitHub - Add Reviewers for a Pull Request|Adds reviews for the specified pull request on GitHub based on the repository name, repository owner, pull request number, and other input parameters you have specified|
|GitHub - Add Pull Request Review|Add a review for a pull request on GitHub based on the repository name, repository owner, pull request number, and other input parameters you have specified|
|Get Issue and Source Control Details|Extract the issue and source control details based on the specified information|
|Get GitHub Connector Configuration|If GitHub connector is configured for the logged in user then return connector configuration id else raise exception|
|Fetch Open Requests (Issues)|Fetch all open GitHub requests (Issues) from Content, Production Setting and Development Setting repositories|
|Fetch Latest Changes|Fetches the details of Latest changes available after last Sync|
|Create a Request (Issue)|Creates a Github Issue against the FortiSOAR Content or Settings Repository with the request content|
|Create Repository|Create the Public Repository for the specified repository name and base branch name in GitHub|
|Create Release|Creates a release from the base branch|
|Create Pull Request|Create the pull request|
|Configure Source Control|Create Content, Production Settings and Development Settings Repository in GitHub|
|Close Change Request|Closed the change Request and and Delete the specified change request branch|
|Check Playbook is Already Running|Specify the playbook name and check whether the playbook is already running|

## Connectors

|Connector|Description|
|:-|:-|
|GitHub|This connector facilitates automated interactions with Github such as creating and managing repositories, branches, issues, and pull requests.|

## Record Sets

- Attachments
- Continuous Delivery

## Picklists

- Environment
- Task Status
- Task Type

## Module Views

- List
- Detail
- Form
