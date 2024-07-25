[Home](../README.md) |
|--------------------------------------------|

# Installation

1. To install a solution pack, click **Content Hub** > **Discover**.
2. From the list of solution pack that appears, search **SLA Management**.
3. Click the **SLA Management** solution pack card.
4. Click **Install** on the lower part of the screen to begin the installation.

## Prerequisites
The **SLA Management** solution pack depends on the following solution packs that are installed automatically &ndash; if not already installed.

| Solution Pack Name | Version         | Purpose                                |
|:-------------------|:----------------|:---------------------------------------|
| SOAR Framework     | v3.0.0 or later | Required for Incident Response modules |

To create and manage SLAs, you must be assigned a role with the following minimum permissions:

1. `Create`, `Read`, and `Update` permissions on the **SLA Templates** module
2. `Execute` permission on the **Playbooks** module
3. `Usage` permission on the **Widgets** module
4. Default `Read` permission on the **Application** module
5. Appropriate permissions to access the **Alert** and **Incident** modules, if displaying SLA within these module records

# Configuration
For optimal performance of **SLA Management** solution pack, you can install and configure the following connector that help with the following:

>* **SLA Calculator** - Calculates SLA due date based on locale and work hours. This connector needs SOAR framework solution pack for supporting playbooks and module changes. To configure and use the SLA Calculator connector, refer to [Configuring SLA Calculator](https://docs.fortinet.com/fortisoar/connectors/slacalc)


# Next Steps
| [Usage](./usage.md) | [Contents](./contents.md) |
|---------------------|---------------------------|