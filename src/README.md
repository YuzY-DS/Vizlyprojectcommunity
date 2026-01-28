# Vizly Analytics Dashboard

A modern, clean, and responsive analytics dashboard built with React, TypeScript, Tailwind CSS v4, and CSS Modules. Focused on delivering an improved UX with minimalist design and AI-powered insights.

## 🎨 Design Philosophy

This dashboard features a **minimalist, UX-focused design** with:

- ✅ Clean, modern interface with soft shadows
- ✅ Rounded cards with subtle hover effects
- ✅ Light grey backgrounds with blue/purple accents
- ✅ CSS Modules architecture for scalable styling
- ✅ Comprehensive design system foundation
- ✅ Single-user experience (Community features removed)
- ✅ Space reserved for future Zia AI Assistant integration
- ✅ Responsive across all devices

## 📁 Project Structure

```
/
  /components          # Reusable UI components
    /auth             # Authentication components (Login, SignUp, ForgotPassword)
    /ui               # shadcn/ui component library
    /Button           # Custom button with CSS Modules
    /figma            # Figma integration utilities
  /constants          # Configuration and mock data
  /context            # React Context providers
  /hooks              # Custom React hooks
  /styles             # Global styles and CSS variables
  /types              # TypeScript type definitions
  /utils              # Helper functions
  App.tsx             # Main application component
```

## 🚀 Core Features

### 🔐 Authentication
- **Login** - Clean split-screen design
- **Sign Up** - User registration flow
- **Forgot Password** - Password recovery

### 🏠 Workspace Management
- **Workspace Home** - Grid view of all workspaces with filtering and search
- **Workspace Screen** - Detailed workspace view with collapsible sidebar navigation
- **Create/Edit** - Modal-based workspace management
- **Data Import** - Import data from CSV, Excel, JSON sources
- **Favorites & Organization** - Star and organize your workspaces

### 📊 Reports & Analytics
- **Report Builder** - Three-panel split layout:
  - Left: Chart type selection and configuration
  - Center: Live chart preview with customization
  - Right: Data settings and future AI assistant integration
- **Chart Types** - Line, Bar, Pie, Area, Scatter charts (Recharts)
- **Color Schemes** - Multiple gradient color palettes
- **Data Table View** - Sortable, filterable, paginated data tables

### 📈 Dashboard View (Latest Update)
- **Per-Chart Insights Layout** - Revolutionary 50/50 split design:
  - **Left 50%**: Chart visualization area
  - **Right 50%**: Dedicated insight panel with AI-powered analysis
- **Vertical Stacking** - One chart per row for focused analysis
- **Interactive Chat** - Chat box at the bottom of each insight area for conversational analytics
- **Multi-Widget Support** - Display multiple charts with their respective insights
- **Edit Mode** - Add, remove, and configure dashboard widgets
- **Export & Share** - Save and share dashboard configurations

### 👤 Profile & Settings
- **Profile Management** - Edit personal information
- **Account Settings** - Security and preferences
- **Notifications** - Notification panel with real-time updates
- **Theme Customization** - Ready for light/dark mode

### 📤 Collaboration & Sharing
- **Share/Export Modal** - Collaborative features:
  - Share via email or link
  - Set permissions (view/edit)
  - Export to PDF, PNG, or Excel
  - Schedule automated reports

## 🎯 Design System

### CSS Modules Architecture
- **Modular Styling** - Component-scoped CSS for better encapsulation
- **Design Tokens** - Centralized variables in `/styles/variables.css`
- **Global Styles** - Base styles and resets in `/styles/globals.css`
- **Tailwind v4** - Utility-first CSS framework integration

### Color Palette
- **Primary**: Blue (`#3B82F6`) to Purple (`#8B5CF6`) gradients
- **Backgrounds**: Light grey (`#F9FAFB`, `#F3F4F6`)
- **Cards**: White (`#FFFFFF`) with soft shadows
- **Accents**: Blue, Purple, Green, Orange, Red, Pink, Teal, Indigo
- **Text**: Dark slate for readability

### Visual Style
- **Borders**: Rounded corners (8px - 16px)
- **Shadows**: Soft, layered shadows for depth
- **Hover Effects**: Smooth transitions and scale transforms
- **Spacing**: Consistent padding and margins (16px - 24px)
- **Typography**: Clean sans-serif hierarchy

## 📦 Tech Stack

### Core Technologies
- **React 18** - Modern UI framework with hooks
- **TypeScript** - Type-safe development
- **Tailwind CSS v4** - Utility-first styling

### UI & Visualization
- **Recharts** - Interactive data visualizations
- **Lucide React** - Icon library
- **shadcn/ui** - High-quality component library
- **CSS Modules** - Scoped component styling

### State Management
- **React Context** - Global state (AppContext)
- **Custom Hooks** - Business logic encapsulation
  - `useWorkspace` - Workspace operations
  - `useNotifications` - Notification management

### Data & Utilities
- **Mock Data** - Comprehensive sample datasets
- **TypeScript Types** - Full type definitions for all entities

## 🛠️ Getting Started

