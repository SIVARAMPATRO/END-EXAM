# Question 8 – Login and Registration Forms (React + Vite)

**Concept:** React State (Controlled Forms)

A simple React application with a **Registration form** and a **Login form**.
Both forms use `useState()` and controlled inputs (`value` + `onChange`).
No backend, no database, plain CSS only.

## Project Structure

```
login-registration-app/
├── index.html
├── package.json
├── vite.config.js
├── README.md
└── src/
    ├── main.jsx      (renders App into the page)
    ├── App.jsx       (tabs, registration form, login form)
    └── style.css     (all styling)
```

## How to Run

Open the project folder in VS Code, open the terminal (`Ctrl + ~`) and run:

```
npm install
npm run dev
```

Then open the link shown in the terminal (usually `http://localhost:5173`).

> Requires Node.js 18 or newer.

## Demo Login Credentials

| Field    | Value             |
|----------|-------------------|
| Email    | `admin@gmail.com` |
| Password | `1234`            |

## Expected Output

**Terminal after `npm run dev`:**

```
  VITE v5.x.x  ready in 300 ms

  ➜  Local:   http://localhost:5173/
```

**Browser:** a centered card with two tabs, **Register** and **Login**.

**Register tab**
- Leaving any field empty shows: `All fields are required. Please fill in every field.`
- Filling all fields and clicking **Register** shows a green box:
  `Registration Successful!` followed by the entered Name, Email and Password.

**Login tab**
- `admin@gmail.com` / `1234` shows: `Login Successful`
- Any other email or password shows: `Invalid Email or Password`

## Concepts Used

- Functional components
- `useState()` for every input and for messages
- Controlled components (`value` and `onChange`)
- `onSubmit` with `event.preventDefault()`
- Conditional rendering (`{condition && <div>...</div>}`)
