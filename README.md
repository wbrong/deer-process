## 小鹿进程

vue3.0 vite element-plus
**删减版**~

### 依赖
```sh
npm install
```

### 运行
```sh
npm run dev
```

### 打包
```sh
npm run build
```

### 预览
```sh
npm run preview
```

### 其它
- 登录账号密码加密采用：`crypto-js`
    
    npm i crypto-js

- 登录完成需存储token，采用`pinia`和`pinia`持久化存储

    npm i pinia pinia-plugin-persist

- setup语法糖插件 ： `unplugin-auto-import` 解决场景 ： 在组件中开发无需每次都引入 import { ref }..

		npm i unplugin-auto-import -D

- 配置：`vite.config.js`
```js
import AutoImport from 'unplugin-auto-import/vite'
  export default defineConfig({
    plugins: [
      AutoImport({
        imports:['vue','vue-router'] //自动导入vue和vue-router相关函数
      })
    ],
  })
```