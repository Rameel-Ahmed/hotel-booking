# hotel-booking
# 🏨 Hotel Reservation System (Python + Pandas)

This is a simple command-line hotel booking system built in Python. It uses **pandas** to read CSV files, **OOP concepts** (classes, inheritance), and simulates secure credit card validation.

---

## 🚀 Features

- Select a hotel using an ID
- Check if the hotel is available
- Simulate credit card validation (expiration, holder, CVC)
- Authenticate card using a password
- Book the hotel and generate a reservation ticket
- Update availability in the `hotels.csv` file

---

## 🗂 CSV Files Used

### 1. `hotels.csv`
Stores hotel data.

| id  | name           | available |
|-----|----------------|-----------|
| 1   | Hilton Garden  | yes       |
| 2   | Marriott Place | no        |

### 2. `cards.csv`
Stores valid credit card details.

| number             | expiration | holder      | cvc |
|--------------------|------------|-------------|-----|
| 1234567890123456   | 12/26      | JOHN SMITH  | 123 |

### 3. `card_security.csv`
Stores passwords for secure authentication.

| number             | password  |
|--------------------|-----------|
| 1234567890123456   | mypass1   |

---

## 🧠 How It Works

### 1. User is asked for a hotel ID:
```bash
Enter the id of the hotel: 1
```

### 2. The system:
- Checks if the hotel is available
- Validates the card details
- Authenticates using a password
- Books the hotel
- Prints a reservation confirmation

---

## 🏗 Classes Overview

| Class              | Purpose                                  |
|--------------------|------------------------------------------|
| `Hotel`            | Manages hotel availability and booking   |
| `ReservationTicket`| Creates confirmation message             |
| `CreditCard`       | Validates credit card info               |
| `SecureCreditCard` | Inherits `CreditCard`, adds password check |

---

## 📋 Example Output

```
Enter the id of the hotel: 1
Enter your name: Rayyan

Thank you for your reservation!
Here are you booking data:
Name: Rayyan
Hotel name: Hilton Garden
```

---

## 📦 How to Run

1. Make sure `pandas` is installed:
```bash
pip install pandas
```

2. Prepare the three CSV files (`hotels.csv`, `cards.csv`, `card_security.csv`) in the same folder.

3. Run the script:
```bash
python main.py
```

---

## ✅ What You’ll Learn from This

- Using pandas to read/write CSV data
- Class-based architecture in Python
- How to simulate real-world booking flows
- OOP: Inheritance, encapsulation, method overriding

---

## 🛠 Future Improvements

- Add GUI using Tkinter or PyQt
- Store bookings in a separate `reservations.csv`
- Support multiple users
- Add card lockout after 3 failed attempts

---


