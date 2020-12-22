#TODO: update alt text on images
#TODO: how do we limit acceptable states for a user to sign in from?

# Challenge 2 - Sign Up, Sign In User Flow

## Prerequisites

There are no prerequisites that are new from the end of challenge 1. Must have an existing B2C tenant.

## Introduction 

This challenge will walk your attendees through a standard, simple sign up & sign in (SUSI) [user flow](https://docs.microsoft.com/en-us/azure/active-directory-b2c/add-sign-up-and-sign-in-policy?pivots=b2c-user-flow). 

## Hackflow

1. If you are coming immediately from the previous hack, once your B2C tenant completes provisioning, it will present you with the option to click to work in your new tenant. Do that.<br><img src="images/02/successful-creation-of-tenant.png" alt="image of search" width="500"/>
    - If you are not coming from the creation screen, you will need to find your tenant in the resource group you dropped it in or switch directories in the Azure portal. 
2. In your new tenant, we will first need to create a [custom attribute](https://docs.microsoft.com/en-us/azure/active-directory-b2c/user-flow-custom-attributes?pivots=b2c-user-flow#create-a-custom-attribute) for the consultant ID. <br><img src="images/02/custom-attribute.png" alt="image of search"/>
3. Now we are ready to create our user flow. Select "User flows" and click the "New user flow" button<br><img src="images/02/signup-signin-user-flow.png" alt="image of search" width="700"/>
3. On the Create a user flow page, select the Sign up and sign in user flow.<br><img src="images/02/select-user-flow-type.png" alt="image of search" width="700"/>
4. Under Select a version, select Recommended, and then select Create. <br><img src="images/02/select-version.png" alt="image of search" width="700"/>
5. On the creation screen, name your flow. Something like "susi" is acceptable. This will make a policy called __B2C_1_susi__. <br><img src="images/02/create-susi.png" alt="image of search" width="700"/>
6. Still on the creation screen, make sure you select "Email signup" as your option for local accounts. Once this is done, click the create button. <br><img src="images/02/create-susi-2.png" alt="image of search" width="700"/>
    - You may want to have a brief discussion with your team about the MFA enforcement options and what this could mean for them in their organizations. 
7. The creation should happen quickly, and you should pop back into the user flows blade. Click the name of your user flow to edit. <br><img src="images/02/user-flow-select.png" alt="image of search" width="700"/>
8. Under settings, select "User Attributes". Your attendees will then select the proper attributes from their challenge.<br><img src="images/02/user-attributes.png" alt="image of search" width="700"/>
    - First Name
    - Last Name
    - Display Name
    - Email Address
    - City
    - State
    - CMC Consultant ID
9. To customize the appearance, select "Page layouts" under Customize, and then select the templates dropdown. For this hack, the slate gray template is preferred: <br><img src="images/02/customize-template.png" alt="image of search" width="700"/>

## Alternate Hackflow

## Hints

[< Previous challenge (Provisioning a B2C Tenant)](./01-provision-b2c.md)[Next challenge (External Identity Providers) >](./03-.md)