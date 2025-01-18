# Counter App with useState Hook

## Project Overview
This project demonstrates a simple counter application built with Next.js and React, utilizing the useState Hook for local state management.

## Features
- Increment/decrement counter functionality
- Prevents counter from going below 0
- Dynamic messages based on counter value
- Responsive design with Tailwind CSS
- Interactive UI elements with hover effects

## Technical Implementation

### Directory Structure
```
alx-project-0x04/
├── pages/
│   ├── _app.tsx
│   └── counter-app.tsx
├── components/
│   └── layouts/
│       └── Layout.tsx
└── styles/
    └── globals.css
```

### Key Components

#### Counter App Component (`pages/counter-app.tsx`)
```typescript
const CounterApp: React.FC = () => {
  const [count, setCount] = useState(0);

  const increment = () => {
    setCount(count + 1);
  };

  const decrement = () => {
    setCount(count > 0 ? count - 1 : 0);
  };
  ...
}
```

### Core Features
1. State Management
   - Uses React's useState Hook
   - Local state management within component
   - Simple increment/decrement operations

2. UI Features
   - Gradient background
   - Animated buttons
   - Emoji feedback
   - Conditional messages
