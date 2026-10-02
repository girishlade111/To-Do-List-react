# To-Do List (React)

A feature-rich React to-do list component (`To-Do List`) — a single drop-in component
(`export default function TodoList()`) with task management, file attachments, and a
dark/light theme toggle.

## Features

- **Task management** — add, complete (checkbox), and delete tasks
- **File attachments** — attach files to tasks (id, name, type, size, URL metadata)
- **Theme toggle** — dark/light mode with sun/moon icons, persisted via `localStorage`
- **Persistence** — tasks saved to `localStorage`, restored on reload
- Animated UI with Framer Motion; styled with shadcn/ui (`Button`, `Input`, `Checkbox`,
  `Card` components) and Lucide icons

## Tech stack

- React (hooks: `useState`, `useEffect`, `useRef`) with TypeScript types
- Framer Motion (animations)
- shadcn/ui components
- Lucide React (icons)

## Usage

This is a **standalone component file**, not a runnable app. To use it, drop the
`To-Do List` file into a React project that has shadcn/ui set up (with
`components/ui/button`, `components/ui/input`, `components/ui/checkbox`,
`components/ui/card`), rename it to `TodoList.tsx`, then:

```tsx
import TodoList from "./TodoList";

export default function App() {
  return <TodoList />;
}
```

## Project structure

```
.
├── To-Do List   # the React component source (rename to .tsx when reusing)
└── README.md
```

## Deploy notes

Not deployed — this repo ships a reusable component, not a website.

---

Built by Girish Lade — https://ladestack.in
