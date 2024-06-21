---
title: Dispute Notification
slug: dispute-notification
date_published: 2024-02-25T03:13:05.000Z
date_updated: 2024-02-26T07:45:32.000Z
tags: 💳 MoeGo Pay
---

The Dispute Notification feature is designed to improve the merchant experience by ensuring better tracking and management of disputes, which is crucial for minimizing losses and protecting income. This features is available on both the Desktop Web Version and the MoeGo App.

Key highlights of the Dispute Notification feature include:

- **Enhanced Notifications:** Introduction of general alerts and specific notifications for card processing disputes to ensure merchants are promptly informed.
- **Improved Dispute Handling:** Revision of dispute and inquiry statuses, along with detailed hover descriptions, for a clearer understanding of their progress.
- **Advanced Dispute Tracking:** Inclusion of a date picker and status filter in the dispute list for streamlined management of disputes.

## 💻 Desktop

### Check for Disputes in Notifications

When a dispute happens, there will be a dispute notice in **Notifications (Bell Icon) > Activity** in the top right of the toolbar.

- Click on the notification to go straight to the **Dispute Page**, or
- Click **< Dismiss >** to mark the notification as "Read".

![](__GHOST_URL__/content/images/2024/02/CleanShot-2024-02-26-at-02.19.43-1.gif)
### Check for Disputes in Transaction Activity

You can also go to **Card processing > Transaction activity > Dispute** to check for dispute information and status.

- If you see a red dot on the Transaction activity, it means there is a dispute. 
- When accessing the dispute details page from either the App or Web Version, the notifications on the other end will disappear and be marked as "Read".

![](__GHOST_URL__/content/images/2024/02/CleanShot-2024-02-26-at-02.22.43-1.gif)
### Filter for Disputes based on Time and Status

To view a certain set of disputes based on the **time** or **status**, you can go to **Card processing > Dispute**. 

**Time filter**

The date filter is defaulted as Year-to-date, you can choose other conditions, such as This week, Month-to-date, Last quarter, or directly set a Custom date range.
![](__GHOST_URL__/content/images/2024/02/CleanShot-2024-02-26-at-02.25.37.gif)
**Status filter**

The status filter is defaulted as All status. You can choose other conditions, such as Evidence processing, Evidence submitted, Won, Lost, etc. If you would like to submit additional evidence, they can click on **< Contact support > **in the tooltips to contact our 24/7 customer support team to submit the evidence.
![](__GHOST_URL__/content/images/2024/02/CleanShot-2024-02-26-at-02.28.15.gif)
### Understanding Dispute Status

To view the status of disputes, go to **Card processing > Dispute**, and find the Status column.
StatusDefinition![image-20240122-073322.png](__GHOST_URL__/content/images/2024/02/image-20240122-073322-1.png)This status indicates that a dispute transaction has occurred, and the MoeGo Pay team is currently gathering evidence to prepare for uploading and countering the dispute.![image-20240122-073755.png](__GHOST_URL__/content/images/2024/02/image-20240122-073755-1.png)This status indicates that the evidence has been uploaded to the Stripe platform and is awaiting processing and decision by the issuing bank.![image-20240122-074103.png](__GHOST_URL__/content/images/2024/02/image-20240122-074103.png)This status represents that the issuing bank's decision on this dispute transaction is "Business won," and the payment will be returned to you, the business owner.![image-20240122-074117.png](__GHOST_URL__/content/images/2024/02/image-20240122-074117.png)This status indicates that the issuing bank's decision on this dispute transaction is 'Business lost,' and the dispute will be upheld in favor of the card owner.![image-20240122-074127.png](__GHOST_URL__/content/images/2024/02/image-20240122-074127.png)This status indicates that an inquiry to the transaction has occurred, and the MoeGo Pay team is currently gathering evidence to prepare for uploading and countering the inquiry.![image-20240122-074135.png](__GHOST_URL__/content/images/2024/02/image-20240122-074135.png)This status signifies that the evidence has been uploaded to the Stripe platform and is awaiting processing and decision by the issuing bank.![image-20240122-074150.png](__GHOST_URL__/content/images/2024/02/image-20240122-074150.png)This status indicates that the inquired transaction has been closed by the issuing bank and won’t be escalated to a dispute.
# 📱App

### Check for Disputes in Payment Settings

When a dispute happens, there will be a red dot in your** Notification > Payment > Dispute tab**.
![](__GHOST_URL__/content/images/2024/02/Dispute-Notification---App---Notification.png)
### Get In-App Notifications for Disputes

When a dispute happens, there will also be a push notification to your mobile phone. You can click on the notification to go to the Dispute page.
![](__GHOST_URL__/content/images/2024/02/CleanShot-2024-02-22-at-01.25.50@2x.png)
### View Disputes List

You can also access a dispute transaction by going to **Payment settings > MoeGo Pay > Transaction history > Dispute.**
![](__GHOST_URL__/content/images/2024/02/Dispute-Notification---App---View-Dispute-List--1-.png)
You can view the list of disputes in this Dispute tab. The information icon is to help you access the wiki article about Disputes, and also more support in every stage of the dispute.

### Filter for Disputes based on Time and Status

Similar to the Web Version, you can view a certain set of disputes based on the **time** or **status **on the app by going to **Payment settings > MoeGo Pay > Transaction history > Dispute.**

In this tab, you can click on Filters to select the time range and status conditions.
![](__GHOST_URL__/content/images/2024/02/Dispute-Notification---App---Filters--1-.png)
# Frequently Asked Questions

**Q: How does the counter-dispute process work in MoeGo?**

**A:** In MoeGo, the support team actively gathers necessary evidence and submits it on your behalf to counteract disputes. Typically, banks decide within 1-2 months. You can track the status of disputes through the path **Payment settings > MoeGo Pay > Transaction Activity > Dispute **on the App or **Card processing > Transaction activity > Dispute** on the Desktop Web Version. The evidence includes service details, receipts, your communication with clients, and signed agreements. You're encouraged to provide any additional evidence that may support your case.

**Q: What exactly is an inquiry?**

**A:** An inquiry is a preliminary step some card networks take before proceeding to a formal dispute and chargeback. This phase, referred to as an "inquiry," "retrieval," or "request for information" by Stripe, is commonly used by American Express and Discover. Mastercard and Visa no longer utilize this phase. It involves the cardholder's bank seeking clarification on a transaction, often because the cardholder does not recognize the transaction details. Resolving an inquiry effectively, either by providing sufficient evidence to address the dispute or by issuing a full refund, can prevent a dispute fee. Note that inquiries on transactions that have been partially refunded may still escalate to a chargeback.
