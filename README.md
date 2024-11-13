

# Hotel Booking Application

## Overview
This project is a hotel booking application developed using the MERN stack (MongoDB, Express, React, and Node.js). The application allows users to search for hotels, view details, and book rooms. It includes a responsive user interface and integrates a backend API for managing bookings, user data, and hotel information.

## Features
### User Interface
- **Homepage**: Displays popular hotels and destinations.
- **Hotel Search**: Users can search hotels by location, check-in/check-out dates, and guest count.
- **Hotel Details Page**: Provides information about each hotel, including room types, amenities, and availability.
- **User Dashboard**: Users can view and manage their bookings.

### Booking Management
- **Room Booking**: Users can book available rooms by selecting check-in/check-out dates and confirming guest information.
- **Booking History**: Registered users can view their past bookings.

### User Authentication
- **Sign Up/Login**: Secure authentication system with JWT for session management.
- **Profile Management**: Users can update personal information and view booking history.

### Admin Features
- **Hotel Management**: Admins can add, edit, or remove hotels and rooms.
- **Booking Management**: Admins can view all bookings, including user details and booking dates.

## Technology Stack
- **Frontend**: React, Redux, Bootstrap
- **Backend**: Node.js, Express
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Token)

## Assumptions and Design Choices
- **Booking Flow**: Only authenticated users can make bookings. Guest users can browse hotels but need to register to complete a booking.
- **Data Storage**: MongoDB is used to store user information, hotel details, and booking data.
- **Payment System**: No payment system is integrated in this version; future updates may include Stripe or PayPal.
- **Admin Role**: Admins have exclusive rights to manage hotels and view all bookings, whereas users can only manage their own bookings.

## Setup Instructions

### Prerequisites
- **Node.js**: Version 14+
- **MongoDB**: Running locally or MongoDB Atlas account
- **NPM** or **Yarn**

### Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/yourusername/hotel-booking-app.git
    cd hotel-booking-app
    ```

2. **Install Backend Dependencies**:
    ```bash
    cd server
    npm install
    ```

3. **Install Frontend Dependencies**:
    ```bash
    cd ../client
    npm install
    ```

4. **Environment Variables**:
   - In the `/server` directory, create a `.env` file and add the following:
     ```env
   MONGO = mongodb+srv://dev:dev@cluster0.capsjox.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0
   JWT = 8hEnPGeoBqGUT6zksxt4G95gW+uMdzwe7EVaRnp0xRI=
     PORT=5000
     ```
   - In the `/client` directory, create a `.env` file and add any frontend environment variables if required.

### Running the Application

1. **Start the Backend Server**:
    ```bash
    cd server
    npm start
    ```

2. **Start the Frontend Server**:
    ```bash
    cd ../client
    npm start
    ```

3. **Access the Application**:
   - Frontend: `http://localhost:3000`
   - Backend API: `http://localhost:5000`

### Running Tests
- **Backend Tests**: Use a testing framework like Mocha or Jest (if set up).
    ```bash
    cd server
    npm test
    ```
- **Frontend Tests**: Run tests with React Testing Library or Jest.
    ```bash
    cd client
    npm test
    ```

## Future Enhancements
- **Payment Integration**: Add Stripe or PayPal for handling secure payments.
- **Notifications**: Send booking confirmations via email.
- **Rating and Review System**: Allow users to rate and review hotels after their stay.
- **Advanced Search**: Include filters for amenities, price range, and hotel ratings.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.



