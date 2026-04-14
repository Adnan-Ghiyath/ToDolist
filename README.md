# ✅ My Tasks — Todo List App

A clean and responsive **Todo List** web application built with **React** and **Material UI**, featuring full CRUD operations and persistent local storage.

---

## 🚀 Live Demo

> _Coming soon — deploy to [Vercel](https://vercel.com/) or [Netlify](https://netlify.com/) for a live link_

---

## 📸 Preview

> _Add a screenshot here after running the app_

---

## ✨ Features

- ➕ **Add Tasks** — quickly add new tasks with a title
- ✏️ **Edit Tasks** — update task title and details via a dialog
- 🗑️ **Delete Tasks** — confirm before deleting with a dialog
- ✅ **Mark as Completed** — toggle task completion status
- 🔍 **Filter Tasks** — view All / Completed / Not Completed
- 💾 **Persistent Storage** — tasks are saved in `localStorage` and survive page refresh
- 🔔 **Toast Notifications** — feedback messages on add, edit, and delete actions

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **React 19** | UI framework |
| **Material UI (MUI v7)** | Component library & styling |
| **useReducer + Context API** | Global state management |
| **localStorage** | Data persistence |
| **UUID** | Unique IDs for tasks |

---

## 📁 Project Structure

```
src/
├── App.js                   # Root component with theme & providers
├── App.css
├── TodoList/
│   ├── TodoList.js          # Main list component (add, filter, dialogs)
│   ├── ToDo.js              # Single task card component
│   ├── UserContext.js       # Todos state context (useReducer)
│   └── TostContext.js       # Toast notification context
├── Reducers/
│   └── todoReducers.js      # Reducer: added / deleted / Updated / Get / Checked
public/
├── index.html
└── Fonts/                   # Custom font (KaushanScript)
```

---

## ⚙️ Getting Started

### Prerequisites
- Node.js ≥ 16
- npm

### Installation

```bash
# Clone the repository
git clone https://github.com/your-username/todo-list-app.git

# Navigate to the project folder
cd todo-list-app

# Install dependencies
npm install

# Start the development server
npm start
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 📦 Available Scripts

| Script | Description |
|---|---|
| `npm start` | Run the app in development mode |
| `npm test` | Launch the test runner |
| `npm run build` | Build for production |

---

## 🧠 How It Works

State is managed globally using **React's `useReducer` + Context API**. All actions (add, delete, update, toggle, load) go through `todoReducers.js`. Every state change is automatically synced to `localStorage` so tasks persist across sessions.

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
