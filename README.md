# TO DO LIST APPLICATION USING VUE

This project is a Vue.js application for managing a simple **To-Do List**. It demonstrates basic operations and state management using Vue's Composition API.

## Features

- Add new tasks to the list.
- Delete tasks from the list.
- Automatically generates unique indices for tasks.

## Project Structure

### Components
- `Header.vue` - Displays the application header.
- `TaskList.vue` - Renders the list of tasks.
- `AddList.vue` - Provides functionality to add new tasks.

### Core Logic
- **Add Task**: Uses `handleAddingNewTask()` to add a new task with a unique index.
- **Delete Task**: Uses `deleteTask()` to remove tasks by index.
- **Unique Index Generation**: Implements `generateIndex()` to ensure unique task IDs.

## Setup and Usage

### Prerequisites
- Node.js and npm installed.
- Vue CLI installed globally.

### Installation
1. Clone the repository to any project folder.
2. navigate to the project folder that contains the clone repository.
3. Install dependencies using `npm install`
3. Run the application by starting the development server using: `npm run dev`

## License

This project is open-source and available under the MIT License.
