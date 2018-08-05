# Walking Tours 2.0 - Database/Backend

## **Objective**

### **Who is this product/feature for?**
This product is for content providers; Governments, local meetups that can curate content being uploaded.

### **Which problem are you trying to solve?**
It isn't possible for Code For Orlando to curate, and upload new, and maintain POIs for all cities over the country.

### **What is the goal of this feature?**
A secure and guarded backend that can upload new content to the user facing portion of this product.

### **What will this feature do, and what will it not do?**
| Will do | Won't do|
| ------- | ------- |
| User login | User registration |
| Password reset for account ||
| Maintain POIs |  |
| Upload a single POI by manually entering the values ||
| Bulk upload POI information via CSV/Excel spreadsheet | |

## **Core Components**
* Easy to maintain POI DB.
    * A user should not be required to write any code.
* Ability to generate GPS co-ordinates from a street address
* Ability to generate a street address based on co-ordinates
* Upload images for a specific POI
* Send reset password email.

## **User flow**
* Login
    * Username
    * Password
    * Forgot password
* Main View
    * View all POIs as a list
    * Sort lists based on columns (perhaps just name for MVP)
    * Bulk Upload button
    * Create new button
* Create new POI
    * Form with the following fields
        * Title
        * Description
        * Installation date - optional
        * Location
            * Human readable address
            * GPS co-ordinates - optional
* Bulk upload - modal view over main view
    * Drag and drop view that accepts:
        * CSV
        * Excel?
