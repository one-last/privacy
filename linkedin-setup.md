# LinkedIn Developer Account Setup Guide

## Individual Developer Setup (Recommended for Starting)

1. **Go to LinkedIn Developers Portal**
   - Visit https://www.linkedin.com/developers/
   - Click "Create app"

2. **App Creation**
   - For "App Name" enter: "OneClicke"
   - For "LinkedIn Page": Select the default company page provided by LinkedIn
   - DO NOT try to create or link your own company page

3. **App Settings**
   - Products: Select "Sign In with LinkedIn"
   - App Logo: Upload your OneClicke logo
   - Application URL: Your application's URL
   - Authorized Redirect URLs: 
     ```
     http://localhost:3000/auth/linkedin/callback (for development)
     https://your-domain.com/auth/linkedin/callback (for production)
     ```

4. **Verify and Get Credentials**
   - Once approved, you'll receive:
     - Client ID
     - Client Secret
   - Save these in your `.env` file

## Important Notes

- You don't need to create a LinkedIn Company Page
- Use the default company page LinkedIn provides
- This is sufficient for basic OAuth and API access
- You can upgrade to business account later if needed

## Features Available with Individual Account

- Sign In with LinkedIn
- Basic Profile API
- Share on LinkedIn
- Social Interactions

## Next Steps

1. Copy your Client ID and Client Secret
2. Add them to your `.env` file:
   ```
   LINKEDIN_CLIENT_ID=your_client_id
   LINKEDIN_CLIENT_SECRET=your_client_secret
   ```
3. Test the integration using localhost
4. Deploy to production when ready 