### **Node.js & Express.js specific snippets** 
Covering everything from basic server setup to advanced patterns.

## Key Categories Included:

### 📦 **Node.js Core Modules**
- `req` - Require module
- `reqpath`, `reqfs`, `reqfsp`, `reqhttp` - Common modules
- `imp`, `impd` - ES6 imports
- `expd`, `expn` - Exports
- `mexp`, `mexpo` - Module exports

### 📁 **File System Operations**
- `nreadfile`, `nreadfilesync`, `nreadfilep` - Read files
- `nwritefile`, `nwritefilep` - Write files
- `nmkdir` - Create directory

### 🌐 **HTTP Server**
- `nserver` - Create basic HTTP server

### 🚀 **Express.js Setup**
- `exapp` - Basic Express app
- `exappfull` - Complete Express app with error handling

### 🛣️ **Express Routes**
- `exget`, `expost`, `exput`, `expatch`, `exdel` - HTTP methods
- `exasync` - Async route with error handling
- `exparams` - Route with parameters

### 🔀 **Express Router**
- `exrouter` - Basic router
- `exrouterfull` - Complete CRUD router with all operations

### 🔧 **Express Middleware**
- `exmw` - Basic middleware
- `exmwa` - Async middleware
- `exerr` - Error handling middleware
- `excors` - CORS middleware
- `exlogger` - Logger middleware
- `exauth` - Authentication middleware

### 📤 **Express Responses**
- `exjson` - JSON response
- `exstatus` - Status response
- `exerror` - Error response
- `exsendfile` - Send file
- `exredir` - Redirect

### 📂 **Static Files**
- `exstatic` - Serve static files

### 🗄️ **Mongoose (MongoDB)**
- `mgconnect` - Connect to MongoDB
- `mgschema` - Create schema
- `mgmodel` - Model CRUD operations

### 🔐 **Authentication & Security**
- `jwtsign` - Sign JWT token
- `jwtverify` - Verify JWT token
- `bchash` - Hash password with bcrypt
- `bccompare` - Compare password with bcrypt

### ⚙️ **Configuration**
- `dotenv`, `dotenvpath` - Load environment variables
- `penv` - Access environment variable
- `pexit` - Exit process

### 🔄 **Async Patterns**
- `asynchandler` - Async handler wrapper
- `useasync` - Use async handler

### ✅ **Validation**
- `exvalidate` - Express validator middleware

### 📤 **File Upload**
- `multer` - Multer setup
- `multersingle` - Single file upload

### 📊 **Logging**
- `morgan` - Morgan logger

### 📧 **Email**
- `nodemailer` - Nodemailer setup

### 🌐 **HTTP Client**
- `axiosget` - Axios GET request
- `axiospost` - Axios POST request

## Installation:
1. Open VSCode
2. Press `Ctrl+Shift+P` / `Cmd+Shift+P`
3. Type "Configure User Snippets"
4. Select `javascript.json` or create `nodejsSnippets.json`
5. Paste the content

## Common Workflow Examples:

**Creating a new API:**
1. `exappfull` - Set up Express app
2. `exrouterfull` - Create CRUD router
3. `mgschema` - Define database schema
4. `exauth` - Add authentication middleware

**Setting up authentication:**
1. `dotenv` - Load environment variables
2. `bchash` - Hash passwords
3. `jwtsign` - Create tokens
4. `exauth` - Protect routes

**File operations:**
1. `nreadfilep` - Read files
2. `nwritefilep` - Write files
3. `multer` - Handle uploads

These snippets will dramatically speed up your Node.js and Express.js development! 🚀💻
