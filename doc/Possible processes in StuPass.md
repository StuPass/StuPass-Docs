# Possible Processes in StuPass

## 1. Profile Processes

### Create Profile
- **Trigger:** A new user completes the registration process or logs in for the first time and is prompted to set up their profile.
- **Success Condition:** The system creates a new profile with default values, saves the provided information (basic details, avatar, bio), and makes the profile accessible to the user and others according to visibility rules.

### Edit Profile
- **Trigger:** User selects the **"Edit"** option on their personal profile page and submits modified details (bio, contact info, avatar).
- **Success Condition:** The system validates the input, updates the database, and displays the revised profile information to the user.

### Add Contact Information *(«extends» Edit Profile)*
- **Trigger:** User selects **"Add contact information"** while editing their profile and submits contact fields (phone number, email address, physical address, or social links).
- **Success Condition:** The system validates contact formats, saves the updated contact details, and displays them according to the user’s visibility settings.

### View Profile
- **Trigger:** User clicks on another user’s name from a marketplace listing or opens their own profile page.
- **Success Condition:** The system displays the user’s public profile information such as avatar, bio, reputation score, and visible contact information.

### View Listing Product *(«extends» View Profile)*
- **Trigger:** While viewing a Seller's profile, user selects **"View listing products"**.
- **Success Condition:** The system displays all active marketplace posts created by the seller, including basic product details such as name, price, category, and status.

### View Purchased Product *(«extends» View Profile)*
- **Trigger:** User opens their own profile and selects **"View purchased products"**.
- **Success Condition:** The system displays the user's purchase history, including purchased items, prices, purchase dates, and order statuses.

### Report User *(«extends» View Profile)*
- **Trigger:** While viewing a profile, user selects **"Report user"**, chooses a report reason, and submits the report.
- **Success Condition:** The system records the report with the reporter ID, reported user ID, reason, and timestamp, and confirms successful submission for moderation review.

### Delete Profile
- **Trigger:** User selects the **"Delete Profile"** option from account settings and confirms the action.
- **Success Condition:** The system permanently removes or deactivates the profile, revokes public access, and confirms the deletion to the user while preserving required audit or transaction records.

---

## 2. Storage Processes

### Add Product
* **Trigger:** Seller fills out the product details form (name, price, category, images) in the Storage section and clicks **Save**.
* **Success Condition:** A new product record is created in the database, visible in the Seller's personal storage.

### Edit Product
* **Trigger:** Seller modifies details of an existing item in their storage.
* **Success Condition:** The product information is updated in the database and reflected in any active marketplace listings.

### View All Product
* **Trigger:** Seller navigates to the Storage screen.
* **Success Condition:** The system retrieves and displays the complete list of available products associated with the user, including basic details such as name, price, status, and category.

### Delete Product
* **Trigger:** When a Seller chooses **Delete** from the storage menu.
* **Success Condition:** The permanent removal of the item from both storage and marketplace.

### Search Product
* **Trigger:** Seller enters keywords or chooses categories into the search bar within their Storage Management screen.
* **Success Condition:** The system displays a list of personal items matching the search criteria.

---

## 3. Marketplace Processes

### Add Post
- **Trigger:** Seller selects the **"Add"** option, chooses an item from storage, and confirms publishing it on the marketplace.
- **Success Condition:** A new marketplace post is created and becomes visible to all users in the main marketplace feed.

### View All Post
- **Trigger:** Seller or buyer navigates to the Marketplace screen.
- **Success Condition:** The system retrieves and displays a list of active posts, including basic details such as title, price, category, condition, and post status.

### View Detail Post *(«extends» View All Post)*
- **Trigger:** Buyer clicks a post card from the marketplace feed or search results.
- **Success Condition:** The system displays full post details, including images, description, seller information, price, and available actions.

### Search + Filter *(«extends» View All Post)*
- **Trigger:** Buyer enters keywords into the marketplace search bar and/or applies filters such as price range, category, condition, or sorting options.
- **Success Condition:** The displayed list is refined to show only posts that match the selected criteria.

### Edit Post
- **Trigger:** Seller selects **"Edit"** on one of their published posts and modifies post details.
- **Success Condition:** The system updates the post information in the database and reflects the changes in the marketplace listings.

