# Possible Processes in StuPass

## 1. Profile & Storage Processes

### Update User Profile
* **Trigger:** Student selects the "Edit" option on their personal profile page and submits modified details (bio, contact info, avatar).
* **Success Condition:** The system validates the input, updates the database, and displays the revised profile information to the user.

### View Profile
* **Trigger:** When a user clicks on a Seller's name from a marketplace listing.
* **Success Condition:** The rendering of the public bio and reputation score.

### Rate User Profile
* **Trigger:** A Buyer or Seller submits a star rating and review after a transaction is marked complete.
* **Success Condition:** The system calculates the new average reputation score and appends the review to the target user's public profile.

---

## 2. Profile & Storage Processes
### Add Product
* **Trigger:** Seller fills out the product details form (name, price, category, images) in the Storage section and clicks "Save".
* **Success Condition:** A new product record is created in the database, visible in the Seller's personal inventory.

### Edit Product
* **Trigger:** Seller modifies details of an existing item in their inventory.
* **Success Condition:** The product information is updated in the database and reflected in any active marketplace listings.

### Remove Product
* **Trigger:** When a Seller chooses "Delete" or "Withdraw" from the storage menu.
* **Success Condition:** The permanent removal of the item from both inventory and marketplace.

### Search Personal Storage
* **Trigger:** Seller or buyer enters keywords or chooses categories into the search bar within their Storage Management screen.
* **Success Condition:** The system displays a list of personal items matching the search criteria.

---

## 3. Marketplace Processes

### Publish Listing
* **Trigger:** Seller selects an item from inventory and chooses to make it public on the marketplace.
* **Success Condition:** The product becomes visible to all users in the main marketplace feed.

### Search Marketplace Listings
* **Trigger:** Buyer enters keywords (e.g., "Calculus Textbook") into the global search bar.
* **Success Condition:** The system retrieves and displays a list of active product listings matching the keywords.

### Filter Listings
* **Trigger:** Buyer applies constraints (e.g., Price Range, Category, Condition) to search results.
* **Success Condition:** The displayed list is refined to show only items meeting the selected criteria.

---

## 4. Communication Processes

### Create Group Chat
* **Trigger:** User selects multiple contacts or a specific class/club context and initiates a conversation.
* **Success Condition:** A new shared chat room is instantiated, allowing all selected members to send and receive messages.

### Send Message
* **Trigger:** User types text or attaches media in a chat box and hits "Send".
* **Success Condition:** The message is delivered to the recipient(s) and persistently stored in the conversation history.

### Initiate Video Call
* **Trigger:** User clicks the video call icon within an active chat box.
* **Success Condition:** The system establishes a real-time video connection between the participants.

### Archive Conversation (Hide Chat Box)
* **Trigger:** User selects the "Hide" or "Archive" option on a specific conversation thread.
* **Success Condition:** The chat box is removed from the active "View All" list but remains accessible in the archive.

---

## 5. Transaction Processes

### Share Location
* **Trigger:** User selects the "Share Location" feature during a chat to propose a meeting spot.
* **Success Condition:** The system retrieves geospatial data and renders a map pin in the chat window visible to the recipient.

### Schedule Meeting
* **Trigger:** Users agree on a time and confirm a meeting request form within the chat.
* **Success Condition:** An appointment is created and added to the internal calendar/schedule for both users.

### Execute Online Payment
* **Trigger:** Buyer confirms the checkout process for an item using an integrated payment gateway.

* **Success Condition:** Funds are successfully deducted from the Buyer, held in escrow (if applicable), and a transaction receipt is generated.
