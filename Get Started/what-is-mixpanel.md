---
title: "What Is Mixpanel?"
slug: "what-is-mixpanel"
hidden: false
metadata: 
  title: "What is Mixpanel? | Mixpanel Documentation"
  description: "Explore Mixpanel's documentation to learn about product analytics, implementation, data structure, cohorts, SDK integrations, and more."
createdAt: "2021-04-16T19:30:56.811Z"
updatedAt: "2021-05-10T23:50:46.270Z"
---
Mixpanel is a product analytics tool that enables you to capture data on how users interact with your digital product. Mixpanel then lets you analyze this product data with simple, interactive reports that let you query and visualize the data with just a few clicks.

Our self-serve interface empowers your team to answer questions, no matter their data expertise.
<p align="center">
    <img src=https://storage.googleapis.com/cdn-mxpnl-com/static/readme/Dashboard.svg>
</p>

##Introduction to the Data Model
Analytics tools often track engagement in the form of page views and browser sessions.

Mixpanel instead relies on a different, more powerful data model to track in-product interactions. We call this "event-based" tracking, and it enables much deeper analysis of user behavior.

The event-based model is built on three key concepts: **Events**, **Users**, and **Properties**.

###Events
An event is a data point that represents an interaction between a user and your product. Events can be a wide range of interactions. For example, every time a customer purchases a coffee from your café app, there are details that describe the purchase the moment it happens. Actions like purchasing a coffee can be tracked as an event in Mixpanel.

<p align="center">
    <img src=https://storage.googleapis.com/cdn-mxpnl-com/static/readme/Event.svg>
</p>

###Users
On the other side of an event is a user — the specific individual that completed an interaction with your product.

Because each user is unique, Mixpanel tracks which users completed what events and marries the two distinct data points by joining them.
`event.distinct_id = user_profile.distinct_id`

<p align="center">
    <img src=https://storage.googleapis.com/cdn-mxpnl-com/static/readme/Users.svg>
</p>

###Properties
Properties are attributes that help you define the specifics of an **Event** or a **User**.

As the name suggests, an **Event Property** describes an event. For a coffee purchase, the event would be Purchase and the event property could be *Item Type* (in this case a Coffee) or *Item Price* (in this case $2.50)

<p align="center">
    <img src=https://storage.googleapis.com/cdn-mxpnl-com/static/readme/Event_Property.svg>
</p>

A **User Property** on the other hand provides details on a User. This could be something as simple as a user's name or age, or something more nuanced, like their most frequently ordered item.

<p align="center">
    <img src=https://storage.googleapis.com/cdn-mxpnl-com/static/readme/User_Property.svg>
</p>

[Mixpanel's different reports](https://mixpanel.com/behavioral-analytics/) allow you to view data about various users or events and slice and dice that data by any property.