# **Constituent Systems in StuPass**

## **1\. Authentication System**

**Boundary Rule:** This system strictly manages user identification, session security, serving as the entry point for identity verification without managing personal attributes or reputation.

## **2\. Profile Management System**

**Boundary Rule:** This system owns the user's personal data, contact information, and **Reputation Score** (calculated via report history); it aggregates the user's activity history (listings/purchased views) but does not handle the item data itself.

## **3\. Storage System**

**Boundary Rule:** This system functions as a private, persistent inventory (warehouse) where users create, modify, and store product data indefinitely in a "Draft" state, completely isolated from public view until published.

## **4\. Marketplace System**

**Boundary Rule:** This system controls the public exhibition of goods; it transforms private inventory items into public posts, handling newsfeed distribution, search visibility, and content moderation (post reporting).

## **5\. Communication System**

**Boundary Rule:** This system manages real-time transmission and persistence of messages/calls to facilitate negotiation, serving as the primary validation layer for user interaction in the absence of transaction records.
