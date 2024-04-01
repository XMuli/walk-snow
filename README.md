## Walk Snow



```bash
npm install -g webpack
npm install -g @vue/cli
npm install -g serve

# Chrome 运行
npm run serve

# 打包为 dist 文件夹
npm run build
serve -s dist

# 通过 electron 打包为 EXE 安装程序
cnpm install --save-dev electron
vue add electron-builder # 安装electron-builder插件
npm run electron:serve   # 运行本地
npm run electron:build   # 打包 EXE

[遇bug1] https://blog.csdn.net/qq_34988204/article/details/133793214 # 报错 background.js from Terser; Error: error:0308010C:digital envelope routines::unsupported
[遇bug2] 三个文件下载失败，https://juejin.cn/post/7250179028648067131
[最后生成EXE文件路径] "./dist_electron\walk-snow Setup 0.1.0.exe" 
```

