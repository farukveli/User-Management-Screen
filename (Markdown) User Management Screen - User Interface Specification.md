# **User Management Screen - User Interface Specification**

## **Introduction**

The User Management Screen is a user interface designed to allow administrators to manage users within the system. This document outlines the requirements and specifications for developing the User Management Screen. It is intended for software developers who will be responsible for implementing the user interface.

## **Requirements**

The User Management Screen should fulfill the following requirements:
- Allow administrators to create new users by providing required user details (username, display name, phone, email, user roles, enable).
- Display a list of existing users with their relevant information (id, user name, email, status).
- Hide disabled users from list of existing user.
- Filter or sort list by user details.
- Allow administrators to edit existing user details, such as username, display name, phone, email, role and status.

## **UI Components and Behavior**

UI components details is given this section.

### 1.User List

- The User List will be displayed in a tabular format, showing each user's id, username, email and status.
- Status column's title will be "Enabled" and each cells that are in this column must be "true" or "false".
- Administrators can click on a user's row to view detailed user information and perform editing actions.
- The User List will be filtered or sorted by each information title. For this behavior every title will include sort icon and filter icon. When clicked filter icon, filter options will be accessible.
- Disabled users will hidden when clicked the check box that is tagged "Hide Disabled User"

### 2.New User Form

- The New User Form will be accessible via a "+ New User" button on the User Management Screen.
- The form will include text fields for entering the new user's username, display name, phone, email.
- The user's role will be selected by clicking combo box which is include roles that guest, admin, super admin.
- The status will set by clikcking check box that is tagged "Enabled".
- Username, phone, email and role fields musn't be null.
- If the display name field is null, display field will filled with username.
- Each components will tagged by relevant information name.
- The new user will saved when clikced "Save User" button on the User Management Screen.
- "Save User" button must be disabled when New User form or Display form are not visible.

### 3.Display and Edit Existing User

- The Display form will be same with the New User Form.
- When a user's row is clikced, guests can only view detailed user information but admins and super admin can perform editing actions.
- The changes will saved when administrators clikced "Save User" button on the User Management Screen.

### 4.Success and Error Messages

- Success messages should be displayed when user management operations (e.g., create, edit) are successful.
- Error messages should be shown in case of any errors or validation failures during these operations.
- The messages should be displayed at the top of the User Management Screen and fade away after a few seconds.

## **Initial Display**

- Opening the User Management Screen, the list of all existing users will be displayed in the User List.
- User List should be sorted by increased id.
- New User form or Display form are not visible at the first.

## **Conclusion**

This User Interface Specification document outlines the requirements and specifications for just the User Management Screen. Following these guidelines, the software developers can implement an efficient and user-friendly user interface for managing users in the system. This document not include backend specifications like how to generate id number for new user.



