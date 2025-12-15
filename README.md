📊 Personal Finance Tracker

A full-stack application that helps users manage income, expenses, budgets, and monthly summaries — complete with JWT authentication, budgeting analytics, and a lightweight dashboard UI.

⸻

🚀 Features

🔐 User Authentication (JWT)
	•	Secure login & registration
	•	Password hashing (BCrypt)
	•	Stateless authentication using JWT tokens

⸻

🧾 Transaction Management
	•	Add income & expenses
	•	Categorize transactions
	•	Update & delete entries
	•	Filter by category or date range

⸻

🗂️ Categories
	•	Create custom categories
	•	Set monthly & yearly budgets
	•	Track spending against limits

⸻

📈 Monthly Summary Dashboard
	•	Total income & total expenses
	•	Category-wise breakdown
	•	Budget alerts (monthly & yearly)
	•	Pie chart visualization (Chart.js)

⸻

🏛️ Tech Stack

Backend
	•	Java 17
	•	Spring Boot (Web, Security, JPA)
	•	PostgreSQL
	•	JWT Authentication
	•	Hibernate ORM
	•	Maven

Frontend (simple UI)
	•	HTML, CSS, JavaScript
	•	Chart.js
	•	Fetch API

⸻

🧩 Architecture

personal-finance-tracker/
└── backend/
    ├── controller/        → API endpoints
    ├── service/           → Business logic
    ├── repository/        → Database operations (Spring Data JPA)
    ├── dto/               → Request/response objects
    ├── mapper/            → Entity ↔ DTO conversions
    ├── model/             → JPA entities
    ├── security/          → JWT filter, config
    ├── config/            → Security & CORS setup
    ├── resources/         → application.properties
    └── Dockerfile         → Containerization support


⸻

📊 Dashboard Preview (Optional to add screenshots)

Include screenshots like:
	•	Login page
	•	Dashboard summary
	•	Category chart
	•	Budget alerts

⸻

🗄️ Database Schema (Simplified)

User
	•	id
	•	username
	•	password (hashed)

Category
	•	id
	•	name
	•	type (INCOME / EXPENSE)
	•	monthlyBudget
	•	yearlyBudget
	•	user_id (FK)

Transaction
	•	id
	•	amount
	•	description
	•	date
	•	category_id (FK)
	•	user_id (FK)

⸻

🔥 Future Enhancements (Roadmap)
	•	React frontend
	•	Recurring transactions
	•	Expense predictions using ML
	•	Multi-user dashboards
	•	Export to PDF/Excel

⸻

📦 Deployment

Supports containerized deployment via Docker:

docker build -t finance-backend .
docker run -p 8080:8080 finance-backend


⸻

🤝 Contribution

Contributions, issues, and feature requests are welcome!
Feel free to fork the repo and submit pull requests.

⸻

📄 License

MIT License
