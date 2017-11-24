---
layout: post
title: Consentua Use Case Stories. 
published: true
author: chris_cooper
comments: true
---

 

The following white paper is a description of how Consentua is being used. 

Three use cases are described.  The first is where a consent capture is required as part of a customer re-validation process or acquiring a new customer contact.    The second is using Consentua within an existing app.  The third is where Consentua is being used by a platform as a white label consent management service. 

Each will cover three elements:
* The reason for capturing consent
* The client integration story. Including how Consentua was integrated and the template used. 
* Realised benefits.  


## 1. Consent as part of the customer acquisition process

### Reason for capturing consent.
GDPR demands that citizens give consent in certain scenarios.  One of which is for direct marketing purposes, especially where your data will be shared with 3rd parties.   Another is where for trust and brand reputation reasons a transparent and consented to use of personal data is desired.   

The use case here is for a charity.  They have a desire to capture consent from both existing and new supporters.   For new supporters the consent is captured when they first sign up.  For existing supporters the consent request is emailed and the subsequent consent interaction occurs on a customers view of their existing consent, which needs to be verified.  

The charity has approximately 5000 contacts in their CRM database.   The estimate is around 50,000 consent interactions.   This will cost the charity $99 per year.

### Client Integration Story
The charity are required to make a number of changes to use Consentua.   The web component will be used.  This is applied to the charities web site.    The charity also needs to be able to process the consent data.  This involves granting access to other systems to the charities client consent service.   As well as making sure they only process based on the result returned from Consentua when queried.  
 Consentua uses the same identifier for a user as the requesting system asking for a view of that users consent.   In this use case the supporters email address is used as the common identifier.   

The other aspect is the consent template that the charity is requiring.   Templates are really about scenarios and can be further broken down into purposes.   This use case has only one purpose and a limited number of personal data types.   This results in a binary consent, single purpose consent service.   

### Transaction Flow 
Existing Supporter being emailed. 
Step 1.   Supporter is given a link via email - clicking on this link takes to the user to a consent screen - (which is a popup on the charities web site) 
Step 2.  Supporter can change email address or inherit one from email and then grant consent 
Step 3.  Consent popup sends the now  agreed to consent request to Consentua.  This creates a unique consent receipt per that user identifier 
Step 4.  Charity systems can ask Consentua via the API who has consented to what or what has this user consented too.  

### New Supporter 
Step 1.  Supporter goes to website - encouraged to provide some details - <<<click here>>
Step 2.  Consent screen pops up - capture email from user and get consent for personal data required
Step 3. As per above. 

### Benefits Realised
The charity were able to deploy Consentua with ease and have been able create consent receipts for all supporters both old and new.    Total cost to the charity was $99, plus the internal effort of using the web component and querying the API via other systems - (estimate at 2 days development and testing time).  

### Total benefits: 
GDPR compliant
Clear consent statement from supporters
Flexibility for future needs already built in. 

## 2. Established mobile app

### Reason for capturing consent
This particular application uses a number of personal data types in its operation.   The app is available on both iOS and Android.    The need to capture consent is because of the multiple purposes for which personal data is used.   Due to a relatively high churn rate (20%) the data controller can never assume consent is granted at all times.  

This app collects personal data on location, sentiment, age, gender and occupation.  The data is shared with numerous parties, albeit in an anonymised form.  The data is used to influence other outcomes and the results are displayed in a public place.   Users are interacted with on a daily or at a minimum a weekly basis.  

The app has a few thousand users, however the interaction count is very high.   Therefore the cost to the customer is $899 per year for 500,000 consents.    

### Client Integration Story
The primary user interface is via a mobile.  So a new app update is shipped with the Consentua SDK deployed in that update.   When the user goes to the new consent view, which can be auto pop-up or via push notification they will start interacting with Consentua.  

On the clients backend a new check is made prior to personal data processing to check Consentua that all users in scope are consenting to that interaction. 

The consent template is broken into two categories, the first is realtime data and outcomes.  The second is historical data used for analysis and prediction.     The first is a linear purpose group the second is a binary purpose group.  

### Transaction Flow 
Step 1.  User receives notification to check consents
Step 2.  Launches Consent view which kicks off a request to Consentua.
Step 3a.  If a new user, Consentua creates them and awaits their saved consent settings. 
Step 3b. If an existing user Consentua retrieves the last save consent setting and displays this.
Step 4.   App management tool can now see who has consented to what via Consentua API.

### Benefits Realised
The customer has a transparent description of how personal data is used and applied, which end users appreciate and trust.  The enablement of the consent receipt for others to access has been of benefit from a later research perspective.   As a new 3rd party could be added and the new consent request updated in realtime.  With no further code updates or app releases required.  This flexibility alone paid for Consentua.  

Cost to this client:  $899 for 500,000 consents per annum.    Plus the internal effort of using the mobile app SDK’s and set up the querying job to the API for other systems - (estimate at 4 days development and testing time).  

### Total benefits: 
GDPR compliance swiftly enabled
Quick & easy to deploy API & SDK
Clear & transparent consent statement from users builds trust.
Flexibility for future needs already built in.  
 


## 3. As a component in a platform (via white label).  

### Reason for capturing consent
This customer has a platform that supports many different other companies.    These customers use this platform as a one stop shop for customer contact and engagement.   These customers expect the platform to be GDPR ready.   

The platform will be creating campaigns for direct marketing specific brands to certain audiences.   Customer acquisition and personalisation are key to these brands so knowing customers better is a primary objective. 

The personal data will be shared with 3rd parties, but the benefits the customer receives as a result need to transparently articulated.    This build trust in these brands.  

### Client Integration Story
The platform systems integration team are using the web component and a dedicated set of consent templates.   These are then assigned to a specific campaign, which is then emailed to customers/prospects.  

Once the consent receipt for the user is safely stored in Consentua.  The campaign management tools in the platform can now ask Consentua for details on which customers have consented to a particular campaign.   

The consent template is relatively simple.  With one purpose and two data types.  This equates to a double binary consent template. 


### Transaction Flow 
Existing Customer being emailed. 
Step 1.  Customer is given a link to a campaign via email - clicking on this link takes the user to a consent screen - (which is a popup on the campaign web site) 
Step 2.  Customer can then grant consent, as well as add additional data to their profile. 
Step 3.  Consent popup sends the now  agreed to consent request to Consentua.  This creates a unique consent receipt per that user identifier 
Step 4.  Campaign management tool on the platform can now ask Consentua via the API who has consented to what or what has this user consented too.  

### Benefits Realised
Multiple.   From the platforms perspective they have a fast path ready made consent service running under their brand.  Their customers have a GDPR ready consent management capability at there fingertips.   

Time to deployment of new consent services is rapid.  A 10minute task to create a new campaign template, service and assign users.   

The total cost to the platform for Consentua is $8999 per annum as the number of consents is going to be near 10 million per annum.   

### Total benefits: 
GDPR compliance swiftly enabled
Quick & easy to deploy API 
White label SaaS offering.  My brand but none of the cost of developing.  
Flexibility for future needs already built in.  
 
