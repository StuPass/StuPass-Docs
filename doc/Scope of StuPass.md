# Scope of StuPass

## 1. Statement of Context

**What StuPass IS:**
> StuPass is a specialized Consumer-to-Consumer (C2C) mobile marketplace targeted toward university students. It facilitates the exchange of unused personal items. StuPass focuses on creating a platform to streamline the discovery of affordable second-hand goods within a verified campus network. It functions primarily as a listing directory and introduction service, bridging the gap between student buyers and sellers to arrange independent, offline transactions.

**What StuPass IS NOT:**
> StuPass is not a general-purpose e-commerce platform for professional retailers or businesses. It does not handle logistics, shipping, or third-party delivery services. It is not a social media platform; communication features are strictly functional to facilitate trade. It does not process payments, hold funds, or facilitate digital transactions. It is not a multimedia communication platform; messaging is restricted to text-based coordination.

---

## 2. In-Scope Functionalities (MVP)

### A. Authentication & Access Control

* **User Registration:** Users can sign up using supported methods (Email/Phone, Google).
* **User Login:** Registered users can sign in securely to access system features.
* **Session Management:** The system maintains authenticated sessions and supports user sign-out.
* **Password Recovery:** Users can reset or change passwords through a secure recovery mechanism

### B. User Profile & Trust
* **Student Verification:** Implicit authentication mechanisms to ensure users are valid students.
* **Profile Management:** Capability for users to update personal details (Bio, Contact Info).
* **Reputation System:** An automatic rating mechanism based on reports from users.

### C. Inventory & Marketplace
* **Inventory Management:** Sellers can add and edit item details (Images, Price, Description, Category) in their personal storage.
* **Internal Search:** Sellers can search within their own inventory.
* **Discovery Engine:** Buyers can search the global marketplace and apply filters (Price, Category) to refine results.

### D. Communication Hub
* **Direct Messaging:** One-on-one text and media messaging between Buyer and Seller.
* **Group Collaboration:** Capability to create group chats for class-based or club-based trading.
* **Real-time Communication:** Integrated Video Call feature for product inspection or verification.
* **Inbox Management:** Ability to archive or hide inactive conversations.

---

## 3. Out-of-Scope Functionalities (Deferred / Discarded)

The following functionalities were deliberately excluded from the MVP to reduce implementation complexity, maintain focus on core objectives, and comply with project constraints.

- **Automated Dispute Resolution and Refunds:**  
  The system does not support automated dispute handling or refund workflows. Any conflicts between users must be resolved manually through direct communication or external support channels.

- **Advanced Publishing Workflow:**  
  Draft, preview, or multi-step publishing processes are not included. Marketplace items are published through a simplified mechanism without approval stages or complex publishing wizards.

- **Integrated Logistics and Shipping Services:**  
  There is no integration with third-party logistics or delivery services. Item exchanges and shipping arrangements are entirely coordinated by users outside the platform.

- **Bidding and Auction Mechanisms:**  
  The marketplace follows a fixed-price model only. Auction-style bidding, dynamic pricing, or competitive bidding features are excluded.

- **Guest or Anonymous Access:**  
  Access to the platform is restricted to authenticated users. Unregistered or anonymous users cannot view listings, profiles, or interact with the system.

- **Shopping Cart and Multi-Item Checkout:**  
  The system does not provide a shopping cart or bundled checkout functionality. Each item interaction is handled individually, aligning with the peer-to-peer nature of the platform.
