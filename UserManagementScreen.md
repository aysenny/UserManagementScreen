User Management Screen UI Specification Document
Overview
The User Management Screen allows administrators to manage user accounts within the system. It provides functionalities for viewing and adding user accounts.

Requirements
User List Display

Display a list of all users with their details (ID, Username, Email, Status).
Each field should be sortable.
Implement a toggle to hide disabled users.

Add New User Functionality

A button to open a form for creating a new user.
The form should include fields for Username, Display Name, Phone, Email, Role, and an Enabled checkbox.

User Role Management

Role should be selectable from the following options: Guest, Admin, Superadmin.

Responsive Design

Ensure the interface is responsive and usable on both desktop and mobile devices.


UI Components

1. New User Button
Type: Button
Style: Blue with a "+" icon
Label: "New User"
Behavior:
Clicking opens a modal/form to add a new user.
2. Hide Disabled Users Toggle
Type: Clickable square
Label: "Hide Disabled Users"
Behavior:
Toggles the visibility of users marked as disabled in the user list.
3. User List Table
Columns:
ID
Username
Email
Enabled
Components:
Each column header should have a sort button to allow sorting.
Behavior:
Display the user list with pagination, showing a set number of users per page.
The list should dynamically update based on the Hide Disabled Users toggle.
5. User Form (for Add New User)
Fields:
Username (Input)
Display Name (Input)
Phone (Input)
Email (Input)
Role (Dropdown: Guest, Admin, Superadmin)
Enabled (Checkbox)
Behavior:
The form should validate input fields before submission.
Upon submission, a new user should be added to the user list, and the form should close.
Initial User Interface State
The screen displays a loading indicator while fetching user data.
Once loaded, the user list table appears, populated with user information.
The New User button and Hide Disabled Users toggle are prominently displayed.
The search bar should be empty, and the user list displays the first page of users.
Page Behavior
Loading State: Display a spinner while fetching user data.
Empty State: Show a message if no users are found after a search.
Error Handling: Display error messages for failed actions (e.g., delete user) in a user-friendly manner.
Accessibility Considerations
Ensure all components are keyboard navigable.
Provide ARIA labels for assistive technologies.