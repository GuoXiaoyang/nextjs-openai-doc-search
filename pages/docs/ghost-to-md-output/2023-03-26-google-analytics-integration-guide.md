---
title: Google Analytics Integration Guide
slug: google-analytics-integration-guide
date_published: 2023-03-25T23:59:21.000Z
date_updated: 2023-03-25T23:59:21.000Z
tags: 07. Online booking
---

### Get your MEASUREMENT ID from Google analytics

GA4 for example:

Create a new property for MoeGo online booking(or you can add booking.moego.pet to your existing data stream domain configuration)

1. Create property
2. Create data stream (web, booking.moego.pet as domain)
3. Copy MEASUREMENT ID

0:00
/
1&#215;

## Config it into MoeGo online booking settings

Paste your MEASUREMENT ID into Online booking settings:
![](__GHOST_URL__/content/images/2023/03/fe3d9137-b2bf-4efe-a9de-8e371785dc27.png)
# Set up your report

You can explore and set up analytics report based on data collected by your GA ID.

Let’s take funnel report by page path for example.

Page path for key steps in booking flow:

Start booking - `/ol/book`

Select service - `/ol/service/choose`

Select groomer - `/ol/groomer/choose`

Select time - `/ol/time`

Submit booking - `/ol/appointment/submitted`

0:00
/
1&#215;