### Delete Post
- **Trigger:** Seller selects **"Delete"** on a post and confirms the action.
- **Success Condition:** The post is removed from public marketplace views and search results.

### Undo Delete *(«extends» Delete Post)*
- **Trigger:** Seller selects **"Undo Delete"** on a recently deleted post.
- **Success Condition:** The system restores the post and makes it visible again in the marketplace.

### Report Post
- **Trigger:** Buyer selects **"Report"** on a post and submits a report reason.
- **Success Condition:** The system records the report and confirms successful submission for moderation review.

---

## 4. Communication Processes

### Create Chat Box
- **Trigger:** User clicks **"Message / Chat"** on another user's profile or from a post details page.
- **Success Condition:** The system creates a new conversation thread (or reopens an existing one) and displays it in the chat box list.

### View All Chat Box
- **Trigger:** User opens the Communication / Inbox screen.
- **Success Condition:** The system loads and displays all conversation threads the user participates in, sorted by latest activity and showing unread indicators.

### View a Chat Box *(«extends» View All Chat Box)*
- **Trigger:** User selects a specific conversation from the chat box list.
- **Success Condition:** The system loads the full conversation history, displays messages in chronological order, and marks unread messages as read.

### Find Chat Box
- **Trigger:** User enters a keyword (user name, order ID, or message content) into the chat search bar.
- **Success Condition:** The system returns matching conversation threads and allows the user to open a selected chat.

### Send Message
- **Trigger:** User types text or attaches media in a chat box and clicks **“Send”**.
- **Success Condition:** The message is delivered to the recipient(s) and persistently stored in the conversation history.

### Initiate Voice Call
- **Trigger:** User clicks the **voice call** icon within an active chat box.
- **Success Condition:** The system establishes a real-time voice connection between participants and displays the in-call interface.

### Initiate Video Call
- **Trigger:** User clicks the **video call** icon within an active chat box.
- **Success Condition:** The system establishes a real-time video connection between participants.

### Turn On / Off Microphone
- **Trigger:** During a voice or video call, user taps the **microphone toggle** button.
- **Success Condition:** The system mutes or unmutes the user’s audio stream and updates the microphone status indicator.

### Turn On / Off Camera
- **Trigger:** During a video call, user taps the **camera toggle** button.
- **Success Condition:** The system disables or enables the video stream and updates the camera status indicator.

### Switch Camera
- **Trigger:** During a video call, user taps the **switch camera** button.
- **Success Condition:** The system switches between available cameras (front/back) without interrupting the call.

### Hide Chat Box
- **Trigger:** User selects **"Hide"** or **"Archive"** on a conversation thread.
- **Success Condition:** The chat box is removed from the active conversation list while remaining accessible in the archive.

### Undo Hide *(«extends» Hide Chat Box)*
- **Trigger:** User selects **“Restore”** or **“Undo Hide”** from the archived conversations list.
- **Success Condition:** The conversation is restored to the active chat box list.

---

## 5. Authentication Processes

### Sign Up
- **Trigger:** User selects the **"Sign up"** option from the authentication screen and provides required registration information.
- **Success Condition:** The system validates the input, creates a new user account, and proceeds to profile creation or initial setup.

### Sign In
- **Trigger:** User selects the **"Sign in"** option and enters valid authentication credentials.
- **Success Condition:** The system authenticates the user successfully and grants access to the application.

### Sign In via Google *(«extends» Sign In)*
- **Trigger:** User selects **"Sign in via Google"** from the sign-in screen.
- **Success Condition:** The system authenticates the user using Google OAuth and signs the user into the system.

### Sign In via Phone Number *(«extends» Sign In)*
- **Trigger:** User selects **"Sign in via Phone Number"**, enters their phone number, and confirms the verification code.
- **Success Condition:** The system verifies the phone number, authenticates the user, and grants access to the application.

### Sign Out
- **Trigger:** User selects **"Sign out"** from the account menu.
- **Success Condition:** The system terminates the current session and redirects the user to the authentication screen.

### Forgot Password
- **Trigger:** User selects **"Forgot password"** on the sign-in screen and submits their registered email or phone number.
- **Success Condition:** The system sends a password reset link or verification code to the user.

### Change Password
- **Trigger:** Authenticated user selects **"Change password"** from account settings or completes password reset flow.
- **Success Condition:** The system validates the new password, updates credentials securely, and confirms the password change.

---