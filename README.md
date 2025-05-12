

# **CRUD Application with ReactJS, Node.js, and MongoDB**  
A simple full-stack CRUD (Create, Read, Update, Delete) application built with:  
- **Frontend**: ReactJS  
- **Backend**: Node.js + Express.js  
- **Database**: MongoDB  

## **Features**  
- Add new items (name + description).  
- View all items in a list.  
- Edit existing items.  
- Delete items.  
- Error handling for API requests.  

---

## **Prerequisites**  
- Node.js (v16+)  
- MongoDB (local or cloud connection)  
- npm/yarn  

---

## **Setup Instructions**  

### **1. Backend Setup**  
1. Navigate to the backend folder:  
   ```bash
   cd backend
   ```
2. Install dependencies:  
   ```bash
   npm install
   ```
3. Set up environment variables:  
   Create a `.env` file in the `backend` folder with:  
   ```env
   MONGO_URI=your_mongodb_connection_string
   PORT=5000  # or your preferred port
   ```
4. Start the server:  
   ```bash
   npm start
   ```
   *Server runs on `http://localhost:5000` by default.*  

### **2. Frontend Setup**  
1. Navigate to the frontend folder:  
   ```bash
   cd frontend
   ```
2. Install dependencies:  
   ```bash
   npm install
   ```
3. Start the React app:  
   ```bash
   npm start
   ```
   *Frontend runs on `http://localhost:3000`.*  

---

## **Project Structure**  
```
├── backend/               # Node.js + Express server
│   ├── models/            # MongoDB schema (e.g., `Item.js`)
│   ├── routes/            # API routes (e.g., `items.js`)
│   ├── app.js             # Express server setup
│   └── package.json
│
├── frontend/              # ReactJS app
│   ├── src/
│   │   ├── components/    # Reusable components
│   │   ├── pages/         # Main views (e.g., `ItemList.js`, `AddItem.js`)
│   │   ├── App.js         # Main app router
│   │   └── index.js       # React entry point
│   └── package.json
│
└── README.md
```

---

## **API Endpoints**  
| Method | Endpoint       | Description                |
|--------|---------------|----------------------------|
| GET    | `/api/items`  | Fetch all items            |
| POST   | `/api/items`  | Add a new item             |
| PUT    | `/api/items/:id` | Update an item by ID    |
| DELETE | `/api/items/:id` | Delete an item by ID    |

---

## **Screenshots **  
![Item List](https://github.com/user-attachments/assets/36427d5e-2709-4dfa-80e5-13d6f6c6c984)
List of all items with Add/delete options.
