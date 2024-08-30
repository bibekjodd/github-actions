# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

<!-- YOUTUBE:START -->
- [Real Or Cake For $10,000](https://www.youtube.com/watch?v=QtD-CeUdRUQ)
- [7 Days Stranded In A Cave](https://www.youtube.com/watch?v=ndAQfTzlVjc)
- [Running With Bigger And Bigger Feastables](https://www.youtube.com/watch?v=AydS-vA3qa4)
- [Survive 100 Days In Nuclear Bunker, Win $500,000](https://www.youtube.com/watch?v=UPrkC1LdlLY)
- [Spot The Fake Animal For $10,000](https://www.youtube.com/watch?v=8bTQMDM4qvY)
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
