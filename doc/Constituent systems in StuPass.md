# Constituent Systems in StuPass

## 1. Identity & Profile System
> **Boundary Rule:** This system owns all data related to the user entity, reputation, and access control. It does not handle product data or financial records.

**Assigned Processes:**
* **Register Account:** (Implicit required process)
* **Login/Authenticate:** (Implicit required process)
* **Update User Profile:** Managing personal bio, avatar, and contact details.
* **Rate User Profile:** Calculating and storing trust scores/reviews.

---

## 2. Marketplace & Inventory System
> **Boundary Rule:** This system manages the lifecycle of goods (items). It handles the creation, storage, retrieval, and public display of products. It is distinct from the transaction system as it deals with "listings" rather than "orders."

**Assigned Processes:**
* **Add Product:** Creating item records in the database.
* **Edit Product:** Modifying item details.
* **Search Personal Inventory:** Querying the user's own stock.
* **Search Marketplace Listings:** Querying the global product database.
* **Filter Listings:** Applying constraints to global search results.

---

## 3. Communication System
> **Boundary Rule:** This system is responsible for all real-time and asynchronous interaction between users. It manages connection states (sockets) and message persistence but does not process business logic (e.g., it delivers a "payment confirmed" message, but does not process the payment itself).

**Assigned Processes:**
* **Create Group Chat:** Instantiating multi-user conversation threads.
* **Send Message:** Handling text/media delivery and storage.
* **Initiate Video Call:** Establishing WebRTC (or similar) connections.
* **Archive Conversation:** Managing the visibility state of chat threads.

---

## 4. Transaction & Scheduling System
> **Boundary Rule:** This system handles the "business deal." It manages the exchange of value (money) and the logistics of the exchange (time/location). It interfaces with external Payment Gateways and Map Services.

**Assigned Processes:**
* **Execute Online Payment:** Processing financial transfers and maintaining ledger records.
* **Share Location:** Processing geospatial data for meetings.
* **Schedule Meeting:** Managing calendar objects for physical hand-offs.