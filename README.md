# Getting Started with EventHub Frontend



## Overview

**EventHub** is a full-stack web application that allows users to create, browse, join, and manage events. This is the frontend built with React and connected to a Node.js + PostgreSQL backend.

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in development mode.  
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.  
You may also see any lint errors in the console.

### `npm run build`

Builds the app for production to the `build` folder.  
It correctly bundles React in production mode and optimizes the build for the best performance.

### `npm test`

Launches the test runner in the interactive watch mode.  
(Testing is not configured in this project by default.)

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This will copy all configuration files and dependencies into your project for full control.

---

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

---

## Project Features

- 🧾 Create and manage events
- 📅 RSVP and track joined events
- 🧑‍💼 Organizer dashboard with attendee management
- 📷 Event detail pages with image display
- 🔒 Basic login flow using Context API

## Tech Stack

- React 18
- Axios for API calls
- Tailwind CSS for styling
- React Router DOM for routing
- Node.js & Express (backend)
- PostgreSQL (database)

## API Proxy Configuration

This project proxies API requests to the backend using:

```json
"proxy": "http://localhost:5000"
