# AI-Powered Azure Chaos Engineering Web App

A comprehensive chaos engineering platform that integrates AI-powered architecture analysis with Azure Chaos Studio for resilience testing and monitoring.

## 🚀 Quick Start

### ✨ One-Click Setup (Recommended)
```bash
# Complete modern setup with compatibility fixes
setup-complete.bat
```

### 📊 Check Installation Status
```bash
# See what's installed and what's missing
quick-status.bat
```

### 🚀 Start Application
```bash
# Start both backend and frontend services
start-all.bat

# Or start individually
start-backend.bat
start-frontend.bat
```

### 🔍 Access Your Application
- **Frontend**: http://localhost:3000
- **Backend API**: http://localhost:8000  
- **API Documentation**: http://localhost:8000/docs

## 🛠️ Setup Options

| Script | Purpose | Best For |
|--------|---------|----------|
| `setup-complete.bat` | **Complete setup** with modern compatibility | ✅ **New installations & backup restoration** |
| `setup-fix.bat` | Setup with enhanced compatibility fixes | Version conflicts & troubleshooting |
| `quick-status.bat` | Check installation status | Diagnosing issues |
| `validate-setup.bat` | Detailed validation | After setup completion |
| `integration-test.bat` | **Complete platform testing** | Final verification & testing |

## 💾 Backup & Restoration

### Creating Backups
```bash
# Create complete project backup with restoration script
backup-complete.bat
```

### Restoring from Backup  
1. **Extract backup** to desired location
2. **Run restoration**:
   ```bash
   # Use provided restoration script from backup
   RESTORE.bat
   
   # Or manual setup
   setup-complete.bat
   ```

### Testing Complete Setup
```bash
# Run comprehensive platform test
integration-test.bat
```

## 🔧 System Requirements

- **Node.js 18+** (tested with 24.2.0)
- **Python 3.13+** (tested with 3.13.2)  
- **Windows 10/11**
- **PowerShell 5.1+** or Command Prompt

📖 **Complete Setup Guide:** See `SETUP_GUIDE_COMPLETE.md` for comprehensive instructions.
🔧 **Troubleshooting:** See `SETUP_TROUBLESHOOTING.md` for common issues.
🎉 **Modernization Status:** See `MODERNIZATION_COMPLETE.md` for full automation details.

## ✨ Features

### 🤖 AI-Powered Analysis
- **Architecture Diagram Analysis**: Upload and analyze system architecture diagrams
- **Intelligent Experiment Generation**: AI suggests optimal chaos experiments
- **Risk Assessment**: ML-driven risk analysis and impact prediction
- **Performance Optimization**: AI recommendations for system improvements

### ☁️ Azure Integration
- **Chaos Studio Integration**: Native Azure Chaos Studio support
- **Resource Discovery**: Automatic Azure resource detection
- **Multi-Subscription Support**: Manage resources across subscriptions
- **Azure AD Authentication**: Secure enterprise authentication

### 📊 Real-Time Monitoring
- **Live Metrics Dashboard**: Real-time experiment monitoring
- **Intelligent Alerting**: Smart alerts based on experiment status
- **Custom Dashboards**: Configurable monitoring views
- **Performance Tracking**: Detailed metrics and trends

### 🚀 Advanced Platform Features
- **Plugin Marketplace**: Extensible plugin ecosystem
- **Multi-User Collaboration**: Team-based experiment management
- **Role-Based Access Control**: Granular permission system
- **Audit Logging**: Complete activity tracking
- **CI/CD Integration**: Seamless pipeline integration
- **Comprehensive Reporting**: Automated report generation

