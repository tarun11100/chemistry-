# Material Detective

A modern chemistry application with local authentication using localStorage. No backend server required.

## Features

- 🔐 **Secure Login & Signup** - All data stored locally in browser
- 💬 **AI Chatbot** - Material and chemistry queries
- 🏠 **Home Dashboard** - Welcome page after login
- 📱 **Responsive Design** - Works on all devices
- 🚀 **Vercel Ready** - One-click deployment

## Local Setup

1. Clone the repository
```bash
git clone https://github.com/tarun11100/chemistry-.git
cd chemistry-
```

2. Open in browser
```bash
# Option 1: Open login.html directly in browser
# Option 2: Use local server (Python)
python -m http.server 3000

# Option 3: Use Node.js http-server
npx http-server -p 3000
```

3. Visit `http://localhost:3000/login.html`

## Test Credentials

### Sign Up
- Create a new account with any email and password
- Credentials are stored locally in browser localStorage

### Login
- Use the same email and password you created
- You'll be redirected to the home page

## Deployment on Vercel

```bash
# Method 1: Connect GitHub repository
# 1. Push code to GitHub
# 2. Go to vercel.com
# 3. Click "New Project"
# 4. Import the GitHub repository
# 5. Click Deploy

# Method 2: Using Vercel CLI
vercel --prod
```

## Project Structure

```
.
├── login.html       # Authentication page
├── home.html        # Home page (after login)
├── chatbot.html     # AI Chatbot page
├── package.json     # Project metadata
├── vercel.json      # Vercel configuration
└── README.md        # This file
```

## Data Storage

All user data is stored in browser's **localStorage**:
- `md_users` - Array of registered users
- `md_isLoggedIn` - Login status
- `md_username` - Current user's username
- `md_email` - Current user's email

## Security Note

This is a local storage solution suitable for development/demo purposes. For production with sensitive data, implement proper backend authentication.

## Browser Support

- ✅ Chrome/Chromium
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers

## License

MIT - Free to use and modify
