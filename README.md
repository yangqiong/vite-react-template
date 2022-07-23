# vite-react-template

本文将以`vite`为基础，手把手搭建前端基础框架。

## 包含

- vite
- react
- typescirpt
- prettier
- eslint

* 建议使用[Visual Studio Code](https://code.visualstudio.com/)编辑器

## 开始

### 创建项目 - [vite](https://vitejs.dev/)

- 首先执行`npm create vite@latest`根据提示输入项目名称，例如`vite-react-template`。
- 然后依次选择`react`, `react-ts`。
- 最后根据提示执行下面命令启动项目。

```
cd vite-react-template
npm install
npm run dev
```

### 添加[prettier](https://prettier.io/)并保存的时候自动格式化

- Visual Studio Code 的扩展中安装[Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)插件
- Visual Studio Code 快捷键`Command + Shift P`输入`format`选择`Format Document With...`选择`Configure Default Fomater...`选择`Prettier`
- Visual Studio Code `Preferences -> Settings`搜索`Format On Save`并选中。

### 添加[Eslint]

- 执行`npm install eslint --save-dev`按照 eslint
- 执行`npx eslint --init`配置 eslint
- Visual Studio Code 的扩展中安装 eslint 插件

```
✔ How would you like to use ESLint? · problems
✔ What type of modules does your project use? · esm
✔ Which framework does your project use? · react
✔ Does your project use TypeScript? · No / Yes
✔ Where does your code run? · browser
✔ What format do you want your config file to be in? · JSON
The config that you've selected requires the following dependencies:

eslint-plugin-react@latest @typescript-eslint/eslint-plugin@latest @typescript-eslint/parser@latest
✔ Would you like to install them now? · No / Yes
✔ Which package manager do you want to use? · npm
```

- 打开`App.tsx`会提示`'React' must be in scope when using JSX`错误信息，表明配置成功
- 在`.eslintrc.json`中添加`"react/react-in-jsx-scope": "off"`关闭此错误提示
