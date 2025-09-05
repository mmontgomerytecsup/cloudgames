# CloudGames

CloudGames is a modern web application template that combines **React**, **Unity**, and **TypeScript** using [Vite](https://vitejs.dev/) for lightning-fast development and hot module replacement (HMR).

## Features

- ⚡ **Vite** for instant reloads and optimized builds
- ⚛️ **React** for building interactive UIs
- 🎮 **Unity** integration for rich game experiences
- 🦾 **TypeScript** for type safety and better developer experience
- 🧹 **ESLint** with recommended rules for code quality

## Getting Started

1. **Install dependencies:**
   ```bash
   npm install
   ```
2. **Start the development server:**
   ```bash
   npm run dev
   ```
3. **Build for production:**
   ```bash
   npm run build
   ```

## Recommended Plugins

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react) (Babel-based Fast Refresh)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) (SWC-based Fast Refresh)

## ESLint Configuration Tips

For production-grade applications, enhance your ESLint setup:

- Update `parserOptions` in your ESLint config:
  ```js
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
  ```
- Use stricter TypeScript rules:
  - Replace `plugin:@typescript-eslint/recommended` with `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
  - Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Add React linting:
  - Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react)
  - Extend with `plugin:react/recommended` and `plugin:react/jsx-runtime`

## License

This project is licensed under the Tecsup License.
