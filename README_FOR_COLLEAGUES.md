# 🚀 Azure Chaos Engineering Platform - Setup for Colleagues

## 📋 Quick Start (5 Minutes Setup)

This platform is **fully tested and ready** with comprehensive dependency management. Follow these steps for a smooth installation:

### 1. Prerequisites

**Required Software:**
- **Python 3.13+** (tested with 3.13.2) - [Download here](https://python.org/)
- **Node.js 24+** (tested with v24.2.0) - [Download here](https://nodejs.org/)
- **Git** (for cloning/updates)

**Verify Installation:**
```cmd
python --version  # Should show 3.13+
node --version    # Should show v24+
npm --version     # Should work
```

### 2. One-Command Setup

**Clone and run the setup:**
```cmd
git clone [repository-url]
cd chaos-engineering-platform
setup-complete.bat
```

**That's it!** The script will:
- ✅ Install ALL Python dependencies (including aiosqlite, email-validator, OpenAI, Azure SDK)
- ✅ Install ALL Node.js dependencies with compatibility fixes
- ✅ Create configuration files with placeholders
- ✅ Validate everything works

### 3. Start the Application

```cmd
start-all.bat
```

**Access Points:**
- **Frontend:** http://localhost:3000
- **Backend API:** http://localhost:8000
- **API Documentation:** http://localhost:8000/docs

## 🛠️ Configuration (After Setup)

### Backend Configuration
Edit `backend\.env` and update these variables:
```env
# Required for full functionality
AZURE_SUBSCRIPTION_ID=your_subscription_id_here
AZURE_TENANT_ID=your_tenant_id_here
AZURE_CLIENT_ID=your_client_id_here
AZURE_CLIENT_SECRET=your_client_secret_here

# Required for AI features
OPENAI_API_KEY=your_openai_key_here

# Required for blob storage
BLOB_STORAGE_CONNECTION=your_blob_connection_here
```

## 🆘 Common Issues & Solutions

### Issue: "aiosqlite not found" or similar import errors
**Solution:** This is already fixed! The setup script installs ALL required dependencies.

### Issue: Node.js compatibility warnings
**Solution:** The setup uses `--legacy-peer-deps` flag for compatibility.

### Issue: Python virtual environment issues
**Solution:** The script automatically cleans and recreates the venv.

### Issue: Permission errors on Windows
**Solution:** Run Command Prompt as Administrator.

## 📁 Project Structure

```
chaos-engineering-platform/
├── backend/              # Python FastAPI backend
│   ├── venv/            # Virtual environment (auto-created)
│   ├── .env            # Configuration file
│   ├── requirements.txt # All Python dependencies
│   └── main.py         # FastAPI application
├── frontend/            # React TypeScript frontend
│   ├── node_modules/   # Dependencies (auto-created)
│   ├── src/            # Source code
│   └── public/         # Static assets
├── setup-complete.bat  # ONE-COMMAND SETUP
├── start-all.bat      # Start both services
├── start-backend.bat  # Start backend only
└── start-frontend.bat # Start frontend only
```

## 🔧 Individual Service Management

### Backend Only:
```cmd
start-backend.bat
# Access at: http://localhost:8000
```

### Frontend Only:
```cmd
start-frontend.bat
# Access at: http://localhost:3000
```

### Stop All Services:
```cmd
stop-all.bat
```

## 📚 Additional Resources

- **Troubleshooting:** `DEPENDENCY_TROUBLESHOOTING.md`
- **Full Documentation:** `docs/` folder
- **Development Guide:** `docs/DEVELOPMENT.md`
- **Azure Setup:** `docs/AZURE_AUTHENTICATION_GUIDE.md`

## 💡 Pro Tips

1. **First Time Setup:** Always run `setup-complete.bat` first
2. **Updates:** Re-run `setup-complete.bat` when pulling new changes
3. **Issues:** Check `DEPENDENCY_TROUBLESHOOTING.md` for specific error solutions
4. **Development:** Use individual start scripts for faster development

## ✅ Tested Environments

- ✅ Windows 10/11
- ✅ Python 3.13.2
- ✅ Node.js v24.2.0
- ✅ npm 10.8.2
- ✅ Modern Command Prompt and PowerShell

## 🆘 Need Help?

If you encounter any issues:
1. Check `DEPENDENCY_TROUBLESHOOTING.md`
2. Run `quick-status.bat` for diagnostics
3. Contact the project maintainer with error details

---
**This setup has been thoroughly tested and debugged. Your installation should work smoothly! 🎉**
