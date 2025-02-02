BharatFD Backend
A robust Node.js backend for the Multilingual FAQ Management System. This service provides RESTful APIs for managing FAQs with support for multiple languages using the Google Translate API.

📁 Project Structure
bash
Copy
Edit
backend/
├── src/
│   ├── config/         # Configuration files
│   ├── controllers/    # Request handlers
│   ├── models/         # Database models
│   ├── routes/         # API routes
│   ├── services/       # Business logic
│   ├── tests/          # Test files
│   ├── app.ts          # Application entry point
│   ├── server.ts       # Server startup file
├── dist/               # Compiled TypeScript files (generated after build)
├── .env                # Environment variables
├── .env.example        # Example environment variables
├── .eslintrc           # ESLint configuration
├── tsconfig.json       # TypeScript configuration
├── package.json        # Project metadata and dependencies
└── nodemon.json        # Nodemon configuration
🚀 Features
✅ RESTful API endpoints for FAQ management (CRUD operations)
✅ MongoDB integration for data persistence
✅ Redis caching for improved performance
✅ Multilingual support using Google Translate API
✅ CORS enabled for frontend integration
✅ Comprehensive test suite using Mocha + Chai
✅ ESLint & Prettier for code quality

🛠️ Tech Stack
Component	Technology Used
Runtime	Node.js
Framework	Express.js
Database	MongoDB (Mongoose ODM)
Caching	Redis
Testing	Mocha, Chai, Sinon
Translation	Google Translate API
Code Quality	TypeScript, ESLint, Prettier
Other Tools	Nodemon, dotenv
📋 Prerequisites
Ensure you have the following installed before setting up the project:

Node.js (v18 or higher)
MongoDB (for database storage)
Redis (for caching)
npm (Node Package Manager)
🔧 Installation
1️⃣ Clone the Repository
bash
Copy
Edit
git clone https://github.com/tivarii/BackendAssignment
cd backend
2️⃣ Install Dependencies
bash
Copy
Edit
npm install
3️⃣ Setup Environment Variables
Create a .env file in the root directory and configure it:

makefile
Copy
Edit
REDIS_PASSWORD=
REDIS_USER=
REDIS_HOST=
REDIS_PORT=
MONGO_URI=
🚀 Running the Application
Development Mode
bash
Copy
Edit
npm run dev
Production Mode
bash
Copy
Edit
npm run build
npm start
🛠 Running Tests
bash
Copy
Edit
npm test
🎯 Linting & Formatting
bash
Copy
Edit
npm run lint        # Check for linting issues
npm run lint:fix    # Fix linting issues automatically
📚 API Documentation
FAQ Endpoints
Get All FAQs
http
Copy
Edit
GET /api/faqs
✅ Returns a list of all FAQs

http
Copy
Edit
GET /api/faqs?lang=hi
✅ Returns FAQs translated into Hindi

Create a New FAQ
http
Copy
Edit
POST /api/faqs
✅ Creates a new FAQ

Body:

json
Copy
Edit
{
  "question": "What is Node.js?",
  "answer": "Node.js is a JavaScript runtime environment"
}
🔒 Environment Variables
Variable Name	Description
REDIS_PASSWORD	Redis password (if applicable)
REDIS_USER	Redis username (if applicable)
REDIS_HOST	Redis server hostname
REDIS_PORT	Redis server port
MONGO_URI	MongoDB connection string