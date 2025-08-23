# Task Manager App

A beautiful and intuitive task management application built with React Native and Expo. Keep track of your daily tasks with a clean, modern interface.

![Task Manager App](https://images.pexels.com/photos/3243/pen-calendar-to-do-checklist.jpg?auto=compress&cs=tinysrgb&w=800)

## Features

### ✅ Core Functionality
- **Add Tasks**: Create new tasks with custom descriptions
- **Mark Complete**: Toggle task completion status with visual feedback
- **Delete Tasks**: Remove tasks with confirmation dialog
- **Task Statistics**: View progress with completion rates and counts

### 🎨 User Interface
- Clean, modern design with intuitive navigation
- Smooth animations and micro-interactions
- Visual distinction between completed and incomplete tasks
- Responsive design optimized for mobile devices
- Tab-based navigation for future extensibility

### 📱 User Experience
- Real-time task statistics
- Confirmation dialogs for destructive actions
- Keyboard-friendly input handling
- Empty state messaging for new users
- Accessible design with proper touch targets

## Getting Started

### Prerequisites

Make sure you have the following installed:
- Node.js (v16 or later)
- npm or yarn
- Expo CLI (`npm install -g expo-cli`)

### Installation

1. **Clone the repository** (if applicable):
   ```bash
   git clone <repository-url>
   cd task-manager-app
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start the development server**:
   ```bash
   npm run dev
   ```

4. **Run on your device**:
   - Install the Expo Go app on your iOS or Android device
   - Scan the QR code displayed in the terminal
   - Or run `expo start` and follow the instructions

### Development Commands

- `npm run dev` - Start the development server
- `npm run build:web` - Build for web deployment
- `npm run lint` - Run the linter

## Project Structure

```
├── app/
│   ├── (tabs)/
│   │   ├── _layout.tsx      # Tab navigation configuration
│   │   ├── index.tsx        # Main tasks screen
│   │   └── settings.tsx     # Settings and app info
│   ├── _layout.tsx          # Root layout
│   └── +not-found.tsx       # 404 screen
├── components/
│   ├── AddTaskForm.tsx      # Task creation form
│   ├── TaskItem.tsx         # Individual task component
│   └── TaskStats.tsx        # Task statistics display
├── types/
│   └── task.ts              # TypeScript type definitions
└── hooks/
    └── useFrameworkReady.ts # Framework initialization hook
```

## Usage

### Adding Tasks
1. Type your task description in the input field at the top
2. Tap the "+" button or press Enter to add the task
3. Your task will appear at the top of the list

### Managing Tasks
- **Complete a task**: Tap the circular checkbox next to the task
- **Delete a task**: Tap the trash icon and confirm deletion
- **View statistics**: Check the stats cards showing total, completed, and progress

### Navigation
- **Tasks Tab**: Main interface for managing your tasks
- **Settings Tab**: View app information and usage tips

## Technical Details

### State Management
- Uses React's built-in `useState` hook for local state management
- No external state management libraries required
- Proper separation of concerns with component-based architecture

### Data Structure
```typescript
interface Task {
  id: string;          // Unique identifier
  text: string;        // Task description
  completed: boolean;  // Completion status
  createdAt: Date;     // Creation timestamp
}
```

### Key Components
- **TasksScreen**: Main screen managing task list and operations
- **AddTaskForm**: Handles task creation with validation
- **TaskItem**: Individual task display with actions
- **TaskStats**: Real-time statistics and progress tracking

## Platform Support

This app is built with Expo and supports:
- **iOS**: iPhone and iPad
- **Android**: Phones and tablets
- **Web**: Modern browsers (Chrome, Firefox, Safari)

## Contributing

This is a demonstration project showcasing React Native and Expo development best practices. The code is structured for easy extension and modification.

### Potential Enhancements
- Task categories and tags
- Due dates and reminders
- Data persistence with AsyncStorage
- Task search and filtering
- Dark mode support
- Drag and drop reordering

