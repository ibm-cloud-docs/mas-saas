---

copyright:
  years: 2015, 2020
lastupdated: "2020-11-12"

subcollection: mas-saas

---

{:shortdesc: .shortdesc}
{:screen: .screen}  
{:codeblock: .codeblock}  
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:external: target="_blank" .external}

# Limitations & Exclusions
{: #limitations-exclusions}

Maximo Application Suite SaaS is implemented using a defined set of technologies and operates within a security profile designed to ensure our client's data is secure and the applications operate efficiently and effectively.  As a result of the decisions made regarding technologies and to meet the high security standards, there are differences between what is available using the Managed Services and what a client could do if they hosted and operated the Suite themselves.

The following items are not included or allowed in the Maximo Application Suite SaaS offering:

## Databases
{: #databases}

Only IBM DB2 Warehouse is supported.  Oracle and SQLServer are not supported.  Conversion services are available.

Note: DB2 Text Search is not supported.

Note: Running SQL statements (update/insert/delete) directly on the database is not allowed and IBM SRE team will not be able to execute those statements for you. Customers must carry out these changes using the UI via different means for example using Automation scripts or MIF. For further details on use of automation scripts, please see document below:

https://ibm-maximo-dev.github.io/maximo-autoscript-documentation/introduction/whatisautoscript

## Manage Application
{: #manage-application}

No Java extensions are supported.  It is assumed the Manage auomation scripting capability will be used for these types of extensions.  Existing Maximo customers who have Java extensions will need to move these functions into automation scripts within the application. See link above for further details.

## 3rd Party Applications
{: #3rd-party-applications}

Maximo Application Suite SaaS will not host or support any 3rd party applications.  3rd Party applications hosted outside the MAS-SaaS environment can be integrated to applications with the Suite provided they follow standard integration protocols.

## Access
{: #access}

Clients will not have access to the operating system, file system or overall system administration of the Suite.  DBAdmin access or direct updating of the database is not allowed.

## MAS Administrator Functions
{: #mas-administrator-functions}

Direct access to the clusters is not available.  Changes required must be submitted using an IBM support case system and the IBM SRE team will execute. 

## Self-Service Portal
{: #mas-ssp}

A self service portal (SSP) for MAS-SaaS is not available at this time and is under construction.

