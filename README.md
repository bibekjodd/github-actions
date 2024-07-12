# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

<!-- YOUTUBE:START -->
- [Pass The Phone To…](https://www.youtube.com/watch?v=XhuisK0bTSA)
- [How Many Balloons Does It Take To Fly?](https://www.youtube.com/watch?v=lkCRPp7cnP8)
- [I Built 100 Houses And Gave Them Away!](https://www.youtube.com/watch?v=KkCXLABwHP0)
- [World’s Deadliest Obstacle Course!](https://www.youtube.com/watch?v=PWirijQkH4M)
- [$10,000 Every Day You Survive In The Wilderness](https://www.youtube.com/watch?v=U_LlX4t0A9I)
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
