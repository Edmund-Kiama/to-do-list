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

1. Reactive Task List  
   Tasks are stored in a reactive `ref` array, ensuring the UI updates automatically when tasks are added or deleted.

2.  Adding Tasks
    Handles new task submissions using handleAddingNewTask() and generates a unique index for each task.

3.  Deleting Tasks
    Removes tasks by filtering the list based on the unique index.

4.  Unique Index Generation
    Ensures each task has a unique identifier using a simple random number generator.

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
