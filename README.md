# Callio Waitlist Landing Page

This folder contains the complete waitlist landing page for Callio, ready to be hosted on GitHub Pages.

## 🚀 Quick Setup for GitHub Pages

1. **Create a new GitHub repository** (or use an existing one)
2. **Upload the entire `/waitlist` folder** to your repository
3. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Set Source to "main" branch
   - Set folder to `/waitlist` (or root if you placed index.html in root)
   - Save and wait for deployment

Your site will be live at: `https://yourusername.github.io/your-repo-name/`

## 📧 Email Collection System

### How It Works

- **Local Storage:** All email addresses are saved in the browser's localStorage
- **Duplicate Prevention:** Smart detection with quirky ghost messages
- **Timestamps:** Each email is saved with date and timestamp
- **No Backend Required:** Everything works client-side

### Accessing Collected Emails

1. Navigate to your waitlist page
2. Click the small "Admin" link in the footer (nearly invisible for security)
3. Enter password: `callio2026` (change this in the code!)
4. View all collected emails with dates
5. Export to CSV for easy management

### Changing the Admin Password

In `index.html`, find this line around line 777:
```javascript
const ADMIN_PASSWORD = 'callio2026'; // Change this to your desired password
```

Replace `'callio2026'` with your secure password.

## 🎨 Features

### Ghost-Themed Messages

**Success Message (New Email):**
```
👻 Boo-yeah! You're on the list! 
We'll haunt your inbox when Callio launches.
```

**Duplicate Email Messages (Random):**
- "Boo! I already have your email. The ghost remembers! 👻"
- "Spooky! This email is already haunting our waitlist! 👻"
- "Ghost speaking: We've already got you on the list! 👻"
- "Eek! Your email already joined the spirit realm! 👻"
- "Phantom alert! This email is already registered! 👻"
- "Double trouble! Your email is already in our ghost book! 👻"

## 📄 Pages Included

All pages are in a single HTML file (Single Page Application):

1. **Home** - Hero section, features, download buttons, waitlist form
2. **FAQ** - 7 common questions with expandable answers
3. **Contact** - Email support information
4. **Privacy Policy** - Complete privacy policy (Play Store compliant)
5. **Admin** - Hidden admin panel for email management

## 🎯 Key Features

- ✅ **No Backend Required** - Pure HTML/CSS/JavaScript
- ✅ **Responsive Design** - Works on all devices
- ✅ **Email Validation** - Built-in HTML5 validation
- ✅ **Duplicate Detection** - Case-insensitive email checking
- ✅ **Timestamp Tracking** - Know when each user joined
- ✅ **CSV Export** - Download all emails easily
- ✅ **Quirky Messages** - Fun ghost-themed feedback
- ✅ **Play Store Ready** - All required pages included

## 📊 Email Data Structure

Each email is stored as:
```javascript
{
  email: "user@example.com",
  timestamp: "2026-01-24T12:34:56.789Z",
  date: "1/24/2026"
}
```

## 🔒 Security Notes

- Admin link is subtle (low opacity in footer)
- Password protection for admin access
- **Important:** Change the default password before deploying!
- Email data is stored locally in browser (consider backend for production)

## 🎨 Customization

### Colors
The site uses Callio's purple gradient theme:
- Primary: `#667eea`
- Secondary: `#764ba2`

### Support Email
Current: `support@trycallio.app`

To change, search and replace all instances of `support@trycallio.app` in `index.html`

## 📱 Mobile Optimization

- Fully responsive design
- Touch-friendly buttons and FAQ items
- Optimized text sizes for small screens
- Collapsible navigation

## 🌐 Browser Support

Works on all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Android)

## 📝 License

© 2026 Callio. All rights reserved.

---

**Need help?** Contact support@trycallio.app
