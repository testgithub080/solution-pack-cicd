| [Home](../README.md) |
|----------------------|

# Upgrade Instructions

This section points out some actions to take before and after the upgrade to **Continuous Delivery** `v2.0.0`.

> **IMPORTANT**: Follow these instructions closely and do not skip either of them.

## Prerequisites

- Update the GitHub connector to `v1.1.0` before initiating upgrade.

## After Upgrade

Perform these actions after a successful upgrade to **Continuous Delivery** `v2.0.0`.

- Delete the following newly-added export templates if they have no **Last Export Date**.
    - Source Control - Production Content
    - Source Control - Development Settings
    - Source Control - Production Settings

- Run the Continuous Delivery configuration wizard again. Refer to the section [Configuration Wizard](./setup.md#setup-continuous-delivery-on-fortisoar).

- Uncheck the **Attachments** module from the export template if it contains only the export templates.

- Ensure that following playbooks are deactivated:
    - Update Export Templates
    - Synchronize Export Templates
    - Setup Export Templates
    - Setup Export Templates - Content and Settings
    - Push (Export) CR Content to GitHub - Update Export Config Attachment
    - Push Content
    - Push (Initial) Production Environment Content
    - Push (Export) CR Content to GitHub - Extract Export Zip File from FortiSOAR
