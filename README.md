# LangGraph Project Starter

This repository contains the foundational setup for building stateful, multi-actor applications with **LangGraph** using TypeScript.

## 🚀 Quick Start

### 1. Initialize and Install Dependencies

Run the following commands in your terminal to set up the project structure and necessary packages:

```bash
# Initialize project
npm init -y

# Install dev dependencies (TypeScript and tsx for execution)
npm i -D typescript @types/node tsx

# Install environment management
npm i dotenv
```

### 1. Configure Typescript

Create a tsconfig.json file in the root directory with the following configuration:

```bash
{
  "compilerOptions": {
    "module": "esnext",
    "target": "ES2022",
    "moduleResolution": "bundler",
    "lib": ["ES2022", "DOM"],
    "esModuleInterop": true,
    "resolveJsonModule": true,
    "strict": true,
    "skipLibCheck": true,
    "noEmit": true,
    "types": ["node"]
  },
  "include": ["src"]
}
```

### 3. Project Structure

Create these essential files in your root directory:

- .gitignore (Add node_modules and .env)
- .env (For your API keys)
- src/index.ts (Your application entry point)
- src/env.ts (initialize dotenv config)

### 4. Usage

To run your project during development without a manual build step

```bash
npx tsx src/index.ts
```

### 5. Folder Layout
```bash
.
├── src/
│ └── index.ts
├── .env
├── .gitignore
├── package.json
└── tsconfig.json
