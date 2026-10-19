# Steps

A small, interactive React component that presents a three-step learning-and-career journey. It is a focused example of state-driven UI: users can move through steps, see completed progress, and show or hide the panel.

## Features

- Three clearly labelled progress steps
- Previous and Next controls with boundary protection
- Visual indication of the current and completed steps
- Toggle button to hide or reveal the steps panel
- Responsive, lightweight styling with no component-library dependency

## Built with

- [React](https://react.dev/)
- [Create React App](https://create-react-app.dev/)
- CSS

## Getting started

### Prerequisites

Install a current LTS release of [Node.js](https://nodejs.org/), which includes npm.

### Installation

1. Clone the repository and enter the project directory.

   ```bash
   git clone <repository-url>
   cd steps
   ```

2. Install dependencies.

   ```bash
   npm install
   ```

3. Start the development server.

   ```bash
   npm start
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Available scripts

| Command         | Description                                                                       |
| --------------- | --------------------------------------------------------------------------------- |
| `npm start`     | Runs the app in development mode.                                                 |
| `npm test`      | Launches the test runner in interactive watch mode.                               |
| `npm run build` | Creates an optimized production build in `build/`.                                |
| `npm run eject` | Copies the Create React App configuration into the project. This is irreversible. |

## How it works

The `Steps` component stores two pieces of UI state:

- `step` tracks the active step, constrained between 1 and 3.
- `isOpen` determines whether the steps panel is visible.

The messages are defined in a single array, so the text shown on screen always corresponds to the active step. The navigation handlers prevent users from moving before the first step or after the last one.

## Project structure

```text
steps/
├── public/          # Static files and application HTML shell
├── src/
│   ├── App.js       # Steps component and interaction logic
│   ├── index.css    # Application styles
│   └── index.js     # React application entry point
├── package.json      # Dependencies and npm scripts
└── README.md
```
