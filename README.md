# Campus Notifications Dashboard

A clean, minimal React + Vite application for displaying campus notifications with real-time filtering.

## Features

✨ **Simple & Fast** - Built with React + Vite for instant HMR  
🎯 **Filter by Type** - Event, Result, and Placement notifications  
🎨 **Beautiful UI** - Gradient background with responsive design  
📱 **Mobile Ready** - Works on all screen sizes  

## Project Structure

This project uses exactly **3 program files** for maximum simplicity:

```
src/
├── main.jsx                    # React entry point
├── App.jsx                     # Main component with UI
└── notificationService.js      # API calls & data logic
```

## Getting Started

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Open browser to http://localhost:5173
```

## How It Works

- **main.jsx** - Mounts the React app to the DOM
- **App.jsx** - Displays notifications with filter buttons and responsive layout  
- **notificationService.js** - Fetches notifications and handles filtering logic

## API Integration

To connect to the real API, edit `notificationService.js`:

```javascript
// Replace the mock data fetch with:
const response = await fetch('http://20.207.122.201/evaluation-service/notifications', {
  headers: { 'Authorization': 'Bearer YOUR_TOKEN' }
});
return await response.json();
```

## Notification Types

- **Event** (Blue) - Campus events like induction, tech fest
- **Result** (Green) - Exam results and placements  
- **Placement** (Pink) - Company hiring announcements

## Build for Production

```bash
npm run build
```

Output will be in the `dist/` folder.
