# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

<!-- YOUTUBE:START -->
- [World’s Deadliest Obstacle Course!](https://www.youtube.com/watch?v=PWirijQkH4M)
- [$10,000 Every Day You Survive In The Wilderness](https://www.youtube.com/watch?v=U_LlX4t0A9I)
- [Sprinting with More and More Money](https://www.youtube.com/watch?v=T8I165Qxeo8)
- [Giving 1000 Phones Away](https://www.youtube.com/watch?v=i-9V21MqlhY)
- [Bottle Head Smashing World Record Attempt!](https://www.youtube.com/watch?v=f0cXJ6mJxGc)
<!-- YOUTUBE:END -->

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
