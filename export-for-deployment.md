# Export Your Project for Vercel

## Quick Export Steps

### 1. Download Your Project
Click the 3-dot menu in Replit → Download as ZIP

### 2. Extract and Clean
- Extract the ZIP file
- Remove `.replit` folder (not needed for Vercel)

### 3. Key Files for Vercel
Make sure these files are included:
- `vercel.json` ✅ (Vercel configuration)
- `api/chat.js` ✅ (Chatbot serverless function)
- `package.json` ✅ (Dependencies)
- All `client/` folder contents ✅
- All `server/` folder contents ✅
- All `shared/` folder contents ✅

### 4. Upload to GitHub
1. Create new repository on GitHub
2. Upload all files
3. Make repository public (for free deployment)

### 5. Connect to Vercel
- Go to vercel.com
- Sign in with GitHub
- Import your repository
- Deploy automatically

## Your Site Will Be Live At:
`https://yourprojectname.vercel.app`

## Chatbot Will Work!
The Wadadli Bot is configured as a serverless function and will respond to questions about Antigua & Barbuda with authentic local knowledge.