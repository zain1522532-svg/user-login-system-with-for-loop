# 🔐 Python User Login System

A simple **Python-based Login System** that allows users to log in using predefined usernames and passwords.  
The program gives the user **three attempts** to enter correct credentials before denying access.

---

## 🧠 Features
- Stores multiple users and their passwords using a Python dictionary  
- Checks username and password validity  
- Displays custom messages for:
  - Successful login  
  - Incorrect password  
  - Username not found  
- Limits login attempts to 3 tries

---

## 🧩 Code Example

```python
users = {
    "Zain": "22532",
    "Hammad": "22542",
    "Muneeb": "38924",
    "Ahmed": "04734"
}

for attempt in range(3):
    username = input("Enter username: ")
    password = input("Enter password: ")

    if username in users:
        if password == users[username]:
            print("Login Successful!")
            break
        else:
            print("Incorrect password!")
    else:
        print("Username not found!")

    attempts_left = 3 - 1 - attempt
    if attempts_left > 0:
        print(f"Attempts left: {attempts_left}\n")
else:
    print("Too many failed attempts! Access denied.")
    print("Try Again Later!")
````

---

## 🛠️ Requirements

* **Python 3.x** (any version 3.6 or above)

---

## 🚀 How to Run

1. Clone or download this repository:

   ```bash
   git clone https://github.com/your-username/login-system.git
   ```
2. Open the folder in your IDE or terminal.
3. Run the script:

   ```bash
   python login.py
   ```

---

## 📚 Learning Goals

* Understanding Python dictionaries
* Practicing `if-else` and nested conditions
* Handling user input and loops

---

## 🧑‍💻 Author

**Zain Akram**
💼 *Beginner Python Developer*
📧 *zain1522532@gmail.com*
🌐 [[GitHub Profile](https://github.com/your-username)](https://github.com/zain1522532-svg)

---

## 🪪 License

This project is open source and available under the [MIT License](LICENSE).

```

---

Would you like me to make a **shorter README (for beginners)** or a **professional GitHub-style one with badges and screenshots**?
```
