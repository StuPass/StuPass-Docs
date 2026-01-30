# Possible Scenarios in StuPass

## 1. Association Matrix

The following table defines the permissions of the **Student actor**, who may act as a **Seller** or **Buyer** depending on usage context.

> Note: Although Seller and Buyer have different functions, they belong to the same role (User).

| Process ID | Process Name | Student (Seller) | Student (Buyer) |
|-----------|-------------|:----------------:|:---------------:|
| P-01 | Sign up | X | X |
| P-02 | Sign in | X | X |
| P-03 | Sign in via Google | X | X |
| P-04 | Sign in via phone number | X | X |
| P-05 | Sign out | X | X |
| P-06 | Forgot password | X | X |
| P-07 | Change password | X | X |
| P-08 | Create profile | X | X |
| P-09 | Edit profile | X | X |
| P-10 | View profile | X | X |
| P-11 | Delete profile | X | X |
| P-12 | Add contact information | X | X |
| P-13 | Verify identity | X | X |
| P-14 | Rating user | X | X |
| P-15 | Write review | X | X |
| P-16 | Report user | X | X |
| P-17 | Add product | X | |
| P-18 | Edit product | X | |
| P-19 | Delete product | X | |
| P-20 | View own product | X | |
| P-21 | View purchased product | | X |
| P-22 | Add post | X | |
| P-23 | Edit post | X | |
| P-24 | Delete post | X | |
| P-25 | Undo delete post | X | |
| P-26 | View all posts | | X |
| P-27 | View detail post | | X |
| P-28 | Search + filter posts | | X |
| P-29 | Report post | | X |
| P-30 | Create chat box | X | X |
| P-31 | Create group chat box | X | X |
| P-32 | View all chat boxes | X | X |
| P-33 | View unread chat box | X | X |
| P-34 | View a chat box | X | X |
| P-35 | Chat (messaging) | X | X |
| P-36 | Voice call | X | X |
| P-37 | Video call | X | X |
| P-38 | Hide chat box | X | X |
| P-39 | Archive chat box | X | X |
| P-40 | Undo hide chat box | X | X |

---

## 2. Internal Dependencies

### 2.1 Mandatory Logic (`<<include>>`)

- Sign up `<<include>>` Create profile  
- Delete post `<<include>>` Undo delete post  
- Hide chat box `<<include>>` Undo hide chat box  
- Hide chat box `<<include>>` Archive chat box  

---

### 2.2 Optional Logic (`<<extends>>`)

#### Authentication
- Sign in `<<extends>>` Sign in via Google  
- Sign in `<<extends>>` Sign in via phone number  

#### Profile Management
- Edit profile `<<extends>>` Add contact information  
- Edit profile `<<extends>>` Verify identity  
- View profile `<<extends>>` Rating user  
- View profile `<<extends>>` Write review  
- View profile `<<extends>>` Report user  

#### Marketplace Management 
- Delete post `<<extends>>` Undo delete post  
- View all posts `<<extends>>` View detail post  
- View all posts `<<extends>>` Search + filter posts  
- View all posts `<<extends>>` Report post  

#### Chat Box Management
- View all chat boxes `<<extends>>` View a chat box  
- View unread chat box `<<extends>>` View a chat box  
- View a chat box `<<extends>>` Chat  
- View a chat box `<<extends>>` Voice call  
- View a chat box `<<extends>>` Video call  
- Hide chat box `<<extends>>` Undo hide chat box  
- Hide chat box `<<extends>>` Archive chat box  
