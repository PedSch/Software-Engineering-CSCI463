# CSCI463 - Software Engineering

## Login Application

A Windows Forms login application with both desktop and web implementations.

### Files
- **Login/Login/** - C# Windows Forms desktop application
- **Login/web-login.html** - Modern web-based login interface

---

## 🖥️ Desktop Application (Windows Forms)

### Requirements
- Windows OS
- Visual Studio 2015 or later
- .NET Framework 4.5 or later

### How to Compile and Run

**Option 1: Using Visual Studio**
1. Open `Login/Login.sln` in Visual Studio
2. Press `F5` or click the "Start" button
3. The application will compile and run automatically

**Option 2: Using MSBuild (Command Line)**
```bash
# Navigate to the solution directory
cd Login

# Build the solution
msbuild Login.sln

# Run the compiled executable
cd Login/bin/Debug
Login.exe
```

**Option 3: Using Developer Command Prompt**
```bash
# Open "Developer Command Prompt for VS"
cd path\to\Login
msbuild Login.sln /p:Configuration=Release
```

### Features
- Username and password fields with placeholder text
- Password masking when typing
- Interactive placeholder behavior (clears on focus)
- Login button with success message
- Centered, borderless form design

---

## 🌐 Web Application

### How to Run

**Option 1: Direct Browser Open**
1. Navigate to `Login/web-login.html`
2. Right-click and select "Open with" → your browser
3. Or double-click the file to open in default browser

**Option 2: Using a Local Server**
```bash
# Using Python
cd Login
python3 -m http.server 8000
# Open browser to: http://localhost:8000/web-login.html

# Using Node.js (if you have http-server installed)
npx http-server Login -p 8000
# Open browser to: http://localhost:8000/web-login.html

# Using PHP
cd Login
php -S localhost:8000
# Open browser to: http://localhost:8000/web-login.html
```

**Option 3: Using VS Code Live Server**
1. Install "Live Server" extension in VS Code
2. Right-click `web-login.html`
3. Select "Open with Live Server"

### Web Features
- ✨ Modern purple gradient design with animations
- 🔐 Form validation (required fields)
- 👁️ Password show/hide toggle
- 📱 Responsive and mobile-friendly
- 🎯 Interactive hover effects
- ✅ Success modal with animations
- 🔗 "Forgot Password" functionality (demo)

---

## Project Structure
```
Software-Engineering-CSCI463/
├── README.md
├── hw1/                          # Homework 1 documentation (PDFs)
├── term project/                 # Term project documentation
└── Login/
    ├── Login.sln                 # Visual Studio solution file
    ├── web-login.html            # Web-based login (NEW)
    └── Login/
        ├── Form1.cs              # Main form logic
        ├── Form1.Designer.cs     # Form UI design
        ├── Program.cs            # Application entry point
        ├── Login.csproj          # Project file
        └── Properties/           # Assembly info and resources
```

---

## 🔧 Recent Updates

### Desktop Application (Form1.cs)
- ✅ Fixed all event handler wiring
- ✅ Added proper placeholder text initialization
- ✅ Improved password masking behavior
- ✅ Fixed placeholder restoration logic
- ✅ Removed trailing spaces from placeholders

### Web Application (web-login.html)
- ✅ Created modern, responsive web interface
- ✅ Added form validation
- ✅ Implemented password toggle feature
- ✅ Added smooth animations and transitions
- ✅ Professional gradient color scheme

---

## 📝 Notes

- The desktop application is designed for Windows and requires Visual Studio or .NET Framework
- The web version works on any platform with a modern browser
- Both implementations provide the same core login functionality
- The web version includes additional features like validation and password visibility toggle