# Automis AI Platform - Modern SaaS Design

Professional, clean, analytics-ready platform for AI-powered voice agents.

## 🎨 Design Features

### **Modern SaaS Aesthetic**
- ✅ Light, clean theme with professional typography
- ✅ Subtle gradients and shadows
- ✅ Clear visual hierarchy
- ✅ White space emphasis
- ✅ Consistent component library

### **Color Palette**
- **Primary**: #6366f1 (Indigo) - Professional and trustworthy
- **Accent**: #f59e0b (Amber) - Warm and inviting
- **Success**: #10b981 (Emerald)
- **Error**: #ef4444 (Red)
- **Neutrals**: Tailwind-inspired gray scale

### **Key Features**
- 📊 Analytics-ready dashboard layout
- 📱 Fully responsive (mobile-first design)
- 🎯 Mission control-style interface
- ⚡ Smooth micro-interactions
- 🔍 Clear data visualization
- 🎨 Professional gradients (subtle, not heavy)

## 📁 Project Structure

```
design/
├── components/
│   ├── design.css          ← Main stylesheet (Modern SaaS)
│   ├── home.html           ← Landing page
│   ├── login.html          ← Authentication
│   ├── dashboard.html      ← Call Dashboard
│   ├── agents.html         ← AI Agents Management
│   ├── call-logs.html      ← Call Logs & Filters
│   ├── analytics.html      ← Analytics & Reports
│   └── settings.html       ← Account Settings
├── index.html              ← Entry point (redirects to home)
├── vercel.json             ← Vercel configuration
├── styles.css              ← Original CSS (preserved)
└── README.md               ← This file
```

## 🚀 Deploy to Vercel

### **Method 1: Vercel CLI** (Recommended)

1. **Install Vercel CLI**
```bash
npm install -g vercel
```

2. **Navigate to project**
```bash
cd H:\design
```

3. **Deploy**
```bash
vercel
```

4. **Follow prompts:**
   - Set up and deploy? **Y**
   - Which scope? (Select your account)
   - Link to existing project? **N**
   - What's your project's name? `automis-ai-platform`
   - In which directory is your code located? `./`
   - Want to override settings? **N**

5. **Production deployment**
```bash
vercel --prod
```

### **Method 2: GitHub + Vercel Dashboard**

1. **Push to GitHub**
```bash
cd H:\design
git init
git add .
git commit -m "Initial commit - Automis AI Platform"
git remote add origin <your-github-repo-url>
git push -u origin main
```

2. **Import on Vercel**
   - Go to [vercel.com/new](https://vercel.com/new)
   - Import your GitHub repository
   - Click **Deploy**
   - Done! Your site is live

### **Method 3: Drag & Drop**

1. Go to [vercel.com/new](https://vercel.com/new)
2. Drag the entire `design` folder
3. Click **Deploy**
4. Your site is live!

## 🌐 Navigation Structure

```
Home (index.html) → components/home.html
    ↓
Login → components/login.html
    ↓
Dashboard → components/dashboard.html
    ├── Agents → components/agents.html
    ├── Call Logs → components/call-logs.html
    ├── Analytics → components/analytics.html
    └── Settings → components/settings.html
```

## 📱 Pages Overview

### 1. **Home Page** (`components/home.html`)
- Hero section with gradient background
- Features showcase (6 cards)
- CTA section
- Footer

### 2. **Login Page** (`components/login.html`)
- Email/password authentication
- Login/Register tab switcher
- Clean, centered design
- Subtle gradient background

### 3. **Dashboard** (`components/dashboard.html`)
- 4 KPI cards (Calls Today/Week/Month/Year)
- Call statistics (Success/Failed)
- Minute quota with progress bar
- Ready for charts integration

### 4. **Agents** (`components/agents.html`)
- Create new agents modal
- Agent cards grid
- Empty state design
- Agent configuration form

### 5. **Call Logs** (`components/call-logs.html`)
- Advanced filters (Agent, Phone, Date, Status)
- Export options (PDF/TXT)
- Search functionality
- Call logs table (ready for data)

### 6. **Analytics** (`components/analytics.html`)
- Call volume trend chart placeholder
- Success rate visualization
- Average call duration metric
- Peak hours bar chart
- Agent performance table
- Time range filters

### 7. **Settings** (`components/settings.html`)
- Account information
- Password change
- Notification toggles
- Billing & subscription
- API keys
- Danger zone (account deletion)

## 🎯 Design Principles

Based on the UX redesign brief:

✅ **Modern SaaS Look** - Clean cards, professional typography
✅ **Futuristic Yet Professional** - Subtle gradients, not heavy effects
✅ **Clear Hierarchy** - Strong typography scale, proper spacing
✅ **White Space** - Emphasis on breathing room
✅ **Mission Control** - Dashboard-centric design
✅ **Analytics Ready** - Prepared for rich data visualization
✅ **Scalable** - Easy to add new features

## 🛠️ Customization

### **Change Colors**
Edit CSS variables in `components/design.css`:
```css
:root {
    --color-primary: #6366f1;    /* Your brand color */
    --color-accent: #f59e0b;     /* Accent color */
    /* ... */
}
```

### **Add Your Logo**
Replace the SVG logo in header sections of each HTML file.

### **Connect Backend**
- Forms are ready for API integration
- Add your endpoints to JavaScript sections
- Update data fetching logic

## 📊 Integrating Real Data

### **Dashboard Stats**
```javascript
// Example: Update call statistics
fetch('/api/dashboard/stats')
    .then(res => res.json())
    .then(data => {
        document.querySelector('.stat-card .value').textContent = data.callsToday;
    });
```

### **Charts Integration**
Ready for libraries like:
- Chart.js
- Recharts
- ApexCharts
- D3.js

Placeholder elements with class `.chart-placeholder` are ready.

## 🔧 Development

### **Local Development**
Simply open `index.html` in a browser, or use a local server:

```bash
# Python
python -m http.server 8000

# Node.js
npx serve

# PHP
php -S localhost:8000
```

Then visit: `http://localhost:8000`

## ✨ Features

- ✅ **Zero Dependencies** - Pure HTML/CSS/JS
- ✅ **Fast Loading** - Optimized assets
- ✅ **SEO Ready** - Proper meta tags
- ✅ **Accessible** - Semantic HTML
- ✅ **Mobile First** - Responsive design
- ✅ **Production Ready** - Vercel optimized

## 📝 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers

## 🚨 Important Notes

- All pages use `design.css` for styling
- `styles.css` is preserved but not used
- Navigation is client-side (no backend required)
- Forms don't submit (add your API endpoints)
- Charts are placeholders (integrate your library)

## 📞 Support

For issues or questions:
- Check Vercel docs: https://vercel.com/docs
- Review design requirements: `Automis_UX_Redesign_Brief_and_Screens_v2.docx`

## 🎉 Ready to Deploy!

Your Automis AI Platform is ready for production. Just deploy to Vercel and share your link!

---

**Built with modern SaaS design principles**
**Optimized for Vercel deployment**
**Production-ready code**
