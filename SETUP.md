# Setup Guide

## Quick Start

1. Install dependencies:
   ```bash
   npm install
   ```

2. Create a `.env` file in the root directory:
   ```env
   VITE_GOOGLE_SHEET_ID=your_spreadsheet_id_here
   VITE_GOOGLE_API_KEY=your_api_key_here
   ```

3. Run the development server:
   ```bash
   npm run dev
   ```

4. Open `http://localhost:3000` in your browser

## Google Sheets API Setup

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project
3. Enable the Google Sheets API
4. Create credentials (API Key)
5. Create a Google Sheet with these tabs:
   - `Workflows` (columns: Timestamp, Name, Type, Steps, Status)
   - `TemplateUsage` (columns: Timestamp, TemplateId)
   - `FormData` (columns: Timestamp, ...your form fields)

## Note

The app will work without Google Sheets API setup - it will use localStorage as a fallback. However, for full functionality, Google Sheets integration is recommended.

