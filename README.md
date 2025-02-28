# Real-Time Chat Application

This is a real-time chat application built using **Java, Spring Boot, MongoDB, and React.js**. The project leverages **STOMP-based WebSockets** to enable bidirectional messaging between users in dynamically created chat rooms.

## Features

- **Real-time messaging** using WebSockets (STOMP protocol)
- **Chat room functionality** with unique Room IDs
- **Pagination for chat history**, optimizing message retrieval
- **MongoDB integration** for persistent message storage
- **Spring Boot backend** with REST API support
- **React.js frontend** for an interactive user experience

## Tech Stack

- **Backend:** Java, Spring Boot, WebSockets, STOMP, MongoDB, Maven
- **Frontend:** React.js
- **Database:** MongoDB

## Project Structure

```
chat-application/
│── backend/
│   ├── src/main/java/com/example/chat/
│   │   ├── config/   # WebSocket and MongoDB configurations
│   │   ├── controller/   # REST controllers
│   │   ├── model/   # Data models (User, ChatRoom, Message)
│   │   ├── repository/   # MongoDB repositories
│   │   ├── service/   # Business logic layer
│── frontend/
│   ├── src/
│   │   ├── components/   # React components
│   │   ├── services/   # API calls
│   │   ├── App.js
│── README.md
```

## Setup Instructions

### Backend (Spring Boot)
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/chat-application.git
   cd chat-application/backend
   ```
2. Configure MongoDB in `application.properties`:
   ```properties
   spring.data.mongodb.uri=mongodb://localhost:27017/chatdb
   ```
3. Build and run the backend:
   ```sh
   mvn spring-boot:run
   ```

### Frontend (React.js)
1. Navigate to the frontend directory:
   ```sh
   cd ../frontend
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the frontend:
   ```sh
   npm start
   ```

## Usage
- Open the application in a browser.
- Join a chat room using a unique Room ID.
- Send messages in real-time and retrieve chat history with pagination.

## Future Improvements
- User authentication and profiles.
- Typing indicators and read receipts.
- Push notifications for new messages.

## Contributing
Contributions are welcome! Feel free to fork the repository and submit pull requests.

## License
This project is open-source and available under the **MIT License**.

---

Happy coding! 🚀

