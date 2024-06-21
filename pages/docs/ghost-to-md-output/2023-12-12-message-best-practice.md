---
title: MoeGo SMS Message Best Practice
slug: message-best-practice
date_published: 2023-12-12T01:49:46.000Z
date_updated: 2023-12-14T16:31:58.000Z
tags: Messages
---

In the dynamic landscape of messaging, the challenge of ensuring secure and clear communication is a collective effort involving carriers, SMS service providers, and users like yourself. At MoeGo, we understand the frustration that arises when messages encounter filtering, sometimes disrupting your communication with clients.

While MoeGo has been actively engaging with our partners in ongoing communication regarding these filtering concerns, it's crucial to acknowledge that **the****decision on which words are filtered ultimately lies with the carriers and our SMS service provider Twilio**. 

In this guide, we'll clarify the roles of **carriers** and MoeGo's SMS service provider **Twilio** in shaping safe and effective messaging communication on MoeGo. We will then provide practical insights for crafting messages that align with industry standards, avoiding mistakenly filtered word cases and URL restrictions.

## Understanding the Industry Standard of Message Filtering

The intricacies of message filtering often stem from industry standards set by carriers and SMS service providers. 

Mobile carriers, the foundational pillars of mobile communication, implement stringent guidelines to ensure a secure and compliant messaging environment for users. Carriers are entrusted with the responsibility of regulating message traffic to safeguard users from unwanted or potentially harmful content. These regulations often include restrictions on certain types of messages or content deemed inappropriate, in adherence to the regional or global standards. As a result, messages passing through carrier networks undergo scrutiny to maintain a safe and reliable communication ecosystem.

The guidelines established by mobile carriers set the stage for how SMS service providers like **Twilio** implement content moderation. By establishing a framework for acceptable messaging practices, carriers contribute to fostering a secure and standardized messaging experience for users across diverse platforms.

You may also wonder why the same SMS can be sent from your personal phones but not within MoeGo. This distinction arises from the different classifications of messages: A2P (Application-to-Person) for business messages and P2P (Person-to-Person) for personal messages. **Business messages (A2P) **are subject to more restrictions, ensuring compliance with industry standards and regulations, which may lead to variances in message delivery experiences between personal devices and the MoeGo platform. Understanding this difference is crucial for adhering to the guidelines governing business messaging.

## Best Practices for Safe and Effective Messaging

In the realm of messaging best practices, it is essential to recognize that certain words may trigger content filters established by carriers and SMS service providers, leading to message restrictions. 

### 1. Alternative Expressions for Commonly Filtered Words

In the pet industry setting, specific terms like "anal" and "CBD" have been identified as commonly filtered words due to compliance issues. For a smoother messaging experience, consider alternative expressions such as substituting "anal" with "gland" and replacing "CBD" with terms like "pain relief oil" or "soothing oil" for users in regions where CBD products are legal. This proactive approach ensures your communication aligns with industry standards, minimizing the risk of message interception. 

### 2. Navigating URL Restrictions

According to the general expectations from US carriers, short links created by Public URL shorteners could be identified as spam and be filtered. Carriers are currently blocking non-compliant URLs like "[goo.gl](http://goo.gl/)" and "[bit.ly](http://bit.ly)". 

If you would like to use a shortened link, it should include the following components: 

- **proprietary** – a dedicated custom domain that belongs to your business, not a free shared public link shortener
- **properly branded** – the domain aligns with the message sender identified in the text message itself

You can read more about how to send short links in [this Twilio guide](https://support.twilio.com/hc/en-us/articles/1260804572090-How-can-I-send-shortened-links-in-my-messages-).

In general, we **recommend sending the full link** to your customers, although it's not ideal for your customer's reading experience. 

### 3. Restricted Message Categories

Delving deeper into messaging best practices, it's crucial to be aware of restricted message categories outlined by carriers and SMS service providers. Highlighted within these categories are specific content types that may lead to message restrictions. While we provide an overview here, it's important to note that **the detailed regulations can vary by region and country**. We recommend referring to [Twilio's detailed guidelines](https://support.twilio.com/hc/en-us/articles/360045004974-Forbidden-Message-Categories-in-the-US-and-Canada-Short-Code-Toll-Free-and-Long-Code-) on message categories that may lead to restrictions. Below are three of the most relevant categories:

**Illegal Substances/Articles**

*Examples:* Cannabis, CBD, Vape/E-cigs, Fireworks

Businesses involved in cannabis, CBD, Kratom, or drug paraphernalia products are not recommended from utilizing SMS/MMS messaging on Twilio in the US and Canada, irrespective of the content. These restrictions persist regardless of federal or state legality. All use cases for these entities are disallowed from sending SMS, even if the content does not explicitly involve cannabis. 

**Third-Party Lead Generation Services and Marketing**

*Examples:* Companies, NGOs, or political campaigns engaged in buying, selling, or sharing consumer information. 

Third-party lead generation services and marketing activities are not recommended. Consent must be directly obtained from end-users; any third-party use cases are not recommended. Political use case customers sending SMS messages are not permitted to use voter registration databases for consent collection and outreach to end-users. Additionally, businesses with terms of service or privacy policies mentioning sharing or selling consumer data/opt-in information are considered noncompliant.

**High-risk financial services**

*Examples*: Payday loans, Short-term high-interest loans, New loan soliciting, Third-party loans, Student loans, Cryptocurrency, Stocks and investing platforms

Businesses exclusively dealing in stocks, investing, or cryptocurrency are restricted from sending SMS traffic. However, exceptions may apply for mixed-use cases, where approval depends on the overall content and purpose beyond these high-risk financial components. Promotional messaging for first-party loans is not permitted. Third-party loans encompass auto, mortgage, personal, etc., originating from entities other than the servicing party.
