# UberXpress-Backend

UberXpress-Backend is a robust backend service designed to power ride-hailing and delivery applications. Built with scalability, security, and performance in mind, this project provides RESTful APIs for user management, ride booking, payment processing, and real-time updates.

## Features

- **User Authentication**  
  Register and login functionality for both drivers and passengers.

- **Ride Booking**  
  Passengers can request rides by entering source and destination locations.

- **Driver Assignment**  
  Nearby drivers are notified in real-time. The first driver to accept is assigned the ride.

- **Location Tracking**  
  Drivers continuously update their live location. Redis GEO queries are used to find nearby drivers.

- **Booking Management**  
  Both drivers and passengers can view their current and past bookings.

- **Feedback System**  
  Passengers can rate and review drivers after a completed ride.

- **Real-Time Notifications**  
  Implemented using Socket.IO for instant booking alerts and confirmations.


## Getting Started

### Prerequisites

- Node.js (v16+)
- MongoDB
- Redis

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/adarshRai7/UberXpress-Backend.git
    cd UberXpress-Backend
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

3. Configure environment variables in `example.env`:
    ```
    MONGO_URI=your_mongo_connection_string
    PORT=your_desired_port
    JWT_SECRET=your_jwt_secret
    REDIS_URI=your_redis_connection_string
    ```

4. Start the server:
    ```bash
    npm start
    ```

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements and bug fixes.
