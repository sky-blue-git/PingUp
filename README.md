# SayHey

SayHey is a modern, full-stack social media application designed to bring people together. Share your moments, connect with friends, and chat in real-time through a sleek and responsive interface.

## 🚀 Features

- **Secure Authentication**: Robust user sign-up and login functionality powered by **Clerk**.
- **Interactive Feed**: Create and view posts with support for rich media.
- **Stories**: Share ephemeral updates that disappear after 24 hours.
- **Real-time Messaging**: Instant chat functionality to stay in touch with your connections.
- **Network & Discover**: Follow users, manage connections, and discover new people.
- **Media Management**: Seamless image uploads and optimization using **ImageKit**.
- **Responsive Design**: Built with **Tailwind CSS** for a mobile-first, adaptive experience.

## 🛠️ Tech Stack

### Client

- **Framework**: React 19 (Vite)
- **Styling**: Tailwind CSS 4
- **State Management**: Redux Toolkit
- **Routing**: React Router DOM 7
- **Authentication**: Clerk React SDK
- **HTTP Client**: Axios
- **Icons**: Lucide React

### Server

- **Runtime**: Node.js
- **Framework**: Express.js 5
- **Database**: MongoDB (Mongoose)
- **Authentication**: Clerk Express SDK
- **Storage**: ImageKit (with Multer)
- **Background Jobs**: Inngest
- **Email**: Nodemailer

## 📦 Getting Started

Follow these steps to set up the project locally.

### Prerequisites

Ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v18+ recommended)
- [MongoDB](https://www.mongodb.com/) (Local or Atlas)

### Installation

1.  **Clone the repository**

    ```bash
    git clone https://github.com/your-username/SayHey.git
    cd SayHey
    ```

2.  **Install Dependencies**
    - **Client**:

      ```bash
      cd client
      npm install
      ```

    - **Server**:
      ```bash
      cd server
      npm install
      ```

3.  **Environment Configuration**

    Create a `.env` file in the `server` directory and add the following:

    ```env
    PORT=5000
    MONGODB_URI=your_mongodb_connection_string
    CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
    CLERK_SECRET_KEY=your_clerk_secret_key
    IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
    IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
    IMAGEKIT_URL_ENDPOINT=your_imagekit_url_endpoint
    INNGEST_EVENT_KEY=your_inngest_key
    INNGEST_SIGNING_KEY=your_inngest_signing_key
    ```

    Create a `.env` file in the `client` directory:

    ```env
    VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
    ```

4.  **Running the Application**
    - **Start the Backend**:

      ```bash
      cd server
      npm run server
      ```

      The server will start on port 5000 (or your defined PORT).

    - **Start the Frontend**:
      ```bash
      cd client
      npm run dev
      ```
      The client will run on `http://localhost:5173`.

## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

## 📄 License

This project is licensed under the [ISC License](LICENSE).
