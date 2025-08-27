# Vumble - Dating App

A modern dating application built with React and Node.js, featuring swipe-based matching, real-time chat, and user authentication.

## 🚀 Features

- **User Authentication**: Secure signup/login with JWT tokens and bcrypt password hashing
- **Profile Creation**: Comprehensive onboarding with personal details, photos, and preferences
- **Swipe Interface**: Tinder-like card swiping for matching with other users
- **Smart Matching**: Gender-based matching algorithm with user preferences
- **Real-time Chat**: Instant messaging between matched users
- **Responsive Design**: Modern UI with smooth animations and intuitive navigation
- **Secure Backend**: RESTful API with MongoDB database and Express.js server

## 🛠️ Tech Stack

### Frontend
- **React.js** - User interface and state management
- **React Router** - Navigation and routing
- **React Tinder Card** - Swipe functionality
- **Axios** - HTTP client for API calls
- **React Cookies** - Cookie management for authentication

### Backend
- **Node.js** - Server runtime environment
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database
- **JWT** - JSON Web Token authentication
- **bcrypt** - Password hashing
- **CORS** - Cross-origin resource sharing
- **UUID** - Unique identifier generation

## 📁 Project Structure

```
Vumble/
├── public/                 # Static assets
├── src/                    # React source code
│   ├── components/         # Reusable UI components
│   │   ├── AuthModal.js   # Authentication modal
│   │   ├── Chat.js        # Chat functionality
│   │   ├── ChatContainer.js # Chat container
│   │   ├── ChatDisplay.js # Chat display
│   │   ├── ChatHeader.js  # Chat header
│   │   ├── ChatInput.js   # Chat input
│   │   ├── MatchesDisplay.js # Matches display
│   │   └── Nav.js         # Navigation component
│   ├── pages/             # Page components
│   │   ├── Dashboard.js   # Main dashboard with swipe
│   │   ├── Home.js        # Landing page
│   │   └── OnBoarding.js  # User profile setup
│   ├── images/            # Image assets
│   ├── App.js             # Main app component
│   └── index.js           # React entry point
├── index.js               # Express server
├── package.json           # Dependencies and scripts
└── README.md              # Project documentation
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- MongoDB database
- npm or yarn package manager

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/vumble.git
   cd vumble
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   Create a `.env` file in the root directory:
   ```env
   URI=your_mongodb_connection_string
   ```

4. **Start the backend server**
   ```bash
   npm run start:backend
   ```
   The server will run on `http://localhost:8000`

5. **Start the React frontend**
   In a new terminal:
   ```bash
   cd src
   npm start
   ```
   The app will open in your browser at `http://localhost:3000`

## 🔧 API Endpoints

### Authentication
- `POST /signup` - User registration
- `POST /login` - User authentication

### User Management
- `GET /user` - Get user profile
- `PUT /user` - Update user profile
- `GET /gendered-users` - Get users by gender preference
- `GET /users` - Get multiple users by IDs

### Matching & Chat
- `PUT /addmatch` - Add a new match
- `GET /messages` - Get chat messages
- `POST /message` - Send a new message

## 💡 Key Features Explained

### Swipe Interface
The app uses `react-tinder-card` to create an intuitive swipe experience:
- Swipe right to like and potentially match
- Swipe left to pass
- Automatic match detection and storage

### User Matching
- Users are matched based on gender preferences
- Matches are stored in the database
- Real-time updates when new matches occur

### Chat System
- Instant messaging between matched users
- Message persistence in MongoDB
- Real-time chat interface with user avatars

### Profile Management
- Comprehensive onboarding process
- Profile photo upload via URL
- Customizable gender preferences and visibility settings

## 🔒 Security Features

- **Password Hashing**: bcrypt with salt rounds
- **JWT Authentication**: Secure token-based authentication
- **Input Validation**: Server-side validation for all inputs
- **CORS Protection**: Configured for secure cross-origin requests

## 🎨 UI/UX Features

- **Responsive Design**: Works on desktop and mobile devices
- **Smooth Animations**: Card swipe animations and transitions
- **Modern Interface**: Clean, intuitive design inspired by popular dating apps
- **Accessibility**: Proper form labels and semantic HTML

## 🚧 Development

### Available Scripts
- `npm run start:backend` - Start the backend server with nodemon
- `npm test` - Run tests (currently placeholder)

### Code Style
- ES6+ JavaScript features
- React functional components with hooks
- Consistent component structure
- Clear separation of concerns

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the ISC License.

## 🙏 Acknowledgments

- Inspired by popular dating applications
- Built with modern web technologies
- Community-driven development approach

## 📞 Support

For support and questions, please open an issue in the GitHub repository.

---

**Note**: This is a demo project for educational purposes. Please ensure compliance with local laws and regulations when deploying dating applications.

