# Challenge 0: Pre-requisites - Ready, Set, GO!

**[Home](./README.md)** - [Next Challenge >](./01-assessment.md)

## Coach tips

There are a lot of opportunities for things to go wrong in this step especially if the attendee does not follow the instructions!

* If the attendees are sharing an Azure subscription, the following items will need to be made unique in the create-cluster.sh file for each attendee:

    * resourceGroupName
    * clusterName

    The location may also potentially need to be made unique if you are getting errors related to quota.

*  Even though it's commented out, the AKS CLI tools may need to be installed if the attendee is not using Azure Cloud Shell

* Both the Azure CLI and Helm will need to be installed. These are included with Azure Cloud Shell but will need to be downloaded separately otherwise

* Attendees should not be using the public IP address of the PostgreSQL/MySQL containers when configuring the application.

* The attendees may make mistakes with the datasourceURL and username/password for PostgreSQL/MySQL. If the application isn't working, have the attendees check the log:

```bash
    kubectl -n {infrastructure.namespace goes here} logs deploy/contosopizza --tail=5000
```

* Google ReCaptcha will not work by default which means they will not be able to register as a user in the application. The attendee will need to generate their own. The instructions are here: https://github.com/pzinsta/pizzeria

* The approximate cost for this hack is about $15/day:
    AKS: $90/month
    Azure DB for MySQL: $153/month
    Azure DB for PostgreSQL: $139/month

    Total: $382/month (or $13 + any incidental charges for storage, private endpoints, etc.)

* This hack can be done in an Azure trial account (one attendee per Azure trial). However, Microsoft anti-fraud detection may prevent multiple Azure trial subscriptions from being created in the same network location. Also, each attendee will need a working credit card to setup an Azure trial subscription (even though the card will not be charged).