### 🎨 Modern User Experience
- **Responsive Design**: Mobile-first, responsive interface
- **Dark/Light Themes**: Customizable UI themes
- **Real-Time Updates**: Live data with React Query
- **Intuitive Navigation**: User-friendly interface design

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                    Frontend (React 18)                      │
├─────────────────────────────────────────────────────────────┤
│ ├── Dashboard & Real-time Monitoring                        │
│ ├── Experiment Builder & Management                         │
│ ├── AI-Powered Architecture Analysis                        │
│ ├── Plugin Marketplace & Settings                           │
│ └── Reports & Analytics                                     │
└─────────────────────────────────────────────────────────────┘
                              │
                              │ REST API / WebSocket
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                   Backend (FastAPI)                        │
├─────────────────────────────────────────────────────────────┤
│ ├── Azure Services Integration                              │
│ ├── AI/ML Services (OpenAI, Azure Cognitive)              │
│ ├── Experiment Management & Orchestration                  │
│ ├── Real-time Monitoring & Alerting                       │
│ ├── Authentication & Authorization                         │
│ └── Plugin System & Marketplace                           │
└─────────────────────────────────────────────────────────────┘
                              │
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                   Azure Infrastructure                     │
├─────────────────────────────────────────────────────────────┤
│ ├── App Service (Backend API)                              │
│ ├── Static Web Apps (Frontend)                             │
│ ├── PostgreSQL (Primary Database)                          │
│ ├── Blob Storage (File Storage)                            │
│ ├── Key Vault (Secrets Management)                         │
│ ├── Application Insights (Monitoring)                      │
│ └── Chaos Studio (Chaos Engineering)                       │
└─────────────────────────────────────────────────────────────┘
```

## 🚀 Quick Start

## 🛠️ Prerequisites

- **Node.js 18+** and npm (⚠️ Node.js 24+ requires compatibility fixes)
- **Python 3.9+** and pip (⚠️ Python 3.13+ requires compatibility handling)
- **Azure subscription** with appropriate permissions
- **Azure CLI** (for deployment)
- **Git** for version control

### 🔧 Automated Setup

The fastest way to get started with compatibility fixes:

```bash
# Clone the repository
git clone <repository-url>
cd chaos-engineering-app

# Windows (Recommended - includes compatibility fixes)
.\setup-fix.bat

# If setup-fix.bat is not available, use original setup
.\setup.bat

# Unix/Linux/macOS  
chmod +x setup.sh && ./setup.sh
```

### 🚨 Common Setup Issues & Quick Fixes

**NPM Peer Dependency Errors (Node.js 24+):**
```bash
.\npm-fix.bat
```

**Setup Script Failures:**
```bash
.\setup-fix.bat  # Use this instead of setup.bat
```

**Manual Frontend Fix:**
```bash
cd frontend
npm cache clean --force
npm install --legacy-peer-deps --force
```

### 🏃‍♂️ Start Development

```bash
# Start both backend and frontend
.\start-all.bat        # Windows
./start-all.sh         # Unix/Linux/macOS

