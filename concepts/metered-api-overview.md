---
title: "Metered APIs in Microsoft Graph"
description: "Provides an overview of metered APIs on Microsoft Graph."
author: "JeremyKelley"
ms.localizationpriority: high
ms.custom: scenarios:getting-started
---

# Metered APIs in Microsoft Graph

Microsoft Graph includes APIs that are both available at no additional cost with service licenses as well as APIs that are metered. Metered APIs incur a cost per API call made.

## Working principles
These are the working principles that guide our approach to Microsoft 365 API endpoints on Microsoft Graph.

Customer Data ownership: Customer data belongs to the customer. Learn more about how Microsoft categorizes customer data. 
Reasonable access: We include access to Customer content, within defined limits, in our user license, and provide developer experiences and documentation focused on cohesion, simplicity, and transparency – around reasonable usage, throttling limits, and pricing. 

Trust: We understand the importance of the trust our developers, partners, and customers place in us. A change to a generally available API would always follow our breaking change policy. 
Ecosystem health: We strive for a balance between platform access and cost to ensure the health of our current and future ecosystem. 

## Categories of services 
With the working principles in place, there are three categories of use cases represented in Microsoft Graph. Note that these categories are useful for illustration but don’t reflect any formal naming or branding. 

Standard: This category includes the broad set of APIs used to perform “CRUD” (create, read, update, delete) operations on customer content and administrative endpoints for service configuration. We continue to define and update the limits of reasonable access based on documented usage thresholds to protect our customer experience and encourage good API usage patterns. Access to this category of APIs within the defined limits is included as part of the user license without any additional costs. This is the default category for most endpoints. 

High-Capacity APIs: We want to ensure that our customers and developers have access to data at scale. This category includes purpose-built, bulk-export services like Teams Export APIs and Microsoft Graph Data Connect, bulk-import capabilities such as Microsoft Graph Connectors, and future bulk export or import endpoints.

Advanced APIs: The third category represents access to data that’s enriched or aggregated by Microsoft or offers access to advanced functionality extended directly from Microsoft 365 infrastructure, Azure Communication Services is an example of this.

## Accessing metered APIs
In order to access metered APIs on Microsoft Graph an application must be associated with an active Microsoft Azure Subscription. For instructions on associating an app to a subscription please see [](metered-api-how-to-cli).

## Developer considerations when using metered APIs
When building an app that leverages metered APIs it is important to remember that metered APIs may return errors related to your subscription status in addition to other more common errors. See [Microsoft Graph errors and resource types](errors.md) for more information on error types in Microsoft Graph.

## Next steps