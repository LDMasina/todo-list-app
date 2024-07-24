# GIDHub Application (To-Do List) by Lance Masina

This is my simple To-Do List application built with React and TypeScript. Nice and simple The application allows users to add, edit, delete, and mark tasks as completed. The application is basic in it's format but demonstrates state management, CRUD operations, and local storage. For data persistence I opted for local storage use, so your tasks will be saved even after you refresh the page or close the browser.

## How It Works

### Component Structure

1. **TodoApp Component:**
   - This is the main component that holds the state and manages the to-do list.
   - It includes states for `todos`, `text`, and `placeholder`.
   - It uses `useEffect` to load tasks from local storage and save tasks to local storage whenever the `todos` state changes.
   - It includes functions to add, edit, delete, and toggle the completion status of tasks.

2. **TodoForm Component:**
   - This component handles adding new to-do items.
   - It includes an input field for entering the task text and a button to submit the form.
   - The input field's placeholder text dynamically updates based on the number of tasks.

3. **TodoList Component:**
   - This component renders the list of to-dos.
   - It receives the list of tasks and functions to edit, delete, and toggle tasks from the `TodoApp` component.

4. **TodoItem Component:**
   - This component represents a single to-do item.
   - It includes options to edit the task text, delete the task, and toggle its completion status.

### State Management

- The `todos` state holds the list of tasks, each represented by an object with `id`, `text`, and `completed` properties.
- The `text` state holds the current input value for the new task.
- The `placeholder` state dynamically updates the placeholder text in the input field based on the number of tasks.

### Local Storage

- The application uses local storage to persist tasks across browser sessions.
- When the application loads, it fetches tasks from local storage and updates the `todos` state.
- Whenever the `todos` state changes, it updates the local storage with the current list of tasks.

### Dynamic Placeholder Text

- The `placeholder` state starts with the value "Enter your first task".
- After a task is added, it updates to "Enter your next task", providing a clear guide for the user.

## Getting Started

To get started with this project, follow these steps:

### Prerequisites

- Node.js and npm installed on your machine.

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/todo-list-app.git

2. **Navigate to project directory:**
   ```bash
   cd todo-list-app

3. **Install dependencies:**
   ```bash
   npm install

4. **Start dev server:**
   ```bash
   npm start

### Usage

Once you have the server running, you can access the application at http://localhost:3000. Very simple stuff and from there, you can start adding, editing, deleting, and marking tasks as completed.

### Contributing and Feedback

This is a very simple application, that I will iteratively update as I continue to build a more solid proficiency in TypeScript. If you have any suggestions or improvements where I can refactor code to more ideal syntaxes, please feel free to open an issue or submit a pull request. Or reach out to me below...

### Follow Me

- **GitHub:** https://github.com/LDMasina
- **Instagram:** https://instagram.com/lancemasina
- **LinkedIn:** https://linkedin.com/in/lancemasina
