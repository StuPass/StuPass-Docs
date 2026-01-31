# **Constituent Systems in StuPass**

## **1. Authentication System**

**Boundary Rule:** This system strictly manages user identification, session security, and credential recovery, serving as the entry point for identity verification without managing personal attributes or reputation.

**Core Use Cases:**
- Sign up
- Sign in
  - *«extends»* Sign in via Google
  - *«extends»* Sign in via Phone number
- Sign out
- Forgot password
- Change password

---

## **2. Profile Management System**

**Boundary Rule:** This system owns the user's personal data, contact information, and **Reputation Score** (calculated via report history). It aggregates the user's activity history (listings/purchased views) but does not handle the item data itself.

**Core Use Cases:**
- Create profile
- Edit profile
  - *«extends»* Add contact information
- View profile
  - *«extends»* Report user
  - *«extends»* View listing product
  - *«extends»* View purchased product
- Delete profile

---

## **3. Storage System**

**Boundary Rule:** This system functions as a private, persistent inventory (warehouse) where Sellers create, modify, and store product data indefinitely in a "Draft" state, completely isolated from public view until published to the Marketplace.

**Core Use Cases:**
- Add product
- Edit product
- Delete product
- View all product
- Search product

---

## **4. Marketplace System**

**Boundary Rule:** This system controls the public exhibition of goods; it transforms private inventory items into public posts, handling newsfeed distribution, search/filter visibility, post lifecycle, and content moderation (post reporting).

**Core Use Cases:**
- Add post
- Edit post
- Delete post
  - *«extends»* Undo delete
- View all post
  - *«extends»* View detail post
  - *«extends»* Search + filter
- Report post

---

## **5. Communication System**

**Boundary Rule:** This system manages real-time transmission and persistence of messages and calls to facilitate negotiation between Buyers and Sellers, serving as the primary coordination layer for peer-to-peer interaction.

**Core Use Cases:**
- Create chat box
- View all chat box
  - *«extends»* View a chat box
- View a chat box
  - *«extends»* Voice call
  - *«extends»* Video Call
- Chat
  - *«extends»* Turn on/off mic
- Voice call
  - *«extends»* Turn on/off mic
- Video Call
  - *«extends»* Turn on/off cam
  - *«extends»* Switch camera
- Hide chat box
  - *«extends»* Undo hide
- Find chat box
