# Phone Book Application

The Phone Book Application is a simple PyQt5-based desktop application for managing a phone book. It allows users to add new contacts, search for existing contacts, and update or delete contact information. The application uses MongoDB as its backend database.

## Prerequisites

Before running the application, make sure you have the following dependencies installed:

- Python 3
- PyQt5
- pymongo
- peewee (for working with MongoDB)
- bson
- PyQt5.QtCore, PyQt5.QtGui, PyQt5.QtWidgets

You can install the required packages using the following command:

```bash
pip install PyQt5 pymongo peewee
```

## Features

- **Add Contact:** Users can add new contacts by providing their first name, last name, phone number, and address.
- **Search Contacts:** Users can search for contacts based on the first name and last name. The search results are displayed in a table.
- **Update Contact:** Users can update contact information directly in the table. The application prompts for confirmation before updating.
- **Delete Contact:** Users can delete contacts by double-clicking the "Delete" icon in the table. The application prompts for confirmation before deleting.

## Database

The application uses MongoDB as its backend database. It connects to the MongoDB server specified in the `local_settings.py` file and interacts with the "contact" collection.

## User Interface

The application has a tabbed interface with two tabs:

1. **Add Contact:** Allows users to input new contact details and add them to the database.
2. **Search Contacts:** Provides search functionality based on first name and last name. Displays the search results in a table, where users can update or delete contacts.

## How to Use

1. Run the `main.py` script using Python:

   ```bash
   python main.py
   ```
2. The application window will appear with tabs for adding and searching contacts.
3. Use the "Add Contact" tab to input new contact details and click the "Add Contact" button.
4. Use the "Search Contacts" tab to search for contacts based on first name and last name. The search results will be displayed in a table.
5. Double-click on a contact in the table to delete it. A confirmation prompt will appear.
6. Edit contact details directly in the table. A confirmation prompt will appear before updating the contact.

