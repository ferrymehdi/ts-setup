# TypeScript Project Setup

This project is a basic setup for developing a Node.js application using TypeScript, ts-node, and nodemon for automatic restarts during development.

## Getting Started

### Prerequisites

Ensure you have Node.js installed. You can download it from [nodejs.org](https://nodejs.org/).

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ferrymehdi/ts-setup.git
   cd ts-setup
   ```

2. **Install the dependencies:**
   ```bash
   npm install
   ```

### Project Structure

```
ts-setup/
├── src/
│   └── index.ts
├── .gitignore
├── nodemon.json
├── package.json
├── tsconfig.json
└── README.md
```

### Configuration Files

- **`tsconfig.json`**: TypeScript configuration file.
- **`nodemon.json`**: Nodemon configuration file.

### Available Scripts

- **`npm run build`**: Compiles TypeScript files to JavaScript.
- **`npm run dev`**: Runs the project in development mode with nodemon and ts-node.
- **`npm start`**: Runs the project directly using ts-node.

### Running the Project

1. **Development Mode:**
   ```bash
   npm run dev
   ```

   This will start the project with nodemon, which will watch for changes in the `src` directory and automatically restart the server.

2. **Production Mode:**
   ```bash
   npm run build
   npm start
   ```

   This will compile the TypeScript files into the `dist` directory and run the compiled JavaScript files.

### Example Code

You can find the example TypeScript code in `src/index.ts`:

```typescript
const sayHello = (name: string): string => {
  return `Hello, ${name}!`;
};

console.log(sayHello("World"));
```

### License

This project is licensed under the ISC License.
```
