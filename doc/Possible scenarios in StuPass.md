# Possible scenarios in StuPass 

## 1. Association Matrix 

The following table outlines the permissions for the Student actor in their roles as Seller and Buyer:

| Process ID | Process Name | Student (as Seller) | Student (as Buyer) |
| :--- | :--- | :---: | :---: |
| P-01 | Post management | X | X |
| P-02 | Profile management | X | X |
| P-03 | Storage management | X | |
| P-04 | Chat box management | X | X |
| P-05 | Transaction management | X | X |
| P-06 | Edit post | X | |
| P-07 | Delete post | X | |
| P-08 | Add post | X | |
| P-09 | View all post | | X |
| P-10 | Search + filter | X | |
| P-11 | Undo delete | X | |
| P-12 | Report post | | X |
| P-13 | View detail post | | X |
| P-14 | Edit profile | X | X |
| P-15 | View profile | X | X |
| P-16 | Add contact | X | X |
| P-17 | Verify identity | X | X |
| P-18 | Add email | X | X |
| P-19 | Add phone number | X | X |
| P-20 | Rating user | X | X |
| P-21 | Report user | X | X |
| P-22 | Write review | X | X |
| P-23 | Add product | X | |
| P-25 | Edit product | X | |
| P-26 | Delete product | X | |
| P-27 | View own product | X | |
| P-28 | View purchased product | X | |
| P-29 | Add product’s detail | X | |
| P-30 | Categorize product | X | |
| P-31 | Create chat box | X | X |
| P-32 | Create group chat box | X | X |
| P-33 | View all chat box | X | X |
| P-34 | View unread chat box | X | X |
| P-35 | Hide chat box | X | X |
| P-36 | Find chat box | X | X |
| P-37 | View a chat box | X | X |
| P-38 | Chat | X | X |
| P-39 | Video call | X | X |
| P-40 | Undo hide chat box | X | X |
| P-41 | Archive chat box | X | X |
| P-42 | Buy item | | X |
| P-43 | View transaction history | X | X |
| P-44 | Pay online | | X |
| P-45 | Pay offline | | X |
| P-46 | Meet-up scheduling | X | X |
| P-47 | Sharing location | X | X |

## 2. Internal dependencies 


### Mandatory logic: 
* Delete post `<<include>>` Undo delete
* Hide chat box `<<include>>` Undo hide
* Hide chat box `<<include>>` Archive

### Optional logic: 
* Post management `<<extends>>` Edit post
* Post management `<<extends>>` Delete post
* Post management `<<extends>>` Add post
* Post management `<<extends>>` View all posts
* View all posts `<<extends>>` Report post
* View all posts `<<extends>>` View detail post
* View all posts `<<extends>>` Search + filter 
* Profile management `<<extends>>` Edit profile
* Profile management `<<extends>>` View profile 
* Edit profile `<<extends>>` Add contact 
* Edit profile `<<extends>>` Verify identity 
* View profile `<<extends>>` Rating user
* View profile `<<extends>>` Report user
* Verify identity `<<extends>>` Add Email
* Verify identity `<<extends>>` Phone number
* Rating user `<<extends>>` Write reviews
* Storage management `<<extends>>` Add product
* Storage management `<<extends>>` Delete product 
* Storage management `<<extends>>` Edit product 
* Storage management `<<extends>>` View own product 
* Storage management `<<extends>>` View purchased product
* Add product `<<extends>>` Add product's detail 
* Add product `<<extends>>` Categorize product 
* Chat box management `<<extends>>` Create chat box 
* Chat box management `<<extends>>` Create group chat box 
* Chat box management `<<extends>>` View all chat boxes 
* Chat box management `<<extends>>` View unread chat box 
* Chat box management `<<extends>>` Hide chat box 
* Chat box management `<<extends>>` Find chat box 
* View all chat boxes `<<extends>>` View a chat box 
* View unread chat box `<<extends>>` View a chat box 
* View a chat box `<<extends>>` Chat 
* View a chat box `<<extends>>` Video Call 
* Transaction management `<<extends>>` Buy item
* Transaction management `<<extends>>` View transaction history 
* Buy item `<<extends>>` Pay offline
* Buy item `<<extends>>` Pay online
* Pay offline `<<extends>>` Meet-up scheduling
* Pay offline `<<extends>>` Sharing location
* Authentication `<<extends>>` Sign up via Google
* Authentication `<<extends>>` Sign up via Facebook 
* Authentication `<<extends>>` Sign up via Phone number
* Authentication `<<extends>>` Sign out
* Sign up via Google `<<extends>>` Create profile 
* Sign up via Facebook `<<extends>>` Create profile 
* Sign up via Phone number `<<extends>>` Create profile 