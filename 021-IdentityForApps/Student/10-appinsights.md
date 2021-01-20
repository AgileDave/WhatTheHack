# Challenge \#10 - Getting Insights Into B2C

[< Previous Challenge](./09-custom-policy.md) - **[Home](../readme.md)** - [Next Challenge>](./11-subjourney.md)

## Pre-requisites (Optional)

- Provisioned a B2C tenant
- Deployed the Identity Experience Framework (IEF)
- Deployed the Challenge 9 Sign-In Policy

## Description

Your innovative developer (the one who developed the "CMC ID Verify-inator") has been paying attention to your efforts with custom policies and has decided to take a shot at building one. The developer's custom policy has been provided to you in your challenge materials, and the CMC QA Team has asked you to deploy it to your B2C tenant. The policy is a sign-up policy that prompts a prospective customer with a few questions. At the end of the questioning, the user's account is provisioned along with the answers to their questions.

The custom policy deploys fine, but you notice that it doesn't work. When you test the policy in the B2C portal, it errors out on you.

You've decided to add some tracing to the custom policy in order to determine what the error might be. CMC IT Leadership, who's a big fan of your innovative developer, wants the issue fixed quickly...hopefully you find a solution so you can go home soon!

## Success Criteria

You will be successful with this challenge if you are able to:

- Determine where the error in the custom policy is;
- Demonstrate to your coach how you were able to detect the error;
- Redeploy the custom policy and have new users successfully go through the sign-up process without error

## Learning Resources

**- [Using Application Insights to Collect B2C Logs](https://docs.microsoft.com/en-us/azure/active-directory-b2c/troubleshoot-with-application-insights)**
**- [Use Application Insights to track user behavior](https://docs.microsoft.com/en-us/azure/active-directory-b2c/analytics-with-application-insights)**

## Tips

**- Make sure your Custom Policy is in `Developer` deployment mode.**

## Advanced Challenges (Optional)

If this was too easy, then try to add Usage Analytics to the steps in the custom policy. Test it out with a few users, having each of the users only get so far in their journey before quitting the process (and some successfully finishing the sign-up process).

Also, use different browsers to test your usage tracking, along, if possible, testing it out on different devices (mobile vs. desktop). This way, you'll have different sessions running.
