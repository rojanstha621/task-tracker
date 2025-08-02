# Task Manager Frontend

A modern, responsive React application for task management with authentication, dark mode support, and a beautiful UI.

## Features

### 🎨 Modern UI/UX
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Dark Mode Support**: Toggle between light and dark themes
- **Beautiful Components**: Modern, clean design with Tailwind CSS
- **Smooth Animations**: Loading states and transitions for better user experience

### 🔐 Authentication
- **User Registration**: Create new accounts with email and password
- **User Login**: Secure authentication with JWT tokens
- **Protected Routes**: Automatic redirection for unauthenticated users
- **Logout Functionality**: Secure logout with token removal

### 📋 Task Management
- **Create Tasks**: Add new tasks with title and optional description
- **View Tasks**: See all your tasks in a clean, organized layout
- **Complete Tasks**: Mark tasks as completed with visual feedback
- **Delete Tasks**: Remove tasks with confirmation dialog
- **Filter Tasks**: View all, pending, or completed tasks
- **Task Statistics**: Dashboard with task counts and progress

### 🧭 Navigation
- **Navbar**: Responsive navigation with authentication status
- **Footer**: Links and information about the application
- **Breadcrumbs**: Clear navigation between pages

## Tech Stack

- **React 19**: Latest version with hooks and modern features
- **React Router**: Client-side routing
- **Tailwind CSS**: Utility-first CSS framework
- **Axios**: HTTP client for API communication
- **JWT**: JSON Web Tokens for authentication

## Project Structure

```
src/
├── components/
│   ├── Navbar.js          # Navigation component with auth status
│   └── Footer.js          # Footer component with links
├── pages/
│   ├── Dashboard.js       # Main task management interface
│   ├── Login.js          # User authentication page
│   └── Register.js       # User registration page
├── services/
│   └── api.js            # API service with interceptors
├── App.js                # Main application component
└── index.js              # Application entry point
```

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Backend server running on `http://localhost:5000`

### Installation

1. **Install dependencies**:
   ```bash
   npm install
   ```

2. **Start the development server**:
   ```bash
   npm start
   ```

3. **Open your browser**:
   Navigate to `http://localhost:3000`

### Available Scripts

- `npm start` - Start development server
- `npm build` - Build for production
- `npm test` - Run tests
- `npm eject` - Eject from Create React App

## Features in Detail

### Authentication Flow
1. **Registration**: Users can create new accounts
2. **Login**: Secure authentication with email/password
3. **Token Management**: Automatic token handling and refresh
4. **Route Protection**: Unauthorized users are redirected to login

### Task Management
1. **Create**: Add new tasks with title and description
2. **Read**: View all tasks with filtering options
3. **Update**: Mark tasks as complete/incomplete
4. **Delete**: Remove tasks with confirmation

### UI Components
- **Navbar**: Responsive navigation with dark mode toggle
- **Footer**: Information and links
- **Forms**: Styled input fields with validation
- **Cards**: Task display with hover effects
- **Buttons**: Consistent styling with loading states

### Dark Mode
- **Toggle**: Easy switch between light and dark themes
- **Persistence**: Theme preference is maintained
- **Consistent**: All components support both themes

## API Integration

The frontend communicates with the backend through a centralized API service:

- **Base URL**: `http://localhost:5000/api`
- **Authentication**: JWT tokens in Authorization header
- **Error Handling**: Automatic 401 redirects
- **Interceptors**: Automatic token management

## Responsive Design

The application is fully responsive with:
- **Mobile-first**: Optimized for mobile devices
- **Tablet**: Adapted layouts for medium screens
- **Desktop**: Full-featured experience on large screens
- **Touch-friendly**: Optimized for touch interactions

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is licensed under the MIT License.
