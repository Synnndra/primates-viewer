# Deployment Guide - Vercel (Secure Option)

Your API key is now secure! It will be hidden on the server side.

## Step 1: Install Vercel CLI

Open Command Prompt and run:
```bash
npm install -g vercel
```

## Step 2: Deploy to Vercel

Navigate to your project folder:
```bash
cd C:\Users\bobby\solana-nft-viewer
```

Deploy:
```bash
vercel
```

Follow the prompts:
- Login/sign up when prompted
- Press Enter for default settings
- When asked about framework, choose "Other"

## Step 3: Add Your API Key (IMPORTANT!)

After deployment, you need to add your API key as an environment variable:

### Option A: Using Vercel Dashboard (Easier)
1. Go to https://vercel.com/dashboard
2. Click on your project
3. Go to "Settings" → "Environment Variables"
4. Add a new variable:
   - **Name:** `HELIUS_API_KEY`
   - **Value:** `fae97e4f-e2de-46d7-828f-9e18aec8e579` (your API key)
   - Select all environments (Production, Preview, Development)
5. Click "Save"
6. **Redeploy** your project (go to Deployments tab → click the 3 dots on latest deployment → "Redeploy")

### Option B: Using CLI (Advanced)
```bash
vercel env add HELIUS_API_KEY
```
Then paste your API key when prompted.

## Step 4: Test Your Site

Visit your Vercel URL (shown after deployment) and test the app!

## Important Notes:

- Your API key is now **completely hidden** from users
- Only you can see it in Vercel's environment variables
- To update your API key later, just change it in Vercel settings
- Anyone can use your app without seeing your API key!

## Troubleshooting:

**If you see "API key not configured" error:**
- Make sure you added the environment variable in Vercel
- Make sure you **redeployed** after adding it
- Check the variable name is exactly `HELIUS_API_KEY` (case sensitive)

**Need help?**
- Vercel docs: https://vercel.com/docs
- Your current API key: `fae97e4f-e2de-46d7-828f-9e18aec8e579`
