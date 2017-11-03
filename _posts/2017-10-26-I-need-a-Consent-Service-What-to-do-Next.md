---
layout: post
title: I need a Consent Service. What to do Next
published: true
author: chris_cooper
comments: true
---


This is a blog aimed at developers, CTO’s, CIO’s, DPO’s and any one else involved in the enablement of technology to solve the challenges that GDPR throws up.  It will also be of interest to leaders of: compliance,marketing, customer service, operations.  At a stretch CFO’s & CEO’s.

## GDPR

Someone somewhere in your organisation has responsibility for compliance to the new General Data Protection Regulations (aka GDPR).  This responsibility may even rest on your shoulders.   

When GDPR comes into force on 25th May 2018 it will be a game changer.  Now your business has to take full responsibility of the personal data sitting on its servers.   It does not matter whether you are a data processor or a data controller.  The impact of GDPR will be felt across the organisation, as the changes it will require are going to impact your people (how to train your staff and new rights for citizens needing to be considered) and process (how to ensure ongoing compliance) as well as technology (some tools are going to be needed).   

## Privacy Impact Assessment

The GDPR gravy train is starting to build up speed and the business side of your organisation has been busy these last few months.  Deadline is approaching.    Ideally the focus will have been on the Privacy Impact Assessment (PIA).   This exercise teases out where the data is in your organisation and the intended use for that data.  

## My Requirement is….. 

Now that the PIA has been completed it is becoming apparent that a high level list of requirements are now building up.   These requirements are possibly along these lines:  

I need an easy method of capturing consent to use certain types of data for certain purposes.   I need to put my customers in control! But it has to be a great user experience.  
This consent capture has to be unambiguous, ongoing and understandable.   But don't impact the experience.  Nor damage my brand.  
I want the consent ‘receipt’ to be a trusted, inviolable audit point. 
This consent receipt should be in a secure, centrally managed space, so that it can be easily shared with multiple parties both inside & outside my organisation, yet always in a  controlled manner.  
I need to be able to change what I am asking for permission to process as my service is going to change its data types and purposes over time.  
I need to have a local language capability but at the same time… stay in the confines of the  corporate framework. 

## Keep Calm and Get Consentua

The good news is that a new consent management API service has recently come to market that will meet all of the above requirements.   The service is called Consentua.   With the added benefit that it takes the output from the Privacy Impact Assessment and applies this in the setting up of your very own Consentua Client Service.  

<img class="img-center" src="{{ site.baseurl }}/public/post_imgs/2017-10-13-Why-GDPR-is-good-for-Business-and-Citizens/keep-calm-and-get-consent-6.png" alt="img center">

Consentua does one thing very well.  It provides end users with a transparent and easy to understand explanation of the types of data and the purposes their personal data will be used for; whilst also giving the data controller flexible control over what is asked for and the ability to change this anytime.  As well as providing both parties with a central audit point of the consent granted; plus it is secure, lightweight and easy to install.  

## So I want this new service?  How long will it take?

Anywhere from half a day upwards depending the on scale and complexity of your organisation, app deployment schedules and resources to work on the project.   From our end the set up takes minutes.  From your perspective it depends… but to gauge the effort here is what it takes.  

## Not Long

Next step is to agree the consent language to be used (more of an internal team effort here) and the build of the consent template.  This defines what the data purpose is and what purpose groups are required.     Then we create your consent service that links your service and template together.   Finally the widget is seamlessly dropped into your existing browser or mobile app code.  

Once the service has gone through a test cycle the production service is live.  Ideally within two weeks of a successful completion of testing.  But this can happen the same day if all goes smoothly.  The biggest impact is on your organisation and how prepared you are in terms of the use of a new language to describe the data types and purposes.  

## What does the end user see?

Once the Consentua widget is in your code, when the customer launches the consent view (via the hamburger menu) it will call the API.  The API looks up the consent being requested for that users service, if the user has already saved a consent setting this too is returned.    The user can now play with their consents.   

Each user has their own URI and only that user can access the consent settings.  Who can access which consent service is determined by you.   Nice and secure, fully encrypted end-to-end too and in your control.  


## Developer Flexibility

Consentua is not just about apps though.  The service is also enabled to handle consent interactions from systems too.   For example it could be a CRM or customer engagement system that is looking to check customer consent to share data with a 3rd party prior to a campaign launch.  

The full API documentation can be found here:  
http://api.consentua.com/swagger/ui/index

## Any gotchas?

Only one.  Consentua needs to have a common identifier for users with the system calling the service.  Consentua will shortly support OAuth2.0 and multi-factor authentication.  For the moment the access is token driven.   

## What can the Business See?
From a business perspective Consentua provides the critical answer to this question..  What has the customer consented to?  This can be queried either via the API or via the dashboard.   The business can view who has consent to a particular type of interaction or by user.

The by user view is useful as well to support notification of breach, as well as notifying a customer on the data the business holds on them.   The by user view can be a handy way of establishing right to be forgotten proof as well. 

## I wanna change my mind

Yes is the answer.  Of course you can change your mind about the types of data and purposes they are used for and seek a new consent from your customers.   Consentua out of the box is fully configurable and in your control.  The changes can be made real time.  Next time the user goes to the consent view they will see the new data types and purposes.  

## Tactical v Strategic
Consentua can be used as a mix of both.  It could act as a ‘swing’ technology helping an organisation move to a more automated, streamlined future by enabling an evolutionary approach rather than a big bang.  It could be part of  tactical short term fix before a more strategic solution is deployed, but still allows re-use of the PIA and creates a standards based interoperable consent receipt.  Or it could be part of a strategic shift the organisation undertakes to be more transparent and trustworthy with the aim of asking for and using personal data for the benefit of both consumer and provider.   

## Must be expensive?

Actually no.  Users interact for free.  Test is Free.  Consentua for a years subscription or 50,000 consents is only $99.  With 500,000 consents at $949 a year. And 10million consents a bargain at $8999 a year.   Any more than that lets talk! 

A consent interaction from the business will draw down from your consent pool.   This could be a check on the consent of a customer or an update to the consent service.   

## Where do I go to sign up?

Simply use contact@consentua.com







