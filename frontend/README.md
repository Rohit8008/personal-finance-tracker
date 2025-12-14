# Finance Tracker Frontend

A modern, professional frontend for the Personal Finance Tracker application.

## Features

### 🎨 Professional UI
- Modern, clean design with a consistent color scheme
- Responsive layout that works on all devices
- Smooth transitions and hover effects
- Professional typography and spacing

### 📊 Complete API Integration
- **Authentication**: Login and Registration
- **Dashboard**: Monthly/yearly summaries with charts and budget alerts
- **Transactions**: View, add, and filter all transactions
- **Expenses**: Manage expenses with category tracking
- **Incomes**: Track income sources
- **Categories**: Create and manage categories with budget limits
- **Analytics**: Detailed analytics with charts and summaries

### 🔐 Security
- JWT token-based authentication
- Automatic token validation
- Secure API calls with proper headers
- Auto-redirect to login when session expires

### ✨ User Experience
- Loading states for all async operations
- Error handling with user-friendly messages
- Success notifications
- Empty states for better UX
- Form validation
- Date pickers and filters

## Pages

1. **Login** (`login.html`) - User authentication
2. **Register** (`register.html`) - New user registration
3. **Dashboard** (`index.html`) - Overview with stats, charts, and alerts
4. **Transactions** (`transactions.html`) - All transactions with filtering
5. **Expenses** (`expenses.html`) - Expense management
6. **Incomes** (`incomes.html`) - Income tracking
7. **Categories** (`categories.html`) - Category management
8. **Analytics** (`summary.html`) - Detailed analytics and reports

## File Structure

```
frontend/
├── index.html          # Dashboard
├── login.html          # Login page
├── register.html       # Registration page
├── transactions.html  # Transactions page
├── expenses.html       # Expenses page
├── incomes.html        # Incomes page
├── categories.html     # Categories page
├── summary.html        # Analytics page
├── app.js              # API functions and utilities
├── styles.css          # Global styles
└── README.md           # This file
```

## API Endpoints Used

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user

### User
- `GET /api/users/me` - Get current user

### Transactions
- `GET /api/transactions` - Get all transactions
- `POST /api/transactions` - Add transaction
- `GET /api/transactions/filter` - Filter transactions

### Expenses
- `GET /api/expenses/my` - Get user expenses
- `POST /api/expenses` - Add expense

### Incomes
- `GET /api/incomes/user/{userId}` - Get user incomes
- `POST /api/incomes` - Add income

### Categories
- `GET /api/category` - Get all categories
- `POST /api/category` - Create category

### Summary
- `GET /api/summary/monthly` - Monthly summary
- `GET /api/summary/yearly` - Yearly summary
- `GET /api/summary/budget-alerts` - Budget alerts

## Usage

1. Open `login.html` in a web browser
2. Register a new account or login
3. Navigate through the application using the top navigation
4. Add transactions, expenses, incomes, and categories
5. View analytics and summaries on the Dashboard and Analytics pages

## Configuration

Update the `API_BASE_URL` in `app.js` if your backend is running on a different port:

```javascript
const API_BASE_URL = 'http://localhost:8080/api';
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Dependencies

- Chart.js (via CDN) - For charts and graphs
- No build process required - Pure HTML/CSS/JavaScript
