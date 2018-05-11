---
layout: post
title: Our next release is coming!  Welcome to Beluga.
published: true
author: chris_cooper
comments: true
---


In this release we have some exciting new features.   The first is the enablement of a multi-lingual SDK.   The second is a new admin view which allows you to search a users consents direct from the dashboard.   Our third new capability is the automatic notification of a right to be forgotten to the consent service admin.   

Plus we have some other bug fixes and enhancements, including template versioning and allowing for additional information to be included in a new extension to the API when calling `/userconsent/setConsents`. 


## Supporting Multilingual Deployments

Consentua is being used in more countries that do not speak English than those that do.   At first we enabled multi-lingual support with the ability to append a translation table to the original template.   This is still there, and in a future release we will give admins the ability to append child translations to a parent template. 

This however, did not address the fact we had hard coded some elements of the SDK.    So we have done some internal engineering changes that have made the SDK’s completely language independent.   Now it is possible to change the static text to what is required for that language. 

If you have a need for a specific language template, then now you just write the template in that language from the start.   Append that template to a specific service.  Then add those users to that service using that languages template.  

<img class="img-center" src="{{ site.baseurl }}/public/post_imgs/2018-5-11-Our-next-release-is-coming!-Welcome-to-Beluga/Multi-Lingual.PNG" alt="img center">

## User Consent View

This is one change I have been waiting on for ages.   How does an admin quickly check a user consent without having to revert to the command line?  Answer:  Use the dashboard!  We have a new view which supports two queries into Consentua.   

The first is a user query.  This gives us the purposes that this user has agreed (or not) too.   Returning the true/false to a particular purpose ID.   The admin will need to know the purposes they have under their control.  
The second is the purpose query.  This gives the admin a list of users that have agreed to a specific purpose.   

  
<img class="img-center" src="{{ site.baseurl }}/public/post_imgs/2018-5-11-Our-next-release-is-coming!-Welcome-to-Beluga/Consentua-dashboard-reports.PNG" alt="img center">

## Right to be Forgotten

A key new right for us citizens with GDPR is the right to be forgotten.  Now Consentua can support this use case.  We have created a specific public template that you can append to your consent service.   This will always be the last template a user will see.  

The template when interacted with by a user will send an email notification to the client consent service admin.  The admin can then inform the data owner and insure that the request is followed up. 

We have made a conscious decision to stop at this point.  Some of our competitors will start digging through the weeds of your data in your organisation to make sure that the data is truly forgotten.   This is a step to far in terms of making Consentua easy to install.   Hence we have left it at the notification only stage at this time.   However, we do have a future collaboration planned depending on customer sponsorship with this use case in mind.   Watch this space!  

<img class="img-center" src="{{ site.baseurl }}/public/post_imgs/2018-5-11-Our-next-release-is-coming!-Welcome-to-Beluga/Notifiable-template.PNG" alt="img center">

## Ready

Beluga has exited our development environment and is released to test for current customers to check out the new features.   

To get access to the latest Consentua release.  Go to [contact Consentua](https://consentua.com/contact)

