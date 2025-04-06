# 📒 Assistant Bot

**Assistant Bot** is a console-based personal assistant that helps you manage contacts, phone numbers, and birthdays.  
It automatically saves your data between sessions using the `pickle` module.

---

## ✅ Available Commands

| Command                                      | Description                                                        |
|----------------------------------------------|--------------------------------------------------------------------|
| `hello`                                      | Greets the user                                                    |
| `add <name> <phone>`                         | Adds a new contact or phone number to an existing one              |
| `change <name> <old_phone> <new_phone>`      | Replaces an existing phone number                                  |
| `phone <name>`                               | Displays all phone numbers for a given contact                     |
| `all`                                        | Lists all saved contacts with phone numbers and birthdays          |
| `add-birthday <name> <DD.MM.YYYY>`           | Adds a birthday to a contact (format must be DD.MM.YYYY)           |
| `show-birthday <name>`                       | Displays the birthday of the given contact                         |
| `birthdays`                                  | Shows upcoming birthdays within the next 7 days                    |
| `exit` or `close`                            | Exits the program and saves all data automatically                 |

---

## 💾 Data Persistence

All contacts are saved in `addressbook.pkl` using the `pickle` module.  
Data is loaded automatically when the program starts and saved again upon exiting.

---

## 📌 Input Validation

- Phone numbers must contain **exactly 10 digits**.
- Birthdays must be in the **DD.MM.YYYY** format.
- All invalid input is handled with user-friendly error messages.

---

## 🚀 How to Run

```bash
python main.py
