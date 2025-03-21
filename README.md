📜 README.md

# 🟩 Wordle Solver Bot

A Python-based Wordle solver that interacts with the **[Wordle API](https://wordle.votee.dev:8000/redoc)** to make word guesses and display feedback.  

## 🚀 Features
✅ Supports **daily**, **random**, and **custom word** modes  
✅ **Handles invalid words** (HTTP 422 error)  
✅ **Clear, user-friendly feedback** (✅, 🟡, ❌)  
✅ **Formatted output** for readability  

---

## 🔧 Installation & Setup

### **1️⃣ Install Python (if not installed)**
Ensure you have Python **3.6+** installed. Check with:
```sh
python --version
```
If not installed, download it from python.org.

2️⃣ Clone This Repository
```sh
git clone https://github.com/YOUR_GITHUB_USERNAME/wordle-solver.git
cd wordle-solver
```

3️⃣ Install Dependencies
```sh
pip install requests
```

🕹 Usage
Run the script

```sh
python wordle_solver.py
```

Example User Interaction

```sh
Enter mode (daily/random/custom): random
Enter your guess: apple

========================================
🟢 Guess: APPLE
========================================
  A: ✅ Correct
  P: ❌ Absent
  P: ❌ Absent
  L: ❌ Absent
  E: ✅ Correct
========================================
```

Modes
Mode	Description
daily	Guess against the daily Wordle
random	Guess a randomly selected word
custom	Guess against a user-specified word

⚠️ Error Handling
- Invalid Word (HTTP 422) → "⚠️ Invalid guess! Please try another word."
- API Issues (Other Errors) → Displays HTTP status code and error message

📌 Future Improvements
- 🔄 Automate word filtering based on feedback
- 🤖 AI-powered word selection for smarter guesses
- 📊 Game statistics tracking

🤝 Contributing
1. Fork the repository
2. Create a new branch (git checkout -b feature-branch)
3. Commit changes (git commit -m "Add new feature")
4. Push to GitHub (git push origin feature-branch)
5. Open a Pull Request
