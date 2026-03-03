# 🏡 Wanderlust  
### A Full-Stack Airbnb Clone  

Wanderlust is a full-stack web application inspired by Airbnb that allows users to explore, create, review, and manage rental property listings.  
It is built using Node.js, Express, MongoDB, and EJS following the MVC architecture pattern.

---

## 🚀 Live Demo

> Deployed on Render  
(Add your live URL here)

---

## 🛠️ Tech Stack

### 🔹 Backend
- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- Joi (Server-side Validation)

### 🔹 Frontend
- EJS (Embedded JavaScript Templates)
- ejs-mate (Layout Support)
- Bootstrap 5.3.3
- Custom CSS
- Font Awesome 6.7.2

### 🔹 Authentication & Session
- express-session
- connect-mongo
- passport
- passport-local-mongoose

### 🔹 Cloud Storage
- Cloudinary
- multer
- multer-storage-cloudinary

---

## 📂 Project Structure

```
Wanderlust/
│
├── models/          # Mongoose Schemas (Listing, Review, User)
├── routes/          # Express Route Files
├── controllers/     # Business Logic (MVC)
├── views/           # EJS Templates
│   ├── listings/
│   ├── users/
│   ├── layouts/
│   └── includes/
├── public/          # Static Assets (CSS, JS, Images)
├── utils/           # Custom Error Handling & Async Wrapper
├── init/            # Database Seeding Scripts
├── cloudconfig.js   # Cloudinary Configuration
├── app.js           # Main Application Entry
└── package.json
```

---

## ✨ Features

### 🏠 Listings
- Create new rental listings
- View all listings
- View individual listing details
- Edit listing (Owner only)
- Delete listing (Owner only)
- Upload listing images (Cloudinary)

### ⭐ Reviews
- Add reviews to listings
- Delete reviews (Author only)
- Star rating system

### 🔐 Authentication & Authorization
- User Signup
- User Login / Logout
- Session-based authentication
- Only logged-in users can:
  - Create listings
  - Post reviews
- Only owners can:
  - Edit/Delete their listings
  - Delete their reviews

### 🛡️ Security & Validation
- Server-side validation using Joi
- Flash messages for feedback
- Environment variables for sensitive data
- Secure session storage in MongoDB

---

## 🌍 Environment Variables

Create a `.env` file in the root directory and add:

```
ATLASDB_URL=your_mongodb_atlas_connection_string
SECRET=your_session_secret
CLOUD_NAME=your_cloudinary_cloud_name
CLOUD_API_KEY=your_cloudinary_api_key
CLOUD_API_SECRET=your_cloudinary_api_secret
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```
git clone https://github.com/yourusername/wanderlust.git
cd wanderlust
```

### 2️⃣ Install Dependencies

```
npm install
```

### 3️⃣ Run the Application

```
node app.js
```

Or (recommended for development):

```
nodemon app.js
```

---

## ☁️ Deployment (Render)

- **Build Command:**  
  ```
  npm install
  ```

- **Start Command:**  
  ```
  node app.js
  ```

- Add all environment variables in Render Dashboard.

---

## 📸 Image Upload System

Images are uploaded using `multer` and stored securely on **Cloudinary**.  
Only the image URL and filename are saved in MongoDB.

---

## 🧱 Architecture

The project follows the **MVC (Model-View-Controller)** pattern:

- **Model** → Database Schema (Mongoose)
- **View** → EJS Templates
- **Controller** → Route Logic
- **Router** → API Endpoints

This ensures:
- Clean structure
- Scalability
- Maintainability

---

## 🎯 Future Improvements

- Booking system
- Payment integration
- Search & filter functionality
- Pagination
- Wishlist feature
- Map integration
- Admin dashboard

---

## 👩‍💻 Author

**Himanshi Godara**  
Full-Stack Developer | BE CSE Student  

---

## 📜 License

This project is for educational and portfolio purposes.
