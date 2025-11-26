# QUICK REFERENCE - BENIWAL CLOTHS

## 🚀 Deploy in 5 Minutes

### Step 1: Create .env File
```
SECRET_KEY=your-secret-key-here
ADMIN_PHONE=7900012929
ADMIN_TOKEN=@7900012929
GOOGLE_API_KEY=your-api-key-here
```

### Step 2: Push to GitHub
```bash
git init
git add .
git commit -m "Initial"
git remote add origin https://github.com/YOUR_USERNAME/beniwal-cloths
git push -u origin main
```

### Step 3: Deploy to Render
1. Sign up at https://render.com
2. Click "New" → "Web Service"
3. Connect GitHub repo
4. Start command: `gunicorn app:app`
5. Add environment variables (from Step 1)
6. Click Deploy

### Step 4: Access Your App
- Your app will be live at: https://your-app-name.onrender.com
- Admin login: Enter `@7900012929`

---

## 🔑 Key URLs

| URL | Purpose |
|-----|---------|
| `/` | Home page |
| `/admin/login` | Admin panel login |
| `/seller/upload` | Upload products (admin only) |
| `/product/<id>` | View product details |
| `/buy/<id>` | Checkout page |
| `/admin/dashboard` | Manage products |
| `/admin/orders` | View orders |

---

## 🛠️ Local Testing

```bash
pip install -r requirements.txt
python app.py
# Open http://localhost:5000
```

---

## 📋 Environment Variables

| Variable | Value | Required |
|----------|-------|----------|
| `SECRET_KEY` | Random 32-char string | YES |
| `ADMIN_PHONE` | 7900012929 | NO (default shown) |
| `ADMIN_TOKEN` | @7900012929 | NO (default shown) |
| `GOOGLE_API_KEY` | Your API key | NO (AI optional) |

---

## ✅ Audit Results

- No syntax errors
- All 10 templates present
- All 13 routes working
- 5 database tables verified
- Security fixes applied
- Ready for production

---

## 📞 Admin Login

**Token:** `@7900012929` or `7900012929`

That's it! No username/password needed.

---

## 🔒 Important

- `.env` file is in `.gitignore` (won't be pushed)
- Set strong `SECRET_KEY` for production
- Keep GOOGLE_API_KEY secret
- Database file is ephemeral on Render (data lost on redeploy)

---

## 🐛 Troubleshooting

| Issue | Fix |
|-------|-----|
| ModuleNotFoundError | `pip install -r requirements.txt` |
| TemplateNotFound | Check `templates/` folder exists |
| Login fails | Verify ADMIN_TOKEN in `.env` |
| AI not working | Set GOOGLE_API_KEY |

---

## 📚 Full Docs

- `DEPLOYMENT_READY.md` - Complete deployment guide
- `README_DEPLOY.md` - Detailed Render setup
- `AUDIT_REPORT.md` - Full audit findings
- `README.md` - Project overview

---

**Status:** ✅ READY FOR DEPLOYMENT

Generated: 2024-12-20
