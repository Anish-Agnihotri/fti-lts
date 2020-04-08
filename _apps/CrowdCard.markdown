---
layout: post
title:  "CrowdCard"
description: >-
  Save restaurants by allowing them to guarantee each other's gift cards in a centralized platform.
category: application
status: "Awaiting decision"
---
# One line summary of the idea.
{{ page.description }}

# Description of product idea: What will the Minimum Viable Product be in 8 weeks? 
## The problem
Due to the quarantine and closure orders, restaurants need cash now that they can pay back later (credit). Many restaurants are trying to crowdfund cash by selling gift cards at a steep discount. However, there is no central online place where these gift cards for local businesses can be purchased. Online stores like Amazon only sell gift cards for national chains. Moreover, because a gift card issued by a bankrupt business is worthless, people are less willing to purchase gift cards from businesses that are likely to go bust. In this way, the restaurants that need the cash the most will likely get the least. Restaurants will go bankrupt and livelihoods will be harmed by this self-fulfilling prophecy.

## The solution
We will create a platform to enable restaurants to co-insure each other’s gift cards. On our platform, you can buy a gift card for restaurant A. If restaurant A goes out of business, you will receive a credit to purchase a gift card from another restaurant on the site. The purpose of this is to increase people's willingness to buy gift cards for struggling restaurants. We believe people would be more willing to help their favorite businesses if their gift card was backed by the services of other restaurants in the system.

Partner restaurants will have the opportunity to get more cash now. In exchange, they will have to provide services to people who purchased gift cards from bankrupt restaurants. However, this is also an opportunity to be first in the door with customers of a recently closed competitor.

We believe that this product has a great opportunity to get off the ground now, and will be a worthwhile platform for specialized restaurant crowdfunding into the future. With some adjustments, the platform could be especially valuable for new restaurants in a post-pandemic setting. Minimum standards would have to be set for businesses wanting to insure their gift cards.

## MVP
In eight weeks, we hope to create the platform with template restaurants so that we can test before adding actual restaurants to the platform. We expect all features of the platform to work including the ability to search based on name and location, the ability to add gift cards to your cart and the ability to pay.

After payment, the user and restaurant will receive an email confirmation of the order. The restaurant will have the ability to get a giftcard to the consumer in any way that they want. They can mail a physical gift card, email a digital gift card, add credit to the user’s account with the restaurant, or allow the user to pick up the gift card the next time they dine at the restaurant (after the quarantine of course).

A few use cases that we hope to implement in our MVP are:

* A user should be able to input the name of a specific local business in the area
* A user should be able to generate a general list of local businesses in their area
* A user should be able to select a restaurant to purchase a gift card from
* A user should see information about the restaurant, perks of gift card purchasal, and message from the owner
* A user should see other co-insured businesses where they can use the gift card in lieu of the current one
* A user should be able to enter a payment amount
* A user should be able to enter payment information
* A user should be able to redirect the gift card to a friend/colleague/family member if they want to
* A user should be able to read and agree to the terms and conditions
* A user should be able to correctly process the payment
* A user’s item should persist in their cart, where they can check out when needed
* A user should be able to access the gift card on their account after purchase
* A user should receive a gift card code, that will be shared with the restaurants
* A restaurant should be able to login into the app using the partner button
* A restaurant should be able to fill out a form to join the local pools of businesses
* A restaurant should see a list of all the customers it has offered gift cards to
* A restaurant should have access to and be able to modify all information available to the customer
* A restaurant should sign an agreement with the app.

# Describe your work plan.
## Competition and customer acquisition
The platform does not have any competitors in the traditional sense. The purpose of the platform is not to displace other sources of credit that restaurants have access to. Rather, we wish to add to the pool of resources that are available. Crowdfunding sites like GoFundMe and other channels to purchase gift cards are alternatives, but not competitors.

We hope that partner restaurants will help promote our services to their customers using direct emails that come from payment platforms (eg. Square) and loyalty programs. We will also try to get media attention. News outlets have run many recent articles about ways that you can help struggling restaurants. Moreover, there may be a lot of gains to centralized promotion efforts through social media.

## Two week milestone
We need to spend the first two weeks researching exactly what is holding customers back from purchasing gift cards and what partners think is important in a platform. We need to figure out how different types of customers differ and how our platform can best serve them. We expect that users run the gambit from altruistic to mercenary. Altruistic users want to help local businesses while more mercenary users are attracted by guarantees and discounts.

To conduct surveys and research trends, we plan on using a lot of Facebook local groups, that already have a concentration of small businesses. Word of mouth is always a great way to know about locals, and we plan on reaching out to users within the United States for our initial MVP. They have a good population of online payment and card users (as opposed to several Asian countries) and will help us localize our MVP.

