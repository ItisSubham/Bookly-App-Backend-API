<p align="center">
  <img src="./Bookly.png" alt="Bookly Logo" width="80" />
</p>

# 📚 Bookly Backend

Bookly is a full-stack platform for book lovers to discover, share, and manage their reading experiences. This repository contains the backend API built with Node.js, Express, and MongoDB. The mobile frontend is built with React Native and Expo.

## 🚀 Features

- 🔐 User authentication (signup, login, JWT)
- 👤 Profile with avatar (DiceBear Adventurer)
- 📚 Book CRUD (create, read, update, delete)
- 📝 User profile management
- 🖼️ Cloudinary integration for image uploads
- ⚡ Loader and UI feedback components
- 📱 Expo mobile app with tabbed navigation

## 🛠️ Tech Stack

- **Backend:** Node.js, Express, MongoDB, Mongoose
- **Frontend:** React Native, Expo
- **Other:** Cloudinary, DiceBear Adventurer

## ⚙️ Backend Setup

1. **Clone the repository**
   ```sh
   git clone https://github.com/ItisSubham/Bookly-App-Backend-API.git
   cd Bookly-App-Backend-API
   ```
2. **Install dependencies**
   ```sh
   npm install
   ```
3. **Start the server**
   ```sh
   npm start
   ```


## 📚 API Endpoints

- `POST /api/auth/signup` — Register a new user
- `POST /api/auth/login` — Login and get JWT
- `GET /api/books` — List all books
- `POST /api/books` — Add a new book
- `PUT /api/books/:id` — Update a book
- `DELETE /api/books/:id` — Delete a book
- `GET /api/users/:id` — Get user profile

## 📁 Folder Structure

```
backend/
  src/
    index.js
    lib/
      cloudinary.js
      cron.js
      db.js
    middleware/
      auth.middleware.js
    models/
      Book.js
      User.js
    routes/
      authRoutes.js
      bookRoutes.js
```

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.
