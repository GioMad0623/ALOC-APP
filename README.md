
# 💳 A.L.O.C. - All Lines of Credit

**A.L.O.C.** is a mobile-first financial management app that links multiple credit cards to a single virtual wallet. When a purchase is made using the designated virtual card, the app intelligently splits the transaction across all linked credit cards based on customizable rules such as equal distribution, minimum payment obligations, and user preferences.

---

## 🧠 Key Features

- 🔐 User authentication (JWT)
- 💳 Add and manage multiple credit cards
- 📊 Real-time balance display
- ⚙️ Smart transaction splitter based on minimums + even distribution
- 🧾 Customizable allocation options
- 📱 Fully responsive React Native frontend (Expo-powered)
- 🗂️ Backend powered by FastAPI with SQLite (PostgreSQL-ready)

---

## 📁 Project Structure

```
A.L.O.C/
├── backend/                  # FastAPI backend
├── frontend/                 # React Native (Expo) frontend
└── README.md                 # Project info & setup guide
```

---

## ⚙️ Backend Setup (FastAPI)

### Requirements:
- Python 3.9+
- pip

### Setup Instructions:
```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

API available at `http://localhost:8000`

---

## 📱 Frontend Setup (React Native + Expo)

### Requirements:
- Node.js (LTS)
- npm
- Expo CLI

### Setup Instructions:
```bash
npm install -g expo-cli
cd frontend/aloc_app
npm install
npx expo start
```

Open the app on your mobile device using the QR code from the Expo dev tools.

---

## 🔐 Environment Variables

Set the following in a `.env` file for backend secrets (optional):
```env
SECRET_KEY=your_secret_key
DATABASE_URL=sqlite:///./test.db  # Or use PostgreSQL URI
```

---

## 🏦 Integrations (Upcoming)

- **Stripe Issuing** – for virtual card issuing
- **Plaid** – for linking and reading card data securely

---

## 👤 Author

**Giovanni Madaffari**  
Founder & Creator of A.L.O.C.  
Contact: 

---

## 🛠️ Future Improvements

- PostgreSQL migration
- Real transaction posting to cards
- Advanced budget analytics
- Bank account sync via Plaid

---

## 📄 License

MIT License – You may use, modify, and share freely with attribution.
