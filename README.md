<h1 align="center">
  <a href="">
    <img src="/src/assets/state-management.svg" alt="Boiler Plate">
  </a>
</h1>

# React State Management Task Manager with Zustand and useContext Exercise

For this weeks practice you will Create a simple task manager where tasks are managed using Zustand and theme (dark/light mode) is managed using React's useContext.

## Getting Started with the Project

### Dependency Installation & Startup Development Server:

Once cloned, navigate to the project's root directory and this project uses npm (Node Package Manager) to manage its dependencies.

The command below is a combination of installing dependencies, opening up the project on VS Code and it will run a development server on your terminal.

```bash
npm i && code . && npm run dev
```

### Looking for some hints?

## Hints for the Zustand and `useContext` Exercise

1.  Zustand Installation:

    - Zustand isn't included in the boiler plate. You'll need to install it using `npm install zustand`.

2.  State Management with Zustand:

    - When setting up your Zustand store, think of it as a global state container. It should hold all the tasks and provide functions to manipulate them.
    - The `create` function from Zustand is your starting point. It accepts a setter function to help you define the state and its updater functions.

3.  Theme Management with `useContext`:

    - The `useContext` hook in React allows you to access values from a context without prop-drilling. For this exercise, you're using it to manage a theme (light/dark mode).
    - Define a context using `createContext()`. Remember to export both the context and a custom hook (e.g., `useTheme`) to make it easier to access the theme in your components.

4.  Integrating Components:

    - In your main `App.jsx`, integrate both the task manager and theme toggler. This is where you'll see the interplay of Zustand and `useContext`.
    - Ensure that the `ThemeProvider` wraps your entire application so that the theme context is accessible everywhere.

5.  Testing:

    - Before pushing to GitHub, test your application thoroughly. Add tasks, remove them, and toggle the theme. Ensure everything works seamlessly.

6.  Committing and Pushing:

    - Use `git add .` to stage your changes, followed by `git commit -m "Your commit message here"` to commit them.
    - Push your changes to the GitHub repository using `git push origin main`.

7.  Collaboration:

    - If working in pairs or groups, consider using feature branches for different parts of the exercise. This way, you can review each other's code through pull requests.