### Prerequisites
- Node.js 18+
- npm or yarn

### Installation

```bash
# Install dependencies
npm install

# Run development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## 📱 Screens & User Flows

### 1. Authentication Flow
- Login with email/password
- Sign up with validation
- Password reset functionality
- Form validation and error handling

### 2. Workspace Home
- Grid layout with workspace cards
- Search and filter capabilities
- Quick actions (Create, Import, Star)
- Empty states and loading indicators

### 3. Workspace Detail
- Collapsible sidebar with navigation
- Overview dashboard
- Reports listing
- Data sources management
- Settings panel

### 4. Report Builder
- **Three-Panel Layout**:
  - Configuration panel (chart type, data)
  - Live preview with customization
  - Data settings and AI assistant placeholder
- Real-time chart updates
- Color scheme selection
- Save and export options

### 5. Dashboard View (New Layout)
- **50/50 Split Per Chart**:
  - Chart visualization (left 50%)
  - Insight panel (right 50%)
- Vertical stacking (one chart per row)
- Chat interface at bottom of each insight
- Add/remove widgets in edit mode
- Full-screen mode for focused analysis

### 6. Data Management
- Import data modal (CSV, Excel, JSON)
- Data processing with preview
- Data transformation pipeline
- Table view with sorting and filtering

### 7. Profile & Settings
- Profile information editor
- Notification preferences
- Account security settings

## 🎨 Sample Data

The application includes comprehensive mock data:
- **6 Workspaces** - With varied statistics and metadata
- **5 Reports** - Different chart types and configurations
- **2 Dashboards** - Pre-configured widget layouts
- **Revenue Data** - 12 months of sample financial data
- **User Data** - Sample profiles and activity
- **Notifications** - Various notification types

## 📚 Architecture Highlights

### Component-Based Design
- **Reusable Components** - Shared UI components in `/components`
- **Feature Isolation** - Self-contained feature modules
- **Type Safety** - Full TypeScript coverage
- **CSS Modules** - Scoped styling per component

### State Management Strategy
```
User Action → Component → Hook → Context → Update → Re-render
```

### Styling Architecture
```
Global Variables (variables.css)
        ↓
Base Styles (globals.css)
        ↓
Tailwind Utilities
        ↓
CSS Modules (Component-specific)
```

## 🎯 Best Practices

### Code Organization
- **Components**: One component per file, PascalCase naming
- **Hooks**: Custom hooks prefixed with `use`, in `/hooks` directory
- **Types**: Centralized in `/types/index.ts`
- **Constants**: Configuration in `/constants/config.ts`

### Styling Guidelines
- **Tailwind First**: Use utility classes for layout and spacing
- **CSS Modules**: For component-specific styles
- **No Inline Styles**: Maintain consistency with design system
- **Responsive**: Mobile-first approach with breakpoints

### TypeScript Conventions
- **Explicit Types**: Define interfaces for all props and data
- **Avoid `any`**: Use proper typing throughout
- **Type Guards**: Validate data shapes when needed

## 🔮 Future Enhancements

### Zia AI Assistant Integration
- **Conversational Analytics** - Chat with your data
- **Smart Insights** - AI-generated observations per chart
- **Recommendations** - Suggested visualizations and analyses
- **Natural Language Queries** - Ask questions in plain English

### Backend Integration Roadmap
1. **API Layer**
   - RESTful API integration
   - Authentication with JWT
   - Real-time updates via WebSockets

2. **Data Persistence**
   - User accounts and workspaces
   - Report configurations
   - Uploaded datasets
   - Collaborative features

3. **Advanced Features**
   - Real-time collaboration
   - Automated insights
   - Scheduled reports
   - Advanced data transformations

4. **Performance**
   - Lazy loading for large datasets
   - Caching strategies
   - Optimistic UI updates

## 🧹 Recent Changes

### Architecture Refactor
- ✅ Migrated to CSS Modules architecture
- ✅ Established comprehensive design system
- ✅ Removed community and public features for single-user focus
- ✅ Fixed Login component import paths

### Dashboard Redesign
- ✅ Replaced AI chat sidebar with per-chart insights
- ✅ Implemented 50/50 split layout (Chart + Insights)
- ✅ Added vertical stacking (one chart per row)
- ✅ Added chat box at bottom of each insight area
- ✅ Improved focus on individual chart analysis

## 📄 License

This project is proprietary and confidential.

## 👥 Contributors

Built with ❤️ for modern analytics and AI-powered insights

---

## ✨ Key Highlights

- ✅ Clean, minimalist design with UX focus
- ✅ CSS Modules architecture for scalability
- ✅ Comprehensive design system
- ✅ Single-user focused experience
- ✅ Per-chart insights with chat interface
- ✅ Responsive across all devices
- ✅ TypeScript type safety
- ✅ Production-ready code structure
- ✅ Ready for Zia AI Assistant integration
- ✅ Modular, maintainable codebase

---

**Ready to build intelligent analytics dashboards!** 🚀

Start at the Login screen to experience the complete Vizly dashboard.