We will also research ways to co-insure local businesses, and bring immediate relief to them. Lastly, we’ll start building the front-end components of the app that require critical design thinking and user research, and begin initial rounds of A/B testing on low level prototypes of the app, to prevent multiple changes to our app.

## Technologies
### Front-End:
We plan to use React on the front end, due to our team’s familiarity and it’s abundance of packages, that will make getting to the MVP much easier.

### Back-End:
On the back-end, we intend to use Express, Node.js and MongoDB. This will help us create a REST API that will store information of all users, restaurants, gift card purchases etc, in a centralized, persistent database.

### App Specific Features:
* **Payment:** As the backbone of our eCommerce platform, we’ll use [Stripe](https://stripe.com/docs/api) for payment processing. It’s trustworthy design, popularity and ease of use will make it ideal for users to submit their payments, and developers to redistribute payments to the businesses. We are also open to alternative like Snipcart
* **Restaurant retrieval:** We are going to use [Yelp’s API](https://www.yelp.com/developers/documentation/v3/business_search) to get businesses’ data with a specified location. This endpoint returns up to 1000 businesses based on the provided search criteria. It has all the essential information needed for the small businesses we plan on interacting with
* **Location:** To get the user’s location to generate Yelp queries, we will use [Mozilla's Geo-location Api](https://developer.mozilla.org/en-US/docs/Web/API/Geolocation_API). The Geolocation API allows the user to provide their location to web applications if they so desire. For privacy reasons, the user is asked for permission to report location information.
* **Getting Restaurants:** We plan to use Facebook’s Developer API and WhatsApp Plugin to share the post in a Facebook/WhatsApp group to test the demand of a particular gift-card. Facebook Local has a very strong community of people and businesses, where we can advertise our app, and get information about local businesses.
* **Login:** We’ll use react-Facebook-login and react-google-login to keep a list of all the restaurants we’re working with in our MongoDB database.
* **Cart:** We’ll use cookies and tokenizing to store a user’s cart and let it persist, to allow them to checkout at a later time.

## Description and mock-ups
We want our app to be simple, just like our app idea. We intend on having a restaurant facing side of the app and a customer facing side of the app. The customer should be able to search for a restaurant, see perks, and purchase a gift card. A restaurant should be able to partner up with us, inform us of their gift card needs, and maintain a log of customers and liability as to whom they owe services to.

Throughout the app, we’re designing for empathy and trust. A user should be able to purchase the gift cards out of the goodness of their hearts, as they don’t want to see their local stores go under. A user should be able to trust us with their purchase, and know that we will co-insure the gift cards if need be.

We link a [mock-up](/res/CrowdCard/mockup.pdf) and [use-case diagram](/res/CrowdCard/cexp.png).

## Timeline
* **Week 1 - 2:** Market Research, Business Analysis (Basically the stuff we've already written)
* **Week 3 - 4:** Phase 1 development of our app. After finalizing our core features in the first two weeks, we anticipate creating a final mock-up of our application and building it out. We would like to incorporate some essential features such as Search, Restaurant Query and Payment Processing. We will also setup our database schema, and add login auth for the users.
* **Week 5:** User and A/B Testing. As we expect the bones of our app to be constructed quickly with minimal functionality, we would like to test it on a few users who might use this app to find restaurants and invest in gift cards. Some things that we would like to check is whether they trusted the payment process of our app, were they able to find their restaurant with ease and did they receive the gift card via email. This is also when we would like to test out a few potential restaurants, pitch them a mock-up of our app, and adhere to their concerns.
* **Week 6 + 7:** We plan on integrating the changes from user/field testing and adding other core features of our app such as the cart, proper restaurant facing interface, and integrating our APIs
* **Week 8:** After another round of user testing, we'll want to flesh out any minor technical tweaks in our app. However, we anticipate that at this point, we will have a running web application, payment system, and database ready!

# What challenges do you anticipate with this idea?

We worry about rolling it out quickly enough to help restaurants that need it, and worry also about how to get the money to the restaurants without putting ourselves at risk from chargebacks.

Since our app deals with payment, we need to make sure that we’re designing for trust, that users feel safe in giving us their account information and redirect it to small businesses.

While not necessarily a challenge, we expect to discover a lot more opportunities to help restaurants such as selling other goods through the platform and marketing to consumers. 

# Please explain the team's remote working condition.

We will work using Slack and Zoom. It is not possible for us to all meet in one place, and it would not be a good idea either way.

We have been able to work together very well so far despite some time zone differences. We are all available in the morning and at night. Because of classes, these edge times are the most productive hours anyway.