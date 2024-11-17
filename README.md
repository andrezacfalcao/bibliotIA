# **librarIA**

This is a project for managing a digital library application, developed with a **Django backend** and a **React frontend (TypeScript)**. The application provides functionalities like online book reading and personalized recommendation systems.

---

## **Technologies Used**

### **Backend**
- **Django**: Python-based web framework.
- **Django REST Framework**: For creating RESTful APIs.
- **PostgreSQL**: Database (or SQLite for local development).
- **Django-CORS-Headers**: To handle cross-origin resource sharing (CORS).

### **Frontend**
- **React**: JavaScript library for building user interfaces.
- **TypeScript**: Adds static typing to JavaScript.
- **Axios**: For HTTP requests.
- **React Router DOM**: For managing routes in the frontend.

---

## **Features**
- **Online Book Reading**: Provides an interface for reading books without downloading them.
- **Recommendation System**: Suggests books based on user history and favorite categories.
- **User Management**: Sign-up, login, and profile management.
- **Modern Styling**: Support for CSS frameworks like TailwindCSS or Material-UI.

---

## **How to Run the Project**

### **Prerequisites**
- Python 3.8+
- Node.js 16+
- PostgreSQL (or SQLite for local testing)
- npm or yarn package manager

---

# Step 2: Backend Setup (Django)
# ----------------------------------

# Create a virtual environment
python -m venv venv

# Activate the virtual environment
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install backend dependencies
pip install -r requirements.txt

# Run migrations
python manage.py makemigrations
python manage.py migrate

# Start the backend server
python manage.py runserver


# Step 3: Frontend Setup (React with TypeScript)
# ----------------------------------

# Navigate to the frontend directory
mkdir frontend
cd frontend

# Initialize a React project with TypeScript
npx create-react-app . --template typescript

# Install Axios for HTTP requests
npm install axios

# Install React Router DOM for navigation
npm install react-router-dom

# Install type definitions for the dependencies
npm install --save-dev @types/react-router-dom @types/axios

# Optional: Install Tailwind CSS for styling
npm install -D tailwindcss postcss autoprefixer

# Initialize Tailwind CSS
npx tailwindcss init

# Start the frontend development server
npm start
