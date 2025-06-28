# Splitwise-clone
#  Splitwise Clone (Expense Tracker)

A simple web app to manage group expenses, add members, track who owes whom, and view balances — inspired by Splitwise.



## 🚀 Features

* Create groups with member IDs
* Add expenses (equal or percentage split)
* View all group expenses
* View group balances (who owes whom)



## 💠 Tech Stack

* **Frontend**: React, Axios, React Router DOM
* **Backend**: FastAPI, SQLAlchemy, PostgreSQL
* **Database**: PostgreSQL


## 📁 Project Structure

```
splitwise_clone/
│
├── backend/         # FastAPI app (Python)
│   ├── app/
│   │   ├── routers/
│   │   ├── models/
│   │   ├── schemas/
│   │   └── main.py
│   └── requirements.txt
│
├── frontend/        # React app (JavaScript)
│   └── src/components/
│       ├── CreateGroup.js
│       ├── CreateExpense.js
│       ├── ViewExpenses.js
│       └── GroupBalance.js
│
└── README.md
```



## ⚙️ Setup Instructions

### 1️⃣ Backend (FastAPI)

```bash
cd backend
python -m venv venv
venv\Scripts\activate      # On Windows
pip install -r requirements.txt
uvicorn app.main:app --reload
```

> Runs at: `http://127.0.0.1:8000`

### 2️⃣ Frontend (React)

```bash
cd frontend
npm install
npm start


> Runs at: `http://localhost:3000`
            http://127.0.0.1:8000
Swagger Docs:(http://127.0.0.1:8000/docs)



## 📬 API Endpoints

| Method | Endpoint                | Description                |
| ------ | ----------------------- | -------------------------- |
| POST   | `/users/`               | Create a user              |
| POST   | `/groups/`              | Create a group             |
| POST   | `/groups/{id}/expenses` | Add expense to group       |
| GET    | `/groups/{id}/expenses` | List all expenses in group |
| GET    | `/groups/{id}/balances` | View group balances        |



## 📌 Notes

* Make sure PostgreSQL is running and properly configured
* Replace DB settings in `app/database.py` if needed
* Frontend assumes backend runs at `http://127.0.0.1:8000`



## 📷 Screenshots

![image](https://github.com/user-attachments/assets/cd9b43b5-117b-41ff-b5a0-ff9ac6150e0d)
![image](https://github.com/user-attachments/assets/b74a36c4-bc70-490d-8d78-05f0e8ba72bd)
![image](https://github.com/user-attachments/assets/1b2b8489-c7fc-470d-8dcb-96cc16932a37)






## ✍️ Author

Name: Kuppili Pravallika
Project: Splitwise Clone Assignment
Submitted to: [Cuvette (Neurix)-shivam@neurixhq.com]


