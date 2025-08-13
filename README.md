# Lily - AI-Powered Interview Preparation Platform

A modern, AI-driven platform for practicing job interviews with real-time feedback and voice-based interactions.

## 🚀 Features

- **AI-Powered Interviews**: Generate personalized interview questions based on job role, experience level, and tech stack
- **Voice-Based Interactions**: Conduct interviews using Vapi AI voice agents
- **Real-Time Feedback**: Get instant AI-generated feedback on your performance
- **User Authentication**: Secure Firebase-based authentication system
- **Modern UI/UX**: Clean, responsive design built with Tailwind CSS
- **Session Management**: Persistent user sessions with secure cookies

## 🛠️ Tech Stack

- **Frontend**: Next.js 15, React 19, TypeScript
- **Styling**: Tailwind CSS, shadcn/ui components
- **Authentication**: Firebase Authentication
- **Database**: Firestore (Firebase)
- **AI Services**: 
  - Vapi AI (Voice interactions)
  - Google Generative AI (Question generation & feedback)
- **Deployment**: Vercel-ready

## 📋 Prerequisites

Before running this project, make sure you have:

- Node.js 18+ installed
- npm or yarn package manager
- Firebase project with Firestore enabled
- Vapi AI account
- Google AI Studio API key

## 🚀 Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/lily-ai-interview-platform.git
cd lily-ai-interview-platform
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Environment Setup

Create a `.env.local` file in the root directory with the following variables:

```env
# Vapi AI Configuration
NEXT_PUBLIC_VAPI_WEB_TOKEN=your_vapi_web_token
NEXT_PUBLIC_VAPI_WORKFLOW_ID=your_vapi_workflow_id

# Google AI Configuration
GOOGLE_GENERATIVE_AI_API_KEY=your_google_ai_api_key

# Base URL
NEXT_PUBLIC_BASE_URL=http://localhost:3000

# Firebase Client Configuration
NEXT_PUBLIC_FIREBASE_API_KEY=your_firebase_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id

# Firebase Admin Configuration
FIREBASE_PROJECT_ID=your_project_id
FIREBASE_CLIENT_EMAIL=your_service_account_email
FIREBASE_PRIVATE_KEY=your_private_key_with_escaped_newlines
```

### 4. Firebase Setup

1. **Create a Firebase Project**:
   - Go to [Firebase Console](https://console.firebase.google.com/)
   - Create a new project or use existing one

2. **Enable Services**:
   - **Authentication**: Enable Email/Password sign-in
   - **Firestore Database**: Create database in test mode
   - **Authorized Domains**: Add `localhost` and `127.0.0.1`

3. **Get Configuration**:
   - Go to Project Settings → General → Your apps
   - Create a Web app if not exists
   - Copy the configuration values

4. **Service Account**:
   - Go to Project Settings → Service accounts
   - Generate new private key
   - Download JSON and extract the values

### 5. Vapi AI Setup

1. **Create Vapi Account**:
   - Sign up at [Vapi AI](https://vapi.ai/)
   - Create a Voice Workflow
   - Generate a Web token

### 6. Google AI Setup

1. **Get API Key**:
   - Go to [Google AI Studio](https://aistudio.google.com/app/apikey)
   - Create an API key

### 7. Run the Application

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## 📁 Project Structure

```
lily-ai-interview-platform/
├── app/                    # Next.js app directory
│   ├── (auth)/            # Authentication pages
│   ├── (root)/            # Protected pages
│   ├── api/               # API routes
│   └── globals.css        # Global styles
├── components/            # React components
├── firebase/              # Firebase configuration
├── lib/                   # Utility functions and actions
├── public/                # Static assets
└── types/                 # TypeScript type definitions
```

## 🔧 Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

## 🚀 Deployment

### Vercel (Recommended)

1. Push your code to GitHub
2. Connect your repository to Vercel
3. Add environment variables in Vercel dashboard
4. Deploy

### Other Platforms

The project can be deployed to any platform that supports Next.js:
- Netlify
- Railway
- DigitalOcean App Platform

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request


## 👨‍💻 Developer

**Aayush Kotadia**
- Email: [aayushkotadia@gmail.com]


## 🙏 Acknowledgments

- Built with Next.js and modern web technologies
- Powered by Vapi AI for voice interactions
- Enhanced with Google Generative AI for intelligent feedback

---

**Note**: This project is a demonstration of modern web development practices and AI integration. Make sure to replace placeholder values with your actual API keys and configuration.



