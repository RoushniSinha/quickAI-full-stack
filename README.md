# QuickAI-Full-Stack

A comprehensive AI-powered content creation and image processing platform built with React and Node.js. QuickAI provides a unified interface for multiple AI services including text generation, image creation, and professional content tools.

## 🌐 Public URL

**https://quick-ai-main-taupe.vercel.app/**

## 🚀 Features

### Content Generation
- **AI Article Writing**: Generate professional articles using Google Gemini AI
- **Blog Title Creation**: Create SEO-optimized blog titles
- **Resume Review**: Professional resume analysis and improvement suggestions

### Image Processing
- **AI Image Generation**: Create images from text prompts using Clipdrop
- **Background Removal**: Automatically remove backgrounds from images
- **Object Removal**: Intelligent object removal and editing

### Platform Features
- **User Dashboard**: Real-time analytics and usage tracking
- **Subscription Management**: Freemium model with tiered access
- **Community Gallery**: Showcase and share user creations
- **Responsive Design**: Mobile-optimized interface

## 🏗️ Architecture

- **Frontend**: React 18 with Vite, Tailwind CSS, React Router
- **Backend**: Node.js with Express.js
- **Database**: Neon PostgreSQL
- **Authentication**: Clerk
- **AI Services**: Google Gemini, Clipdrop, Cloudinary
- **Deployment**: Vercel (client), Vercel (server)

## 📋 Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- PostgreSQL database (Neon recommended)
- API keys for:
  - Google Gemini
  - Clipdrop
  - Cloudinary
  - Clerk

## 🛠️ Installation

### Backend Setup

1. Navigate to the server directory:
   ```bash
   cd server
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file with the following variables:
   ```
   PORT=5000
   DATABASE_URL=your_neon_database_url
   CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
   CLERK_SECRET_KEY=your_clerk_secret_key
   GEMINI_API_KEY=your_gemini_api_key
   CLIPDROP_API_KEY=your_clipdrop_api_key
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   ```

4. Run database migrations:
   ```bash
   # Execute the SQL in database_schema.sql
   ```

5. Start the server:
   ```bash
   npm start
   ```

### Frontend Setup

1. Navigate to the client directory:
   ```bash
   cd client
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file with Clerk keys:
   ```
   VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

## 🚀 Usage

1. **Sign Up/Login**: Create an account using Clerk authentication
2. **Choose Plan**: Select between free or premium subscription
3. **Access Tools**: Navigate to specific AI tools via the dashboard
4. **Create Content**: Use prompts and parameters to generate content
5. **Manage Creations**: Save, download, and share your generated content

## 📁 Project Structure

```
QuickAI-Full-Stack/
├── client/                 # React frontend
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/          # Page components
│   │   └── assets/         # Static assets
│   ├── package.json
│   └── vite.config.js
├── server/                 # Node.js backend
│   ├── controllers/        # Route controllers
│   ├── routes/             # API routes
│   ├── middlewares/        # Express middlewares
│   ├── utils/              # Utility functions
│   ├── configs/            # Service configurations
│   └── package.json
├── diagrams/               # Architecture diagrams
├── TESTING_DOCUMENTATION.md
├── TODO.md
└── README.md
```

## 🧪 Testing

### Frontend Testing
```bash
cd client
npm test
```

### Backend Testing
```bash
cd server
npm test
```

### End-to-End Testing
```bash
cd client
npm run cypress:run
```

## 📚 API Documentation

The backend provides RESTful APIs for all AI services:

- `POST /api/ai/generate-article` - Generate articles
- `POST /api/ai/generate-titles` - Create blog titles
- `POST /api/ai/generate-image` - Create images
- `POST /api/ai/remove-background` - Remove image backgrounds
- `POST /api/ai/remove-object` - Remove objects from images
- `POST /api/ai/review-resume` - Analyze resumes

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Google Gemini for AI text generation
- Clipdrop for AI image generation
- Cloudinary for image processing
- Clerk for authentication
- Neon for database hosting


