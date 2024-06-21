---
title: MoeGo Pay Pre-authorization
slug: moego-pay-pre-authorization
date_published: 2023-10-18T07:24:19.000Z
date_updated: 2024-03-08T08:47:03.000Z
tags: 💳 MoeGo Pay
---

MoeGo Pay Pre-auth is a recently introduced payment processing pattern. It allows you to validate and hold the full ticket price before the service date. Once the service is completed, you can charge the reserved amount during checkout. Additionally, we offer automatic capturing of authorized funds at the end of the service day.

0:00

                            /0:12
1×

## **Who is eligible to use MoeGo Pay Pre-auth?**

MoeGo Pay Pre-auth is available for all MoeGo Pay users. If you are not currently a MoeGo Pay user, you can refer to [**MoeGo Pay Overview**](__GHOST_URL__/moego-pay-overview/) for a general introduction to MoeGo Pay.

## **What is your customer's experience?**

Once MoeGo Pay Pre-auth is enabled, the following is the charging process for appointments with a card on file:

- 24 hours before the appointment, your customer will notice a hold for the full ticket amount on their selected payment method.
- After the service is completed, they will see that the on-hold amount has been captured, either at the time of checkout or by the end of the service day.
- If the service is canceled, they should expect the authorized amount to be released shortly.

## **How to enable MoeGo Pay Pre-auth**

You can enable MoeGo Pay to preauthorize by 3 methods: 1. apply to all requests in Online Booking, 2. apply to selected clients' requests in Online Booking, 3. apply to specific appointments.

It isn't possible to complete these settings on the app directly, but you can go into **app version** > **<Settings>** > **<Online Booking>** > **<Go to Web version> to **perform the same steps on a web browser. It is still recommended to change these settings on a desktop since user experience is not optimized for a  mobile-device web browser.

### **1. Enable it for all Online Booking requests**

- Go to **Online Booking > Settings > Payments > Payment Requirements**.
- Select** < MoeGo Pay Pre-auth>**.

![](__GHOST_URL__/content/images/2024/01/CleanShot-2024-01-04-at-12.10.58.gif)
### **2. Enable it for Online Booking requests by selected clients**

- Go to **Online Booking > Settings > Payments > Customized Payment Options by Clients**.
- Select a client group/client groups. You can choose from **< New Visitors > **and/or** < Existing clients with filters >**.
- Select** < MoeGo Pay Pre-auth>**.

0:00

                            /0:25
1×

When enabling Pre-auth in Online Booking, you can choose to enable tipping or edit the cancellation policy based on your needs.

- Enable tipping: When turned on, customers will be prompted to select a tip rate before submitting their booking requests.
- Cancellation policy: You can customize your cancellation policy while pre-authorization is enabled, and it will be displayed to customers before they submit their booking requests.

Once enabled, the selected customer group will be required to provide their card information before submitting a booking request via online booking. They will also receive a notification that a full ticket amount authorization will be placed on their selected payment method 24 hours prior to the appointment start time.

### **3. Enable it by specific appointment**

**Desktop**

To enable Pre-auth only for specific clients, such as those with a history of no-shows, you can toggle on the **<MoeGo Pay Pre-auth>** option on the appointment detail page. This option is available both on the app and on desktop.
![](__GHOST_URL__/content/images/2023/10/image.png)![](__GHOST_URL__/content/images/2024/03/CleanShot-2024-03-08-at-4.16.10@2x.png)
If the selected client does not have a card on file, we will send them a link to collect their card information before executing the Pre-auth. This is possible on a desktop only. 
![](__GHOST_URL__/content/images/2023/10/CleanShot-2023-10-18-at-22.24.58@2x.png)
## **How to checkout pre-authorized appointment**

For the pre-auth'ed appointment, you can perform the checkout and take payment as usual, and the authorized fund will be captured along the way. What’s even better, if you were too busy to take payment, the pre-authorized amount will be automatically captured by the end of the service day.

### **Capturing funds during checkout**

For pre-authorized appointments, since we have already determined and authorized their payment method with the corresponding funds, you can proceed directly with charging the selected card to capture the amount.

### **Capture automatically at the end of the service day**

For pre-authorized appointments that have not been paid during checkout, we will automatically capture the final ticket amount from the pre-authorized card by the end of the service day. This will be based on the timezone set in your business settings.

## **Frequently asked questions**

**Q: What happens if pre-authorization fails?**

A: You will receive a notification when pre-authorization fails. After the authorization fails, you can go to the appointment detailed page. From there, you can either retry pre-authorization using the same card or switch to another payment method and attempt pre-authorization again.

**Q: What if the final ticket total is different than the pre-authorized fund?**

A: If the final ticket cost exceeds the preauthorized amount, we will attempt to capture the full amount using the same payment method with the holding funds during checkout. If the selected payment method does not have sufficient funds, you will have the opportunity to switch payment methods and proceed with checkout as usual.

If the final ticket cost is less than the preauthorized amount, we will only capture the actual ticket amount and automatically release the remaining funds.

**Q: How long will the on-hold amount get released if the appointment gets canceled?**

Usually, it takes less than one business day, but depending on the processing bank, it might take up to seven business days.

**Q: What if I forget to check in and/or check out the appointment on the day? Do I still get paid?**

A: Yes, the pre-auth'ed amount will still be charged at the end of the service day. You may need to charge the client again if he/she wishes to tip you.  

**Q: Can I reverse the Pre-authorized amount if my client wants to pay in a different payment method on the day of service? **

A: For manually created appointments, you can toggle off the **<MoeGo Pay Pre-auth> **Button 24 hours before the schedule appointment time. But once the amount has been pre-authorised which is generally the case on the day of service, there isn't a way to reverse it. The only way will be to cancel that appointment and create another apppointment. . 

For Online bookings submitted with pre-auth, you cannot modify the payment method at any point after confirming the booking request. Please cancel the appointment and create a new one. 
