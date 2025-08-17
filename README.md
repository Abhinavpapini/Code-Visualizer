# AI Code Reviewer 🤖

An intelligent code review application powered by AI that analyzes your code, provides improvement suggestions, and converts code between multiple programming languages.

## ✨ Features

### 🔍 **AI-Powered Code Analysis**
- **Smart Code Review**: Get detailed feedback on your code quality, structure, and best practices
- **Line-by-Line Analysis**: Receive specific suggestions for each line of your code
- **Performance Optimization**: Get recommendations for improving time and space complexity

### 🌐 **Multi-Language Support**
- **Input Languages**: JavaScript, Python, Java, C++, C#, TypeScript, HTML, CSS
- **Code Conversion**: Automatically convert your improved code to Java, C, and C++
- **Syntax Highlighting**: Beautiful code display with proper syntax highlighting

### 🎨 **User Experience**
- **Interactive Code Editor**: Built-in code editor with syntax highlighting
- **File Upload**: Upload code files directly (.js, .py, .java, .cpp, .cs, .ts, .html, .css)
- **Dark/Light Theme**: Toggle between themes for comfortable coding
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Real-time Preview**: See your code analysis results instantly

### 📚 **Educational Features**
- **Complexity Analysis**: Detailed time and space complexity breakdown
- **Best Practices**: Learn industry-standard coding practices
- **Personalized Learning**: Get curated learning resources based on your code
- **Multi-format Output**: Results displayed in clean, formatted markdown

## 🛠️ Technology Stack

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **Groq SDK** - AI model integration (DeepSeek R1 Distill Qwen 32B)
- **CORS** - Cross-origin resource sharing
- **dotenv** - Environment variable management

### Frontend
- **React 19** - User interface library
- **Vite** - Build tool and development server
- **TailwindCSS** - Utility-first CSS framework
- **Axios** - HTTP client for API calls
- **PrismJS** - Syntax highlighting
- **React Markdown** - Markdown rendering with rehype plugins

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn package manager
- Groq API key

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd AI-Code-Reviewer-main
   ```

2. **Backend Setup**
   ```bash
   cd backend
   npm install
   ```

3. **Create environment file**
   ```bash
   # Create .env file in backend directory
   echo "GROQ_API_KEY=your_groq_api_key_here" > .env
   ```

4. **Frontend Setup**
   ```bash
   cd ../frontend
   npm install
   ```

### Running the Application

1. **Start the Backend Server**
   ```bash
   cd backend
   npm start
   # Server runs on http://localhost:3000
   ```

2. **Start the Frontend Development Server**
   ```bash
   cd frontend
   npm run dev
   # Frontend runs on http://localhost:5173
   ```

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the backend directory with:
```env
GROQ_API_KEY=your_groq_api_key_here
```

### API Endpoints
- `GET /` - Health check endpoint
- `POST /ai/get-review` - Code review endpoint
  - Body: `{ "code": "your_code_here", "language": "python" }`

## 📁 Project Structure

```
AI-Code-Reviewer-main/
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   │   └── ai.controllers.js
│   │   ├── routes/
│   │   │   └── ai.routes.js
│   │   ├── services/
│   │   │   └── ai.services.js
│   │   └── app.js
│   ├── server.js
│   ├── package.json
│   └── .env
├── frontend/
│   ├── src/
│   │   ├── assets/
│   │   ├── App.jsx
│   │   ├── App.css
│   │   ├── index.css
│   │   └── main.jsx
│   ├── public/
│   ├── index.html
│   ├── package.json
│   └── vite.config.js
├── .gitignore
└── README.md
```

## 🎯 How to Use

1. **Upload or Write Code**: Either upload a code file or write directly in the editor
2. **Select Language**: Choose the programming language from the dropdown
3. **Get Review**: Click "Review Code" to analyze your code
4. **View Results**: See detailed suggestions, improvements, and conversions

## 🤖 AI Model

This application uses the **DeepSeek R1 Distill Qwen 32B** model via Groq API, which provides:
- Advanced code understanding
- Multi-language support
- Performance optimization suggestions
- Educational recommendations

## 🔒 Security

- Environment variables for API keys
- Input validation and sanitization
- CORS configuration for secure cross-origin requests
- Secure markdown rendering with rehype-sanitize

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- [Groq](https://groq.com/) for providing the AI model API
- [PrismJS](https://prismjs.com/) for syntax highlighting
- [TailwindCSS](https://tailwindcss.com/) for the beautiful UI
- [React](https://react.dev/) and [Vite](https://vitejs.dev/) for the development experience

## 📞 Support

If you encounter any issues or have questions, please:
- Open an issue on GitHub
- Check existing issues for solutions
- Contact the development team

---

**Made with ❤️ for developers by developers**
