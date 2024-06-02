# 📋 Task Manager Project

## 📝 Overview

The **Task Manager** project is a web-based application designed to help users manage their tasks efficiently. The application allows users to add tasks with specific priorities, update the status of tasks, and manage deleted tasks. 

## ✨ Features

- **➕ Add Tasks**: Users can add new tasks with a title and priority (low, medium, high).
- **🔄 Update Task Status**: Users can change the status of a task between 'pending', 'in-progress', and 'complete'.
- **❌ Remove Tasks**: Users can remove tasks, which are then stored in the 'Deleted Tasks' section.
- **🗑️ Deleted Tasks Management**: Users can view, restore, or permanently delete tasks from the 'Deleted Tasks' section.
- **🔍 Filter Deleted Tasks**: Users can filter deleted tasks by priority and status.

## 📂 File Structure

The project consists of the following files:

- `index.html`: The main page where users can manage their active tasks.
- `deletedTask.html`: The page where users can view and manage deleted tasks.
- `styles.css`: The stylesheet for the application.
- `scripts/index.js`: The JavaScript file containing logic for managing active tasks.
- `scripts/deletedTask.js`: The JavaScript file containing logic for managing deleted tasks.

## 🚀 How to Run the Project

1. **Clone the Repository**: Clone the project repository to your local machine.
2. **Open `index.html`**: Open the `index.html` file in your web browser to start managing tasks.
3. **Navigate to Deleted Tasks**: Use the navigation bar to go to the 'Deleted Tasks' page (`deletedTask.html`).

## 🛠️ Detailed Description

### `index.html`

The main page for managing tasks. It includes:

- A navigation bar with links to 'Home' and 'Deleted Tasks'.
- An input section for adding new tasks with a title and priority.
- A table that displays the tasks with their title, priority, status, and options to remove them.

### `deletedTask.html`

The page for managing deleted tasks. It includes:

- A navigation bar with links to 'Home' and 'Deleted Tasks'.
- Filter options for filtering deleted tasks by priority and status.
- A table that displays deleted tasks with their title, priority, status, and options to restore or permanently delete them.

### `styles.css`

The stylesheet for the application, defining the appearance of the elements on the pages.

### `scripts/index.js`

The JavaScript file that includes:

- **loadTasks()**: Loads tasks from local storage and displays them in the table.
- **getPriorityColor(priority)**: Returns the color associated with a task's priority.
- **addTask()**: Adds a new task to local storage and updates the display.
- **toggleStatus(index)**: Changes the status of a task and updates the display.
- **removeTask(index)**: Moves a task to deleted tasks and updates the display.

### `scripts/deletedTask.js`

The JavaScript file that includes:

- **loadDeletedTasks()**: Loads deleted tasks from local storage and displays them in the table.
- **displayDeletedTasks(tasks)**: Displays a given list of deleted tasks.
- **getPriorityColor(priority)**: Returns the color associated with a task's priority.
- **restoreTask(index)**: Restores a task from deleted tasks back to active tasks.
- **deleteTaskPermanently(index)**: Permanently deletes a task from deleted tasks.
- **filterTasks()**: Filters deleted tasks based on selected priority and status.

## 💾 Local Storage

The application uses local storage to persist tasks and deleted tasks. This ensures that tasks are saved even when the browser is closed and reopened.

