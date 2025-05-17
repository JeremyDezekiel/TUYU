# Tuyu | Package Tracking Service

A simple and efficient web application to track package deliveries and truck drivers in real time. Built with React, Firebase, and Mapbox, Tuyu provides live location tracking, route history, and seamless management for both admins and drivers.

[Mockup Design on Figma](https://www.figma.com/design/FEyvL4hQSmC2e8xwcpyCNQ/Final-Project?node-id=0-1&t=ZihNP2zfJPvn75Tz-1)

---

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## Features

- **Live Location Tracking:** Real-time tracking of delivery vehicles on an interactive map.
- **Route History:** View historical routes and delivery statuses.
- **Admin Panel:** Manage deliveries, assign drivers, and monitor progress.
- **Driver Dashboard:** Accept and complete delivery tasks, update statuses.
- **Authentication:** Secure login and registration for admins and drivers.
- **Mapbox Integration:** Interactive maps with geocoding and directions.
- **Firebase Backend:** Real-time database and authentication.

---

## Tech Stack

- **Frontend:** React, Vite, Tailwind CSS
- **Backend:** Firebase (Firestore, Auth)
- **Maps:** Mapbox GL JS, Mapbox Directions API
- **Other:** SweetAlert2, ESLint

---

## Project Structure

```
client/
  ├── public/
  ├── src/
  │   ├── assets/
  │   ├── components/
  │   ├── config/
  │   ├── context/
  │   ├── layouts/
  │   ├── pages/
  │   ├── utils/
  │   ├── App.jsx
  │   ├── main.jsx
  │   └── router.jsx
  ├── index.html
  ├── package.json
  └── vite.config.js
server/
  ├── data.json
  ├── db.json
  └── package.json
```

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v16+ recommended)
- [Firebase Project](https://firebase.google.com/)
- [Mapbox Account](https://www.mapbox.com/)

### Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/jeremydezekiel/tuyu-package-tracking.git
   cd tuyu-package-tracking/client
   ```

2. **Install dependencies:**
   ```sh
   npm install
   ```

3. **Setup environment variables:**

   - Copy `.env.template` to `.env` in the `client/` directory.
   - Fill in your Firebase and Mapbox credentials.

   ```
   VITE_API_KEY=your_firebase_api_key
   VITE_AUTH_DOMAIN=your_firebase_auth_domain
   VITE_PROJECT_ID=your_firebase_project_id
   VITE_STORAGE_BUCKET=your_firebase_storage_bucket
   VITE_MESSAGING_SENDER_ID=your_firebase_messaging_sender_id
   VITE_APP_ID=your_firebase_app_id
   VITE_API_KEY_MapBox=your_mapbox_access_token
   ```

4. **Run the development server:**
   ```sh
   npm run dev
   ```

5. **(Optional) Start the mock server:**
   ```sh
   cd ../server
   npm install
   npm start
   ```

---

## Usage

- **Admin:**  
  - Register/login as admin.
  - Add new deliveries, assign drivers, and monitor all routes.
- **Driver:**  
  - Register/login as driver.
  - View assigned deliveries, start and complete delivery, update live location.

---

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements and bug fixes.

---

## License

This project is licensed under the MIT License.

---

## Credits

- [Mapbox](https://www.mapbox.com/)
- [Firebase](https://firebase.google.com/)
- [SweetAlert2](https://sweetalert2.github.io/)
