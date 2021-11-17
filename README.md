# The objective of this project is to build a desktop application that allows a user to capture ToDo items and categorize them into groups.

## Objectives: 
* Item
* User Management
* Interface

## Criteria: 
* Criteria for Item
 1) Each Item can be stand-alone (Uncategorized) or part of a Category of Items (Categorized).
 2) Each Item can have zero or more Tags associated with it.  Tags are independent of Categories and can be used by users to group visually-similar Items.
 3) Each Item  must have a Created Date and Last Updated Date.
 4) Must have a way to manage Purchase Orders (PO); Keep it simple and oriented to what you need for the application, nothing more.
 5) Each Item must have a Quantity value; It should be broken down into Current, Reorder Level, and Pending properties.
* Current is the Active value in stock; this will go up and down over time.
* Reorder Level will be entered once and should be changed only by the appropriate Role.
* Pending should be based on a pending receipt PO.
 6) Each Item must have a Short and Long Description.
 7) Each Item must be associated with a current/past PO.
 8) Draw down of an Item Quantity must come from the older PO first; effectively working from oldest to newest PO.
 
## Criteria for User Management
1) A User can be assigned one or more Roles within the application. 
 * Suggested Roles: Read, Edit, Accounting, Update, Manage, and/or Administer. 
 * Read - User will be able only to View various Items List/Tags and associated PO's.
 * Edit - User will be able to Read and Create/Modify Item List(s) and Items but not Update an individual Item.
 * Accounting - User will be able to create a PO with pending Inventory; Cannot be a part of any other Role.
 * Update - User will be able to Read and Update individual Item's details (such as Description); They will NOT be able to modify an Item's PO information.
 * Manage - User will be able to Read, Edit, and Update, but will NOT be able to Manage Users.
 * Administer - User will be able to Read, Edit, Update, and Manage; in addition, they will be able to Add, Edit, and Remove Users from the application; This will generally also include changing User Password and User contact info.
2) A User can self-register or be pre-registered by an Administrator.
3) Once a User has an ID to login, the ID cannot be changed.
4) User can change contact information and reset their password.

## Criteria for Interface
1) Must have a text-base navigation menubar.
2) Must have a image-based navigation menubar with common actions; can be Role based but not necessary.
3) Body must be split into two sections.
* Left-side: an expandable list of Categories.
* Right-side: shows the ToDo items of the Category.
4) The Right-Side of the Body, must be a GridView of the ToDo items.
5) The GridView rows must be clickable (Single or Double; suggest Double) to show a DetailsView of the Item clicked.
6) DetailsView must provide the ability appropriate with the User's Role.
7) Must have appropriate access to Role-based features.
8) Role-based features must be visible to user's ONLY within that Role.
