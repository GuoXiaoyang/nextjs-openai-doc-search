---
title: MoeGo Processing Fee by Client - Add Surcharges Easily for Credit Card Payments
slug: add-a-convenience-fee-for-credit-card-payments
date_published: 2024-03-03T12:27:00.000Z
date_updated: 2024-03-25T08:12:17.000Z
tags: What's new in MoeGo, 💳 MoeGo Pay
---

The processing fee can be easily added to the invoice at checkout in MoeGo. This will greatly optimize your expenses and allow you to have the flexibility to share the cost with your customers.

## How does it work

The processing fee consists of two parts for each transaction, both of which can be passed on to the client's side: 

1. A percentage
2. A fixed amount 

***Once the fee rate is configured, the exact fees for transactions will be calculated automatically and ready to be applied at checkout.**

💡**Please note:** Credit card surcharge permissions may vary by state, regulatory, or card network rules. It is your responsibility to meet all legal and card network requirements by using this feature.

- **Check your local laws** to make sure your business can transfer the processing fees to clients.
- **Contact a tax professional or your local government** for further guidance on whether your area permits surcharges.

---

## Setting up Processing Fees by Client

**🖥️Desktop:**

To set up processing fees to be paid by the client using the desktop, simply:

1. Go to **< Card processing >** on the side menu bar
2. Select **< Edit >** next to **Credit card processing fee**
3. Elect the fees to be** paid by < Clients >**
4. Sign the **Agreement**
5. Set the** < Fee name on invoice >**
6. Set up the processing fee rates
1. 💡 It is highly recommended to set these fees based on the rates that Stripe charges with MoeGo Pay

7. Set the calculation method to be either:
1. **Earn full ticket amount** (default option: all the processing fees will be covered by the clients)
2. **Charge clients the processing rate displayed above** (the business will still cover a small portion of the processing fee)

8. Switch **< Exclude passing fees to debit card transactions toggle > **on/off
1. 💡 **Please note: **Debit Card transactions are prohibited from being surcharged by some of the credit card networks. By enabling this option, the processing fees paid by clients will not be applied to **debit card transactions.**

![](__GHOST_URL__/content/images/2023/08/Frame-427319931.png)Locating the Credit card processing fee settings![](__GHOST_URL__/content/images/2023/08/Frame-427319933.png)Customizing the name of the fee on the invoice
**📱App:**

To set up processing fees to be paid by the client using the app, simply:

1. Go to **< Settings >** on the side menu bar
2. Select **< MoeGo Pay >** and choose **< Credit card processing fee >**
3. Elect the fees to be** paid by < Clients >**
4. Sign the **Agreement**
5. Set the** < Fee name on invoice >**
6. Set up the processing fee rates
1. 💡 It is highly recommended to set these fees based on the rates that Stripe charges with MoeGo Pay

7. Set the calculation method to be either:
1. **Earn full ticket amount** (default option: all the processing fees will be covered by the clients)
2. **Charge clients the processing rate displayed above** (the business will still cover a small portion of the processing fee)

8. Switch **< Exclude passing fees to debit card transactions toggle > **on/off
1. 💡 **Please note: **Debit Card transactions are prohibited from being surcharged by some of the credit card networks. By enabling this option, the processing fees paid by clients will not be applied to **debit card transactions.**

![](__GHOST_URL__/content/images/2023/08/Frame-427319935.png)Locating the Credit card processing fee settings![](__GHOST_URL__/content/images/2023/08/Frame-427319936.png)Signing the Agreement![](__GHOST_URL__/content/images/2023/08/Frame-427319937.png)Customizing the name of the fee on the invoice
## FAQ

**Q1. Which card processor does it support?**

**Answer:** Processing fees paid by clients is currently only available with MoeGo Pay as the primary card processor.

**Q2. What should I set for the processing fee rate when setting up to pass the fees to be paid by the client?**

**Answer:** Feel free to customize the convenience fee rate to suit your needs. However, it's strongly advised to align it precisely with the fee charged by the processor to prevent any confusion. 

Stripe charges may fluctuate depending on payment methods for each transaction. Should different fee rates apply to your plans, please reach out to support for assistance.

- 2.9% plus 50 cents with a card present for Stripe reader, tap to pay
- 3.4% plus 30 cents without a card present for the online invoice, card on file, enter card info

![](__GHOST_URL__/content/images/2023/08/Frame-427319934.png)
**Q3. Is it available in all regions?**

**Answer:** Processing fees by clients is currently available in the permitted states of the United States and Australia.

**Q4. Can it be applied to debit cards?**

**Answer:** Debit card transactions are prohibited from being surcharged by some of the credit card networks (Visa, Mastercard, etc,.). Implementing convenience fees on debit card transactions poses a risk of being restricted by credit card issuers. Therefore, it is advisable to carefully consider whether or not to enable the "Exclude passing fees to debit card transactions" option.

**Q5.  In what case there will be slight differences in the amount:**

**Answer: **If the processing fee is paid by clients, technically it acts as a surcharge on the invoice. Therefore, Stripe will also take processing fees based on that on their end.

For example, if the client pays $1 for the fee, Stripe charges that $1 for processing.

**Q6. How are the processing fees on the tips charged?**

**Answer:** The tips added from the clients' end will not be included in the processing fee charged to clients.

To be more specific, after sending the invoice to a client, if the client adds a tip at their end, the processing fee based on the tip will not be covered by the client at this moment. In this case, the number could be slightly different when it involves tips in the invoice.

If you had added the tip before sending out the invoice, then the clients would have covered the fee for tips as well.

**Q7. Can the staff remove the processing fee by the client at checkout?**

**Answer:** It depends on whether or not the business owners have granted this access to the staff. The owner can go to role permission to set it up.
