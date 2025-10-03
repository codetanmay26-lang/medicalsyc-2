# React

A modern React-based project utilizing the latest frontend technologies and tools for building responsive web applications.

## 🚀 Features

- **React 18** - React version with improved rendering and concurrent features
- **Vite** - Lightning-fast build tool and development server
- **Redux Toolkit** - State management with simplified Redux setup
- **TailwindCSS** - Utility-first CSS framework with extensive customization
- **React Router v6** - Declarative routing for React applications
- **Data Visualization** - Integrated D3.js and Recharts for powerful data visualization
- **Form Management** - React Hook Form for efficient form handling
- **Animation** - Framer Motion for smooth UI animations
- **Testing** - Jest and React Testing Library setup

## 📋 Prerequisites

- Node.js (v14.x or higher)
- npm or yarn

## 🛠️ Installation

1. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   and
   npm install jspdf tesseract.js react-pdftotext
   ```
   
2. Start the development server:
   ```bash
   npm start
   # or
   yarn start
   ```

## 🔒 Demo Data & Privacy Information

**Important: This is a frontend-only prototype for demonstration purposes.**

### Data Storage
- All demo data (prescriptions, lab reports, vitals, medications) is stored locally 
  in your browser's localStorage.
- Your data is **completely private** and never leaves your computer.
- Each user/device has **separate, isolated data** - your test data will not 
  appear for other users.

### Data Persistence
- Data **persists between browser sessions** (survives closing tabs/browser).
- Data remains until you **manually clear browser storage** or **logout**.

### Fresh Demo Experience
**For a clean demo:**
1. Open the website in **Incognito/Private Browsing mode** (recommended)
2. Or clear browser data: Settings → Privacy → Clear browsing data → Cached files
3. Login with test credentials below to start fresh

### Data Clearing
When you **logout**, only **authentication tokens** are cleared. To completely 
reset all demo data, use **Incognito mode** or manually clear browser storage.

## 📁 Project Structure

```
medicalsyc-2-main
├─ .env
├─ favicon.ico
├─ index.html
├─ jsconfig.json
├─ package.json
├─ postcss.config.js
├─ public
│  ├─ assets
│  │  └─ images
│  │     ├─ favicon.ico
│  │     ├─ logo.png
│  │     └─ no_image.png
│  ├─ favicon.ico
│  ├─ manifest.json
│  └─ robots.txt
├─ README.md
├─ src
│  ├─ App.jsx
│  ├─ components
│  │  ├─ AppIcon.jsx
│  │  ├─ AppImage.jsx
│  │  ├─ ErrorBoundary.jsx
│  │  ├─ ProtectedRoute.jsx
│  │  ├─ ScrollToTop.jsx
│  │  └─ ui
│  │     ├─ BreadcrumbNavigation.jsx
│  │     ├─ Button.jsx
│  │     ├─ Checkbox.jsx
│  │     ├─ EmergencyAlertBanner.jsx
│  │     ├─ Header.jsx
│  │     ├─ Input.jsx
│  │     ├─ Select.jsx
│  │     ├─ Toast.jsx
│  │     └─ UserContextIndicator.jsx
│  ├─ contexts
│  │  └─ AuthContext.jsx
│  ├─ index.jsx
│  ├─ pages
│  │  ├─ admin-analytics
│  │  │  ├─ components
│  │  │  │  ├─ AnalyticsChart.jsx
│  │  │  │  ├─ MetricsOverview.jsx
│  │  │  │  ├─ PredictiveAnalytics.jsx
│  │  │  │  ├─ SystemStatusPanel.jsx
│  │  │  │  └─ UserManagementPanel.jsx
│  │  │  └─ index.jsx
│  │  ├─ doctor-dashboard
│  │  │  ├─ components
│  │  │  │  ├─ AnalysisReportsPanel.jsx
│  │  │  │  ├─ EmergencyAlertsPanel.jsx
│  │  │  │  ├─ FilterControls.jsx
│  │  │  │  ├─ PatientListTable.jsx
│  │  │  │  ├─ PatientVitalsPanel.jsx
│  │  │  │  ├─ QuickActionsPanel.jsx
│  │  │  │  ├─ ReviewedReportsPage.jsx
│  │  │  │  └─ SummaryMetricsCards.jsx
│  │  │  └─ index.jsx
│  │  ├─ login
│  │  │  ├─ components
│  │  │  │  ├─ LoginForm.jsx
│  │  │  │  ├─ TestCredentials.jsx
│  │  │  │  └─ WelcomeHeader.jsx
│  │  │  └─ index.jsx
│  │  ├─ NotFound.jsx
│  │  ├─ patient-portal
│  │  │  ├─ components
│  │  │  │  ├─ AdherenceCalendar.jsx
│  │  │  │  ├─ EmergencyContactPanel.jsx
│  │  │  │  ├─ HealthLogger.jsx
│  │  │  │  ├─ LabReportUploader.jsx
│  │  │  │  ├─ MedicationTimeline.jsx
│  │  │  │  ├─ MedicineListViewer.jsx
│  │  │  │  ├─ MedicineReminder.jsx
│  │  │  │  ├─ MessagingInterface.jsx
│  │  │  │  ├─ NotificationCenter.jsx
│  │  │  │  └─ PrescriptionUploader.jsx
│  │  │  └─ index.jsx
│  │  ├─ patient-profile
│  │  │  ├─ components
│  │  │  │  ├─ AISuggestions.jsx
│  │  │  │  ├─ ChatMessaging.jsx
│  │  │  │  ├─ HealthLogsChart.jsx
│  │  │  │  ├─ LabReportsViewer.jsx
│  │  │  │  ├─ MedicationTimeline.jsx
│  │  │  │  └─ PatientHeader.jsx
│  │  │  └─ index.jsx
│  │  ├─ pharmacy-dashboard
│  │  │  ├─ components
│  │  │  │  ├─ AnalyticsCharts.jsx
│  │  │  │  ├─ EmergencyAlertsPanel.jsx
│  │  │  │  ├─ InventoryOverview.jsx
│  │  │  │  └─ RefillRequestsPanel.jsx
│  │  │  └─ index.jsx
│  │  └─ welcome
│  │     ├─ background.css
│  │     ├─ CombinedIllustration.jsx
│  │     ├─ CustomCursor.jsx
│  │     └─ index.jsx
│  ├─ Routes.jsx
│  ├─ styles
│  │  ├─ index.css
│  │  └─ tailwind.css
│  └─ utils
│     ├─ aiAnalysis.js
│     ├─ cn.js
│     └─ prescriptionAnalysis.js
├─ tailwind.config.js
├─ vercel.json
└─ vite.config.mjs
```



## 🎨 Styling

This project uses Tailwind CSS for styling. The configuration includes:

- Forms plugin for form styling
- Typography plugin for text styling
- Aspect ratio plugin for responsive elements
- Container queries for component-specific responsive design
- Fluid typography for responsive text
- Animation utilities

## 📱 Responsive Design

The app is built with responsive design using Tailwind CSS breakpoints.


## 📦 Deployment

Build the application for production:

```bash
npm run start
```

## 🙏 Acknowledgments
- Powered by React and Vite
- Styled with Tailwind CSS
