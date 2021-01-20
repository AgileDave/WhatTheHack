# Challenge \#9 - Creating Custom Policies

[< Previous Challenge](./08-prepare-ief.md) - **[Home](../readme.md)** - [Next Challenge>](./10-appinsights.md)

## Pre-requisites (Optional)

- Provisioned a B2C tenant
- Deployed the Identity Experience Framework (IEF)

## Description

Now that you've set up the IEF environment, we can begin to clean up the users that signed up with an invalid CMC ID prior to challenge 5. We'll incorporate the REST call for claims enrichment for this sign-in process in order to validate the consultants's CMC ID and alert the user if it's invalid.

Your CMC QA team has put together a checklist of steps that they will check to validate that a user's CMC ID is properly in place in the B2C directory. The steps include:

- Upon sign-in, the user's account is checked for the presence of a CMC ID. If one is not found for that account, then:
  - Present a self-asserted form where the user enters their CMC ID
  - The user's CMC ID is then run through the "CMC ID Verify-inator" to validate the ID and return the new territory name
  - Of course, if the CMC ID is invalid, then a friendly error message is presented
  - Save the CMC ID and Territory Name to the user's account
- If the user's account has a CMC ID and does not have a territory name associated with it, then:
  - Run the CMC ID through the "CMC ID Verify-inator" to validate the ID and return the new territory name
  - If the CMC ID is invalid, present a friendly error message
  - Save the Territory Name to the user's account
- If the user's account has a CMC ID and Territory Name, proceed with signing the user in.

## Success Criteria

To successfully pass this challenge, you should be able to demonstrate:

- A user with a missing CMC ID will have their CMC ID and Territory Name populated upon successful sign-in;
- A user with an existing CMC ID that is invalid will not be able to sign-in;
- A user with an existing CMC ID that is valid will be able to sign-in along with having their Territory Name populated; and,
- A user with a valid existing CMC ID and Territory Name will be able to sign-in without issue.

## Learning Resources

**[RESTful Technical Profile for Custom Policies](https://docs.microsoft.com/en-us/azure/active-directory-b2c/restful-technical-profile)**
**[AD B2C Sample - Integrate REST API claims exchanges](https://github.com/azure-ad-b2c/rest-api)**
**[UserJourneys and Preconditions reference](https://docs.microsoft.com/en-us/azure/active-directory-b2c/userjourneys)**

## Tips

**- Consider using Preconditions on the existence of your claims (CMC ID and Territory Name), and use this for branching in your UserJourney.**

**- Consider creating a few dummy users via the Azure B2C Portal for testing - they won't have a CMC ID nor Territory Name.**
