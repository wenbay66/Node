## Node 開發離不開 npm, 腳本功能是 npm 最常用、最強大的功能之一

# npm 允許在 package.json 使用 scripts 字段定義腳本命令
```javascript
"scripts": {
  "build": "node build.js",
  "test1": "node ./Code/test1.js",
  "test2": "node ./Code/test1.js && node ./Code/test2.js",
  "build1": "echo $npm_package_config_env"
},
"config": {
  "env": "product"
}
```

#### 執行方式
`npm run build`

#### 運行一個js
`npm run test1`

#### 同時運行兩個js
 `npm run test2`

#### npm 允許使用 scripts 字段讀取 config
 input:  `npm run build1`
 output  `product`
