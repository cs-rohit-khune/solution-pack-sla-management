| [Home](../README.md) |
 | -------------------------------------------- |

  # Contents

The **SLA Management** solution pack contains the following resources.

## Module Schema

| Name          | Description                                                                                                                                                                                                                                        |
|:--------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| SLA Templates | SLA Templates in FortiSOAR help create an in-built SLA management for incidents and alerts. For more information, please refer to [SLA Management](https://docs.fortinet.com/document/fortisoar/7.5.0/administration-guide/792686/sla-management). |

## Connector

| Name           | Description                                                                                                                                           |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------------------------------|
| SLA Calculator | Calculates SLA due date based on locale and work hours. This connector needs soar framework solution pack for supporting playbooks and module changes |

## Roles

| Name                 | Description                                                               |
|:---------------------|:--------------------------------------------------------------------------|
| SOC Manager          | Adds Create, Read, and Update permissions for SLA Templates module        |
| Full App Permissions | Adds Create, Read, Update and Delete permissions for SLA Templates module |
| SOC Analyst          | Adds Read permissions for SLA Templates module                            |
| Read-Only User       | Adds Read permissions for SLA Templates module                            |


## Playbook Collection

| 06 - IRP - Case Management |
|:--------------------------:|

| Playbook Name                                                           | Description                                                                                                            |
|:------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------|
| Alert - [01] Capture All SLA (Upon Create)                              | Updates the alert's acknowledgement due date and response due date based on the alert’s severity.                      |
| Alert - [02] Capture Ack SLA (Upon Update)                              | Updates the alert's acknowledgement date and SLA Status based on when the alert status is changed.                     |
| Alert - [03] Capture Response SLA (Upon Update)                         | Updates the alert's response date and SLA Status based on when the alert status is changed.                            |
| Alert - [04] Check for SLA violations                                   | Checks periodically for violations of acknowledgement SLA of the open alerts.                                          |
| Alert - [05] Update Ack and Response Due dates (Post Severity Change)   | Updates the alert’s acknowledge due date and response due date for change in the severity of alerts                    |
| Alert - Periodic Update Alert SLA Status                                | This is a subroutine playbook to periodically check violations of acknowledgement and response SLA of the open alerts. |
| Alert - Update SLA Details                                              | Updates an alert's acknowledgement due date and response due date based on the severity of the alert.                  |
| Fetch SLA Details                                                       | Fetches SLA Details for incidents as per Service, that is, for MSSP or Enterprise.                                     |
| Incident - [01] Capture All SLA (Upon Create)                           | Updates an alert's acknowledgement due date and response due date based on the severity of the incident.               |
| Incident - [02] Capture Ack SLA (Upon Update)                           | Updates an incident's acknowledgement date and SLA status when the status of the incident is changed.                  |
| Incident - [03] Capture Response SLA (Upon Update)                      | Update an incident's response date and SLA status when the status of the incident is changed.                          |
| Incident - [04] Check for SLA violations                                | Periodically check Acknowledgement SLA violations of the Open Incidents.                                               |
| Incident - [05] Update Response and Ack Due date (Post Severity Change) | Update an incident's acknowledgement due date and response due date following a change in severity.                    |
| Incident - [06] Check for Ack SLA violations                            | Notifies users of violation of Acknowledgement SLA.                                                                    |
| Incident - [07] Check for Response SLA violations                       | Notifies users of violation of Response SLA.                                                                           |
| Incident - Periodic Update Incident SLA Status                          | This is a subroutine playbook to check and update an incident’s SLA status.                                            |
| Incidents - Update SLA Details                                          | Updates an alert's acknowledgement due date and response due date based on incident severity.                          |
| Notify Ack SLA Violation                                                | Notify user for Acknowledgement SLA violation                                                                          |
| Notify Response SLA Violation                                           | Checks every 5 minutes for Response SLA violations of acknowledged incidents.                                          |
| Pause SLA - Alerts                                                      | Pauses the alert's acknowledgement or response when its respective SLA status is changed to 'Awaiting Action'.         |
| Pause SLA - Incidents                                                   | Pauses the incident's acknowledgement or response SLA when its respective SLA status is changed to 'Awaiting Action'.  |



## System View

| Name       |
|:-----------|
| Automation |

>**Warning:** We recommend that you clone these playbooks before customizing to avoid loss of information while upgrading the solution pack.

# Next Steps
| [Installation](./setup.md#installation) | [Configuration](./setup.md#configuration) | [Usage](./usage.md) |
| ----------------------------------------- | ------------------------------------------- | --------------------- |