# Or start individually  
.\start-backend-dev.bat  # Backend with auto-reload
.\start-frontend-dev.bat # Frontend with hot reload (includes Node.js 24 fixes)
```

### 🌐 Access the Application

- **Frontend**: http://localhost:3000
- **Backend API**: http://localhost:8000  
- **API Documentation**: http://localhost:8000/docs
- **Interactive API**: http://localhost:8000/redoc

### Backend Setup (Manual)

```bash
cd backend
python -m venv venv
venv\Scripts\activate  # On Windows
# source venv/bin/activate  # On Unix/Linux/macOS
pip install --upgrade pip wheel setuptools
pip install -r requirements.txt --force-reinstall  # For Python 3.13+ compatibility
uvicorn main:app --reload
```

### Frontend Setup (Manual)

```bash
cd frontend
npm cache clean --force  # Clean cache for Node.js 24+
npm install --legacy-peer-deps --force  # For Node.js 24+ compatibility
# Set NODE_OPTIONS=--openssl-legacy-provider  # For Node.js 17+
npm start
```

## 📋 Complete Documentation

### 📖 Setup and Installation
- **[Complete Setup Guide](docs/COMPLETE_SETUP_GUIDE.md)** - Comprehensive installation and setup instructions
- **[Setup Troubleshooting Guide](SETUP_TROUBLESHOOTING.md)** - Common setup issues and fixes
- **[Backup and Restoration Guide](docs/BACKUP_AND_RESTORATION_GUIDE.md)** - Creating and restoring project backups
- **[Azure Authentication Guide](docs/AZURE_AUTHENTICATION_GUIDE.md)** - Setting up Azure AD authentication
- **[Azure Real Data Setup Guide](docs/AZURE_REAL_DATA_SETUP_GUIDE.md)** - Configuring real Azure resources

### 🛠️ Development and Deployment
- **[Development Guide](docs/DEVELOPMENT.md)** - Development guidelines and best practices
- **[Deployment Guide](docs/DEPLOYMENT_GUIDE.md)** - Production deployment instructions
- **[Testing Guide](docs/TESTING_GUIDE.md)** - Testing procedures and guidelines

### 🔧 Available Scripts

The project includes several convenient scripts for common tasks:

#### Setup and Installation
- `setup-complete.bat` - **✅ RECOMMENDED** Complete modern setup with compatibility
- `setup-fix.bat` - Setup with enhanced compatibility fixes  
- `setup.bat` - Standard setup (legacy)
- `install-backend.bat` - Install Python backend only
- `install-frontend.bat` - Install React frontend only

#### Status and Validation
- `quick-status.bat` - **✅ RECOMMENDED** Check installation status
- `validate-setup.bat` - Detailed setup validation
- `GET_STARTED.bat` - Interactive setup guide

#### Running the Application
- `start-all.bat` - **✅ RECOMMENDED** Start both services
- `start-backend.bat` - Start backend service only
- `start-frontend.bat` - Start frontend service only
- `start-backend-dev.bat` - Backend development mode
- `start-frontend-dev.bat` - Frontend development mode
- `stop-all.bat` - Stop all running services

#### Backup and Maintenance
- `backup-complete.bat` - **✅ NEW** Complete project backup with restoration
- `quick-backup.bat` - Quick backup for sharing
- `backup-app.bat` - Application backup

#### Azure Integration
- `get-azure-token.bat` - Get Azure authentication token

## 🛡️ Tested Compatibility

✅ **Verified Working With:**
- Node.js 24.2.0 (latest)
- Python 3.13.2 (latest) 
- Windows 10/11
- PowerShell 5.1+
- npm 11.3.0+

✅ **Modern Features:**
- Legacy peer dependencies handling
- Python 3.13 compatibility
- Virtual environment auto-recreation
- Backup restoration system

## 🤝 Contributing

We welcome contributions! Please see our contributing guidelines:

1. **Fork the repository** and create a feature branch
2. **Make your changes** with comprehensive tests
3. **Follow code style** guidelines (Prettier for frontend, Black for backend)
4. **Update documentation** as needed
5. **Submit a pull request** with a clear description

### Development Guidelines
- Follow TypeScript best practices for frontend
- Use async/await patterns for backend
- Write comprehensive tests for new features
- Update API documentation for backend changes
- Ensure responsive design for UI changes

## � Project Structure

```
chaos-engineering-app/
├── backend/                    # Python FastAPI backend
│   ├── main.py                # Main application entry point
│   ├── config.py              # Configuration settings
│   ├── requirements.txt       # Python dependencies
│   ├── models/               # Database models
│   ├── routers/              # API route handlers
│   ├── schemas/              # Pydantic schemas
│   └── services/             # Business logic
├── frontend/                  # React TypeScript frontend
│   ├── src/                  # Source code
│   │   ├── components/       # React components
│   │   ├── pages/           # Page components
│   │   ├── services/        # API services
│   │   └── utils/           # Utilities
│   ├── public/              # Static assets
│   └── package.json         # Node.js dependencies
├── docs/                     # Comprehensive documentation
│   ├── COMPLETE_SETUP_GUIDE.md
│   ├── BACKUP_AND_RESTORATION_GUIDE.md
│   ├── AZURE_AUTHENTICATION_GUIDE.md
│   ├── DEVELOPMENT.md
│   └── DEPLOYMENT_GUIDE.md
├── infrastructure/           # Azure infrastructure code
├── setup.bat                # Automated setup script
├── start-all.bat            # Launch all services
└── backup scripts           # Project backup utilities
```

## 🚀 Getting Started Guide

### For First-Time Setup
1. **Prerequisites:** Ensure Node.js (16+) and Python (3.8+) are installed
2. **Setup:** Run `setup.bat` in the project root
3. **Start:** Run `start-all.bat` to launch the application
4. **Access:** Open http://localhost:3000 in your browser
5. **Validate:** Run `validate-setup.bat` to verify everything works

### For Colleagues Using Backup
1. **Extract:** Unzip the backup archive to your desired location
2. **Navigate:** Open terminal in the `chaos-engineering-app` folder
3. **Setup:** Run `setup.bat` (this installs all dependencies automatically)
4. **Launch:** Run `start-all.bat` to start both services
5. **Verify:** Check that http://localhost:3000 loads correctly

**📖 Need help?** See `docs/COMPLETE_SETUP_GUIDE.md` for detailed instructions.

## 🔄 Creating and Sharing Backups

### Quick Backup for Colleagues
```cmd
# Creates a clean, shareable backup
quick-backup.bat
```

### What's Included in Backups
- ✅ All source code (backend + frontend)
- ✅ Configuration files and documentation
- ✅ Setup and launch scripts
- ✅ Package configurations (package.json, requirements.txt)

### What's Excluded from Backups
- ❌ Virtual environments (`venv/`)
- ❌ Node modules (`node_modules/`)
- ❌ Build artifacts and cache files
- ❌ Environment files with secrets

**📖 Complete backup guide:** See `docs/BACKUP_AND_RESTORATION_GUIDE.md`

## 🐛 Troubleshooting

### Common Issues and Solutions

1. **Setup script fails:**
   - Ensure Node.js and Python are properly installed
   - Run as administrator if permission issues occur
   - Check `validate-setup.bat` output for specific errors

2. **Services won't start:**
   - Check if ports 3000 and 8000 are available
   - Verify virtual environment activation
   - Review terminal output for specific error messages

3. **Azure authentication issues:**
   - Follow `docs/AZURE_AUTHENTICATION_GUIDE.md`
   - Verify Azure AD app registration settings
   - Check browser console for authentication errors

4. **Dependencies not installing:**
   ```cmd
   # Backend: Recreate virtual environment
   rmdir /s backend\venv
   cd backend && python -m venv venv

   # Frontend: Clear cache and reinstall
   cd frontend && npm cache clean --force && npm install
   ```

### Getting Help
- 📖 **Documentation:** Check the `docs/` folder for detailed guides
- 🔍 **Validation:** Run `validate-setup.bat` to diagnose issues
- 🌐 **API Docs:** Visit http://localhost:8000/docs when backend is running
- 🛠️ **Development:** See `docs/DEVELOPMENT.md` for development guidelines

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Azure Chaos Studio** team for excellent chaos engineering tools
- **FastAPI** and **React** communities for outstanding frameworks
- **OpenAI** for powerful AI capabilities
- **Contributors** who help make this project better

---

## 🚀 Ready to Get Started?

1. **Clone the repository**
2. **Run the setup script** for your platform
3. **Start the development servers**
4. **Open http://localhost:3000** and begin chaos engineering!

For detailed setup instructions, see the [Development Guide](DEVELOPMENT.md).

**Happy Chaos Engineering! 🎯**

## 💻 Technology Stack

### Frontend
- **React 18** with TypeScript for type-safe development
- **Tailwind CSS** for utility-first styling
- **Redux Toolkit** for predictable state management
- **React Query (TanStack Query)** for server state management
- **React Router** for client-side routing
- **MSAL** for Azure AD authentication
- **Lucide React** for consistent iconography

### Backend  
- **FastAPI** for high-performance async API
- **SQLAlchemy** for database ORM
- **Pydantic** for data validation and serialization
- **Azure SDK** for comprehensive Azure integration
- **OpenAI API** for AI-powered analysis
- **PostgreSQL** for production database
- **Redis** for caching and session management

### Infrastructure & DevOps
- **Azure App Service** for backend hosting
- **Azure Static Web Apps** for frontend hosting
- **GitHub Actions** for CI/CD automation
- **ARM Templates** for infrastructure as code
- **Azure Application Insights** for monitoring
- **Docker** for containerization

## 📱 User Interface

### 🎛️ Dashboard
- Real-time experiment status monitoring
- System health overview with live metrics
- Recent activity feed and notifications
- Quick access to common actions

### 🧪 Experiment Management
- Intuitive experiment creation wizard
- Template-based experiment setup
- Drag-and-drop experiment builder
- Advanced scheduling and automation

### 🤖 AI Analysis
- Upload architecture diagrams for analysis
- AI-generated experiment recommendations
- Risk assessment and impact analysis
- Intelligent optimization suggestions

### 📊 Monitoring & Reporting
- Real-time metrics dashboard
- Customizable alert configuration
- Automated report generation
- Historical trend analysis

### 🔌 Plugin Marketplace
- Browse available plugins by category
- Install/uninstall with one click
- Plugin configuration management
- Custom plugin development tools

### ⚙️ Settings & Administration
- User preference management
- Organization settings and policies
- Integration configuration
- Security and compliance controls

## 🔐 Security & Compliance

- **Azure AD Integration** for enterprise authentication
- **Role-Based Access Control (RBAC)** with granular permissions
- **Multi-Factor Authentication (MFA)** support
- **Audit Logging** for compliance and security
- **Data Encryption** at rest and in transit
- **Secret Management** with Azure Key Vault

## 🚀 Deployment Options

### 📋 Manual Setup
