# 📝 To-Do List Web App

A simple yet powerful to-do list web application built with vanilla HTML, CSS, and JavaScript. No frameworks or external dependencies required!

## Features

✨ **Core Features:**

- ✅ Add new tasks with ease
- 🗑️ Delete tasks individually
- ✔️ Mark tasks as completed
- 🎯 Filter tasks by status (All, Active, Completed)
- 🧹 Clear all completed tasks at once
- 📊 View statistics (Total, Active, Completed)
- 💾 Persistent storage using LocalStorage
- 🎨 Beautiful, responsive UI with smooth animations
- 📱 Mobile-friendly design

## Getting Started

### Prerequisites

- Any modern web browser (Chrome, Firefox, Safari, Edge, etc.)
- No server or installation required

### Installation

1. Download or clone this repository to your computer
2. Extract the files to a folder
3. Open `index.html` in your web browser

**That's it! The app is ready to use.**

## File Structure

```
project/
├── index.html          # HTML structure
├── styles.css          # Styling and animations
├── script.js           # JavaScript functionality
└── README.md           # Documentation (this file)
```

## How to Use

### Adding a Task

1. Type your task in the input field
2. Click the "Add Task" button or press **Enter**
3. Your task will appear at the top of the list

### Managing Tasks

- **Mark as Done**: Click the checkbox next to a task to mark it as completed
- **Delete**: Click the "Delete" button to remove a task
- **View Statistics**: Check the stats bar to see total, active, and completed tasks

### Filtering Tasks

- **All**: View all tasks
- **Active**: View only incomplete tasks
- **Completed**: View only finished tasks

### Clearing Completed Tasks

- Click the "Clear Completed" button to remove all finished tasks at once
- A confirmation dialog will appear before deletion

## Features in Detail

### LocalStorage Integration

- All tasks are automatically saved to your browser's LocalStorage
- Your tasks persist even after closing and reopening the browser
- No account or server needed

### Data Validation

- Empty tasks are not allowed
- XSS protection to prevent malicious input
- HTML special characters are properly escaped

### Responsive Design

- Works seamlessly on desktop, tablet, and mobile devices
- Touch-friendly interface
- Optimized layout for all screen sizes

### User Experience

- Smooth animations and transitions
- Real-time statistics updates
- Empty state messages when no tasks match filter
- Keyboard support (Enter key to add tasks)
- Visual feedback on button interactions

## Keyboard Shortcuts

| Key   | Action       |
| ----- | ------------ |
| Enter | Add new task |

## Browser Compatibility

- ✅ Chrome (60+)
- ✅ Firefox (55+)
- ✅ Safari (12+)
- ✅ Edge (79+)
- ✅ Opera (47+)

## Technical Details

### Technologies Used

- **HTML5**: Semantic markup and structure
- **CSS3**: Flexbox layout, gradients, and animations
- **Vanilla JavaScript**: No frameworks or libraries
- **LocalStorage API**: For persistent data storage

### Key JavaScript Concepts

- DOM manipulation
- Event handling
- Array methods (filter, find, map)
- Object destructuring
- LocalStorage API
- ES6 features

## Code Architecture

### State Management

- `todos`: Main array storing all tasks
- `currentFilter`: Tracks the active filter

### Core Functions

- `addTodo()`: Creates and adds new task
- `deleteTodo(id)`: Removes a task by ID
- `toggleTodo(id)`: Marks task as completed/active
- `clearCompleted()`: Removes all completed tasks
- `renderTodos()`: Updates the UI with filtered tasks
- `getFilteredTodos()`: Returns tasks based on current filter
- `updateStats()`: Updates the statistics display
- `saveTodos()`: Persists tasks to LocalStorage
- `escapeHtml(text)`: Prevents XSS attacks

## Data Structure

Each task object contains:

```javascript
{
  id: 1234567890,           // Unique timestamp-based ID
  text: "Buy groceries",    // Task description
  completed: false,         // Completion status
  createdAt: "6/1/2026..."  // Creation timestamp
}
```

## Future Enhancement Ideas

- 📅 Add due dates for tasks
- 🏷️ Implement task categories or tags
- 🔍 Add search functionality
- 🌙 Dark mode toggle
- 📤 Export tasks as JSON or CSV
- 🔔 Add notifications for due tasks
- 🎨 Allow custom color themes
- 👥 Multi-user support with cloud sync
- ⏱️ Add task duration tracking
- 🔄 Add task priorities and sorting

## Tips & Tricks

1. **Bulk Completion**: You can use the filter to view active tasks and quickly mark them as done
2. **Task Organization**: Add tasks in order of priority
3. **Backup**: Use browser's Storage Inspector to export your data if needed
4. **Mobile Usage**: Save this page as a web app on your phone for quick access

## Troubleshooting

### Tasks not saving?

- Check if LocalStorage is enabled in your browser
- Try clearing browser cache and reloading

### Tasks disappeared?

- Check browser's developer tools (F12) > Application > LocalStorage
- Tasks are stored under the current website URL

### Checkboxes not working?

- Refresh the page
- Make sure JavaScript is enabled in your browser

## Contributing

This is a simple project for learning purposes. Feel free to:

- Modify the styling
- Add new features
- Improve the code
- Create your own version

## License

Free to use and modify for personal or educational purposes.

## Author

Created as a Vanilla JavaScript learning project.

---

**Enjoy organizing your tasks! 🎉**
