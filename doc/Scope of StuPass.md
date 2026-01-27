# Scope of StuPass

## 1. Statement of Context

**What StuPass IS:**
> StuPass is a specialized Consumer-to-Consumer (C2C) mobile marketplace designed exclusively for university students. It facilitates the exchange of academic materials (textbooks, electronics) and personal items within a trusted, closed-network environment. The platform focuses on two primary interaction models: direct physical exchange (pay offline) and secure digital transaction (pay online).

**What StuPass IS NOT:**
> StuPass is not a general-purpose e-commerce platform for professional retailers or businesses. It does not handle logistics, shipping, or third-party delivery services. It is not a social media platform; communication features are strictly functional to facilitate trade.



---

## 2. In-Scope Functionalities (MVP)

### A. User Profile & Trust
* **Student Verification:** Implicit authentication mechanisms to ensure users are valid students.
* **Profile Management:** Capability for users to update personal details (Bio, Contact Info).
* **Reputation System:** A rating and review mechanism allowing buyers and sellers to score each other after interactions.

### B. Inventory & Marketplace
* **Inventory Management:** Sellers can add and edit item details (Images, Price, Description, Category) in their personal storage.
* **Internal Search:** Sellers can search within their own inventory.
* **Discovery Engine:** Buyers can search the global marketplace and apply filters (Price, Category) to refine results.

### C. Communication Hub
* **Direct Messaging:** One-on-one text and media messaging between Buyer and Seller.
* **Group Collaboration:** Capability to create group chats for class-based or club-based trading.
* **Real-time Communication:** Integrated Video Call feature for product inspection or verification.
* **Inbox Management:** Ability to archive or hide inactive conversations.

### D. Transaction & Logistics
* **Offline Coordination:** Tools to assist physical meetups, including Location Sharing and Meeting Scheduling.
* **Online Payment:** Integration with a payment gateway to process secure online transfers for items.

---

## 3. Out-of-Scope Functionalities (Deferred/Discarded)
The following features have been explicitly considered and excluded from the MVP scope to reduce complexity and adhere to the project constraints.

* **Automated Dispute Resolution (Refunds):** As Request Refund (P-16) was removed, the system will not support an automated refund workflow. Disputes must be handled manually via external support channels.
* **Manual Publishing Workflow:** As Publish Listing (P-06) was removed, there will be no draft/preview mode. Items added to storage are either immediately live or managed via a simplified toggle, removing the need for a complex publishing wizard.
* **Integrated Logistics/Shipping:** The system relies entirely on user-coordinated meetups (Offline) or user-arranged shipping. There is no integration with delivery services (e.g., GrabExpress, AhaMove).
* **Bidding/Auctions:** The marketplace operates on a fixed-price model. Auction-style bidding capabilities are excluded.
* **Guest/Anonymous Access:** Unregistered users cannot view listings or interact with the app. Strict student authentication is required for all access.
* **Shopping Cart:** As a C2C platform focusing on individual items, there is no "Cart" functionality for accumulating items from different sellers into a single checkout. All transactions are direct single-item or negotiated bulk purchases.