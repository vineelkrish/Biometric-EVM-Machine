#  Biometric EVM (Electronic Voting Machine) using Arduino

This project is a **Biometric-based Electronic Voting Machine (EVM)** built using **Arduino**, a **Fingerprint Sensor Module**, and an **LCD Display**. The goal was to design a small-scale prototype of a secure, tamper-resistant voting system that authenticates users using biometrics instead of traditional methods.

---

##  Components Used

- ✅ Arduino Uno / Mega  
- ✅ R305 Fingerprint Sensor  
- ✅ 16x2 LCD Display  
- ✅ Push Buttons (for candidate voting)  
- ✅ Breadboard & Jumper Wires  
- ✅ Power Supply or USB  

---

##  Project Concept

This EVM prototype uses a fingerprint sensor to allow only registered users to vote. Once the fingerprint is verified, the user can vote for a candidate by pressing a physical button. The vote is recorded, and the LCD screen provides feedback. Multiple votes from the same fingerprint are prevented, ensuring **one person, one vote**.

---

##  Features

-  Biometric authentication using fingerprint  
-  LCD screen to display status (Access Granted, Voted, Error, etc.)  
-  Button-based voting system  
-  Resets for the next user after each vote  
-  Vote count stored in variables (displayed via serial monitor or LCD)  
-  Handles up to **210 voters** (limited by fingerprint sensor memory)
---

## ⚙ How It Works

1. **Fingerprint Enrollment**  
   Users are registered using the fingerprint sensor’s enroll mode.

2. **Authentication and Voting**  
   Voter places finger → matched with enrolled templates  
   → If matched: LCD shows success  
   → Candidate vote via button press  
   → Vote is recorded, duplicate voting blocked

3. **LCD Feedback**  
   Displays real-time messages like:
   - “Place Finger”
   - “Access Granted”
   - “Vote Casted”
   - “Already Voted”
   - “Access Denied”

---

## 📈 Limitations

-  Supports only ~210 users due to fingerprint module memory constraints  
-  No permanent vote storage (unless integrated with SD card or EEPROM)  
-  Basic hardware setup, not suited for mass deployment  
-  No web or backend integration for central monitoring

---

##  Future Enhancements

-  Add EEPROM or SD card for persistent vote storage  
-  Integrate with a cloud dashboard for real-time vote counts  
-  Improve UI/UX with a touchscreen or larger LCD  
-  Face recognition alongside fingerprint (multi-factor auth)  
-  Battery backup for field usability

---

##  Test Summary

-  Tested with: ~25–30 individuals  
-  Max users supported: ~210 (fingerprint storage)  
-  Accuracy: Acceptable for a small population (~92–95%)  
-  False negatives handled with retry prompts

---

## ⚠️ Disclaimer

This project is an academic prototype meant for **educational and experimental purposes only**. It is not intended for official electoral use.



