# Identity for Developers

## Introduction

The Identity for Developers Hack will provide you a deep dive experience into enabling internal and external identity solutions for your applications. Identity is a booming area of the Microsoft Cloud platform and enabling identity solutions in your engagements allows for faster production deployments.

## Learning Objectives

In this hack, we'll enable identity solutions for several applications, demonstrating how to

1. Provision several types of Managed Identities
2. Set up an Azure Active Directory and enable External Identities
3. Set up an Azure Active Directory B2C directory for customer-facing applications, utilizing:

   a. Out of the box user flows

   b. Customized policies

   c. REST APIs for token enrichment and custom approval workflows

## Challenges

Challenge 0: **[Prepare your workstation for Identity development](Student/Challenge-00.md)**

- Get yourself ready to develop Identity solutions

Challenge 1: **[Provision an Azure AD B2C Tenant](Student/Challenge-01.md)**

- Provision a B2C Tenant

Challenge 2: **[Create a Sign Up and Sign In Experience](Student/Challenge-02.md)**

- Create a simple Sign Up and Sign In user flow and connect it to an ASPNETCORE MVC App

Challenge 3: **[Set Up an External IdP](Student/Challenge-03.md)**

- Set up the ability for your users to log in to your app with a GitHub, Facebook, or Gmail identity

Challenge 4: **[Customize Look and Feel and Localization](Student/Challenge-04.md)**

- Add a bit of flare to your sign up and sign in pages by adding your company's logo, colors, and custom layouts to the user experience along with supporting multiple languages

Challenge 5: **[Enrich Claims During Sign-Up](Student/Challenge-05.md)**

- Enrich the claims that you collect about a user during the sign up process by calling out to a custom REST API

Challenge 6: **[Prepare Environment for Custom Policies](Student/Challenge-06.md)**

- We'll need custom policies, so let's get things ready. Apply the Trust Framework and also create an OIDC IdP for your external IdP

Challenge 7: **[Stepping Up To Custom Policies](Student/Challenge-07.md)**

- Implement a custom policy for Sign In that will call to your custom REST API to perform claims enrichment for users that signed up prior to Challenge 5. Also, we'll break the Sign Up and Sign In policy to be just a Sign Up policy.

Challenge 8: **[Tracking a User's Journey in a Policy](Student/Challenge-08.md)**

- Enable App Insights in your custom policy so you can track a user through the various steps in the Orchestration. Add custom events to your Orchestration and track them in App Insights.

Challenge 9: **[Add a SubJourney for Terms of Service](Student/Challenge-09.md)**

- Create a subjourney in your orchestration to check whether a user needs to accept an updated version of the company's Terms of Service and record that the user has accepted them.

Challenge 10: **[Parameterize Your Custom Policies](Student/Challenge-10.md)**

- Take your custom policies and parameterize the values that could change from environment to environment, and use the B2C extension to VS Code to generate environment-specific policy files.

Challenge 11: **[Admin the B2C Tenant with MS Graph](Student/Challenge-11.md)**

- Use the MS Graph API to query your B2C tenant. Also use the Graph API to update various objects in your B2C tenant, such as policies, keys, and identity providers.

## Prerequisites

- Your own Azure subscription with Owner access
- Visual Studio Code
- Azure CLI

## Repository Contents (Optional)

- `../Coach/Guides`
  - Coach's Guide and related files
- `../SteamShovel`
  - Image files and code for steam shovel microservice
- `../images`
  - Generic image files needed
- `../Student/Guides`
  - Student's Challenge Guide

## Contributors

- David Hoerster
- ???
