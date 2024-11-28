# Address Book Application 📖

A simple and efficient **Address Book** program written in C. The application allows users to manage their contacts by adding, editing, deleting, sorting and displaying them in a well-formatted table.
This program validates user inputs such as names, email addresses, and mobile numbers using regular expressions.

---

## 📋 Features

- Add new contacts with validation for:
  - **Name**: Alphabetic characters only.
  - **Email**: Valid email format.
  - **Mobile Number**: 10-digit numeric validation.
- Edit existing contact details.
- Search for specific contacts by name.
- Delete contacts with confirmation.
- Display all contacts in a well-structured table format with styled output.
- Sort and display contacts by various criteria (e.g., name, email, mobile number).
- Supports multi-file project structure.

---

## 🚀 Getting Started

### Prerequisites
- A C compiler (e.g., GCC).
- Basic knowledge of compiling and running C programs.

---

🛠️ How to Use
Upon starting the program, you'll see a menu:

=> Add a contact.
=> Edit a contact.
=> Delete a contact.
=> Search for a specific contact.
=> Display all contacts.
=> Sort all contacts.
=> Exit.


📁 File Structure

address-book/
├── main.c          # Main program entry point

├── main.h          # Header file for main functions

├── file.c          # Contains core functions for file handling

├── file.h          # Header file for file operations

├── contact.c       # Contains contact management logic (add, edit, delete)

├── contact.h       # Header file for contact-related functions

├── Makefile        # Build system for compiling the project

└── README.md       # Project documentation


📜 Input Validation
The program uses regular expressions for validation:

- Name: ^[A-Za-z]+([ '-][A-Za-z]+)*$
- Email: ^[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}$
- Mobile: ^[0-9]{10}$
- Invalid inputs prompt the user to re-enter the data.



✨ Sample Output

 Address Book Application! 📖
-----------------------------------------
1. Add Contact
2. Edit Contact
3. Delete Contact
4. Search Contact
5. Display Contacts
6. Exit
Enter your choice: _

Table Format for Displaying Contacts📱

+----+------------------+------------------------+-------------+

| ID | Name             | Email                 | Mobile      |

+----+------------------+------------------------+-------------+

| 1  | John Doe         | john.doe@example.com  | 9876543210  |

| 2  | Jane Smith       | jane.smith@gmail.com  | 9123456789  |

+----+------------------+------------------------+-------------+
