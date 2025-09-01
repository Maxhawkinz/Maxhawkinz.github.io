# 🚀 Portfolio Deployment Guide

## 📋 **What You'll Get**
- **Live Website**: `https://yourusername.github.io`
- **Working Contact Form**: Sends emails to your Gmail
- **Professional Portfolio**: Accessible worldwide

---

## 🎯 **Step 1: GitHub Repository Setup**

### 1.1 Create Repository
1. Go to [github.com](https://github.com) and sign in
2. Click the **"+"** icon → **"New repository"**
3. **Repository name**: `yourusername.github.io` (replace with your actual username)
4. **Make it Public** ✅
5. Click **"Create repository"**

### 1.2 Upload Files
1. In your new repository, click **"uploading an existing file"**
2. **Drag and drop** all these files:
   - `index.html`
   - `skills.html`
   - `education.html`
   - `experience.html`
   - `certificates.html`
   - `contact.html`
   - `style.css`
   - `main.jpg`
3. **Commit message**: "Initial portfolio upload"
4. Click **"Commit changes"**

### 1.3 Enable GitHub Pages
1. Go to **Settings** (top menu)
2. Click **"Pages"** in left sidebar
3. **Source**: Select "Deploy from a branch"
4. **Branch**: Select "main" and "/ (root)"
5. Click **"Save"**
6. **Wait 5-10 minutes** for deployment

**🎉 Your site will be live at: `https://yourusername.github.io`**

---

## 📧 **Step 2: EmailJS Setup (Contact Form)**

### 2.1 Sign Up
1. Go to [emailjs.com](https://emailjs.com)
2. Click **"Sign Up"** and create account
3. **Verify your email**

### 2.2 Create Email Service
1. In dashboard, click **"Email Services"**
2. Click **"Add New Service"**
3. Choose **"Gmail"**
4. **Connect your Gmail** (`ajaythakare500@gmail.com`)
5. **Save the service**

### 2.3 Create Email Template
1. Click **"Email Templates"**
2. Click **"Create New Template"**
3. **Template name**: "Portfolio Contact"
4. **Subject**: `New Contact from Portfolio: {{subject}}`
5. **Content**:
```
Name: {{name}}
Email: {{email}}
Subject: {{subject}}
Message: {{message}}
```
6. **Save the template**

### 2.4 Get Your IDs
**Note down these IDs:**
- **User ID**: Go to Account → API Keys
- **Service ID**: From Email Services
- **Template ID**: From Email Templates

---

## 🔧 **Step 3: Update Contact Form**

### 3.1 Edit contact.html
1. Open `contact.html` in a text editor
2. **Find these lines** and replace with your actual IDs:

```javascript
// Replace 'YOUR_USER_ID' with your actual EmailJS User ID
emailjs.init("YOUR_USER_ID");

// Replace 'YOUR_SERVICE_ID' and 'YOUR_TEMPLATE_ID' with your actual IDs
emailjs.send('YOUR_SERVICE_ID', 'YOUR_TEMPLATE_ID', templateParams)
```

**Example:**
```javascript
emailjs.init("abc123def456");
emailjs.send('service_xyz', 'template_abc', templateParams)
```

### 3.2 Upload Updated File
1. Go back to your GitHub repository
2. **Edit** `contact.html`
3. **Paste the updated code**
4. **Commit changes**

---

## ✅ **Step 4: Test Everything**

### 4.1 Test Website
1. Visit `https://yourusername.github.io`
2. **Check all pages** load correctly
3. **Test navigation** between sections

### 4.2 Test Contact Form
1. Go to **Contact page**
2. **Fill out the form** with test data
3. **Submit** and check your email
4. **Verify** you received the message

---

## 🎯 **What Happens When Someone Contacts You**

1. **Visitor fills form** on your portfolio
2. **EmailJS sends email** to your Gmail
3. **You get notification** in your inbox
4. **You can reply** directly to their email
5. **All contact info** is preserved

---

## 🔄 **Updating Your Portfolio**

### To make changes:
1. **Edit files** on your computer
2. **Upload to GitHub** repository
3. **Changes auto-deploy** in 5-10 minutes
4. **No additional setup** needed

---

## 🆘 **Troubleshooting**

### Website not loading?
- Check repository name is exactly `yourusername.github.io`
- Wait 10-15 minutes after enabling Pages
- Check repository is Public

### Contact form not working?
- Verify EmailJS IDs are correct
- Check browser console for errors
- Ensure Gmail service is connected

### Need help?
- GitHub Pages: [docs.github.com/pages](https://docs.github.com/pages)
- EmailJS: [emailjs.com/docs](https://emailjs.com/docs)

---

## 🎉 **You're Done!**

**Your portfolio is now:**
- ✅ **Live on the internet**
- ✅ **Contact form working**
- ✅ **Professional appearance**
- ✅ **Easy to update**

**Share your portfolio URL on LinkedIn and start getting opportunities! 🚀**
