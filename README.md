# 📚 Bookly

Bookly is a full-stack application for book lovers to discover, share, and manage their reading experiences. It consists of a backend (Node.js/Express/MongoDB) and a mobile frontend (React Native/Expo).

## Features

- User authentication (signup, login, JWT)
- Profile with avatar (DiceBear Adventurer)
- Book CRUD (create, read, update, delete)
- User profile management
- Cloudinary integration for image uploads
- Loader and UI feedback components
- Expo mobile app with tabbed navigation

## Tech Stack

- **Backend:** Node.js, Express, MongoDB, Mongoose
- **Frontend:** React Native, Expo
- **Other:** Cloudinary, DiceBear Adventurer

## Backend Setup

1. Navigate to the `backend` folder:
   ```sh
   cd backend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Create a `.env` file with your MongoDB URI and Cloudinary credentials:
   ```env
   MONGODB_URI=your_mongodb_uri
   CLOUDINARY_CLOUD_NAME=your_cloud_name
   CLOUDINARY_API_KEY=your_api_key
   CLOUDINARY_API_SECRET=your_api_secret
   JWT_SECRET=your_jwt_secret
   ```
4. Start the server:
   ```sh
   npm start
   ```

## Mobile App Setup

1. Navigate to the `mobile` folder:
   ```sh
   cd mobile
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the Expo app:
   ```sh
   npx expo start
   ```
4. Scan the QR code with Expo Go or run on an emulator.

## API Endpoints

- `POST /api/auth/signup` - Register a new user
- `POST /api/auth/login` - Login and get JWT
- `GET /api/books` - List all books
- `POST /api/books` - Add a new book
- `PUT /api/books/:id` - Update a book
- `DELETE /api/books/:id` - Delete a book
- `GET /api/users/:id` - Get user profile

## Folder Structure

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
mobile/
  app/
    (auth)/
    (tabs)/
    assets/
    components/
    constants/
    lib/
    store/
```

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.