---

copyright:
  years: 2015, 2020
lastupdated: "2022-07-21"

subcollection: mas-saas

---

{:shortdesc: .shortdesc}
{:screen: .screen}  
{:codeblock: .codeblock}  
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:external: target="_blank" .external}

# Provisioning
{: #provisioning}

## Process
{: #process}

Important:

Customers must purchase (or own) App Points for MAS prior to (or in conjunction with) ordering the Maximo Application Suite as a Service (MAS-SaaS). The service provides AWS Cloud based hosting, product installation, operation, maintenance and support for MAS.

The provisioning process is invoked when a client has placed an order using MAS-SaaS part numbers.

Each client is provisioned in an environment that is separate and distinct from other clients.  The provisioning is done to meet the specific customer requirements for a specific order.  This means there is no pre-provisioning done and client environment provisioning begins when an order is placed. 

The provisioning process has several steps, most of them automated, but some that require a manual update(s) to complete.  The time frame to complete provisioning will depend on several factors including:
 
* the size of the order
* the order complexity
* the number of orders in the queue ahead of the order

In general, allow for at least 4 weeks for provisioning to be completed.  

The provisioning itself can be broken down into a number of steps:
 
* Order validation
* Information gathering
* Initial provisioning of MAS base environment
* Provisioning of the individual MAS products the clients has requested
* Internal IBM verification of the provisioned environments
* Welcome letter sent to the client / designated contacts indicating provisioning is complete

## Order Validation
{: #order-validation}

Once an order has been placed, the initial step is to validate the order and the information submitted.  This includes checking the part numbers, ensuring the provisioning form has been completed, performing IBM internal financial checks and setting up the order to be provisioned.  In general this can take 1 to 2 days to complete.

Once this is complete, the order is sent to the IBM MAS-SaaS SRE Provisioning Team to begin the provisioning of the order.

## Information Gathering
{: #information-gathering}

Once the order has been placed into the provisioning queue, additional information needs to be validated and gathered.  This includes preparing the final architecture for the order; specifying the infrastructure needed to meet the order requirements; ensuring requested URL(s) are valid and available; detailed review of the order to ensure completeness; meeting or clarifying specific items with the sales person or client as required and setting up the provisioning parameters.

This step can take a few hours to several days depending on the initial quality and completeness of the information.  Critical information that is needed includes:
 
* products that to be deployed (not all products will be deployed by default).
* anticipated sizing information for each product - this can be based on users, I/O or other metrics specific to each product URL being requested
* Languages required
* Add On and/or Industry Solutions required
* location of the majority of users to determine optimal placement of the Suite in the proper AWS data center

If this information is missing or incorrect it can cause delays in the provisioning process while this information is being confirmed.

## Initial Provisioning
{: #initial-provisioning}

The initial provisioning covers several key aspects of the Maximo Application Suite deployment.

The base architecture is finalized regarding the size and number of OpenShift clusters needed.  The provisioning of all based components and configuration is performed and the initial DNS registration for the Maximo Application Suite done.  A temporary license file is installed.  The client will need to supply the final license file.

## Provisioning of the Individual Products
{: #provisioning-of-the-individual-products}

At this point, the products the client has selected is provisioned based on the sizing parameters that were specified.  This includes deploying the appropriate containers within OpenShift and configuring the products to be available to the client.  This includes the application, database, any network configuration required, DNS registrations and set up of client administration users. 

At this stage, all operational configuration is finalized including ensuring backups are configured properly, monitoring in place and security scans completed.  Alerting is configured and the sites added to the MAS-SaaS escalation process.

## Final Verification of the Provisioning
{: #final-verification-of-the-provisioning}

A final review of the install is done to ensure what has been deployed meets the order and the additional information gathered.  At this point, the order is marked complete and a [welcome letter](/docs/mas-ms?topic=mas-ms-getting-started-with-ibm-maximo-application-suite-managed-service#welcome-letter) is sent to the client.
