# 🏫 Kid's Kingdom Science Academy Gusau
## School Management System — Setup Guide

---

## 📦 What's Included

| File | Purpose |
|------|---------|
| `index.html` | Main application (entire system in one file) |
| `sw.js` | Service Worker — enables offline use |
| `manifest.json` | PWA manifest — enables "Add to Home Screen" |

---

## 🚀 How to Deploy

### Option A: Run Locally (Simplest)
1. Place all 3 files in one folder
2. Open `index.html` in Chrome or Edge
3. The app works immediately — data is saved in your browser (IndexedDB)

### Option B: Host on a Web Server (Recommended)
To get full PWA features (install on phone, offline access), you need HTTPS:

**Free hosting options:**
- **Netlify** (https://netlify.com) — Drag & drop the folder
- **GitHub Pages** — Free with GitHub account
- **Vercel** — Free tier available

**Steps for Netlify:**
1. Go to https://app.netlify.com/drop
2. Drag your folder onto the page
3. You'll get a live URL like `https://your-app.netlify.app`
4. Share the URL with teachers, parents and students

### Option C: Local Network Server
If you want all computers on school network to access it:
```bash
# With Python (if installed):
python -m http.server 8080

# Then visit: http://YOUR-COMPUTER-IP:8080
```

---

## 📱 Install on Phone

**Android:**
1. Open the app URL in Chrome
2. Tap the "Install" banner at the top, OR
3. Tap ⋮ menu → "Add to Home Screen"

**iPhone/iPad:**
1. Open the app URL in Safari
2. Tap the Share button (box with arrow)
3. Tap "Add to Home Screen"

---

## 🗃️ Database

All data is stored in **IndexedDB** — a built-in browser database.
- ✅ No internet required after first load
- ✅ Data persists between sessions
- ✅ Works on all modern browsers
- ⚠️ Data is stored per-device/browser (not shared between computers)

**To share data between multiple computers**, you would need a backend server.
Contact your IT team or a developer to set up a shared server if needed.

---

## 👥 User Roles
Switch roles using the buttons in the sidebar:
- 🛡️ **Admin** — Full access to all modules
- 👩‍🏫 **Teacher** — Attendance, grades, timetable
- 🎒 **Student** — View results, timetable, notices
- 👨‍👩‍👧 **Parent** — View ward's results, fees, notices

---

## 📋 Modules
1. **Dashboard** — Stats overview, recent activity
2. **Students** — Enrolment, records, search
3. **Staff** — Staff directory management
4. **Timetable** — Weekly class schedule (JSS, SSS, Primary)
5. **Attendance** — Daily marking + monthly history
6. **Grades & Reports** — Score entry + printable report cards
7. **Fee Payments** — Fee tracking, payment recording
8. **Library** — Book catalogue, borrowing records
9. **Notice Board** — Post and manage announcements

---

## 🎨 Customisation
To add your school logo:
1. Open `index.html` in a text editor
2. Find the line: `<div class="brand-logo" id="logoArea">🏫</div>`
3. Replace `🏫` with an `<img>` tag pointing to your logo file

---

## 🆘 Support
Built for Kid's Kingdom Science Academy, Gusau, Zamfara State.
For technical support, contact your system developer.
