

## 运行步骤


### 准备node环境

https://nodejs.org/zh-cn/download


### 安装pnpm

```sh
npm install pnpm -g
```

### 安装依赖

```sh
pnpm install
```

### 开发环境运行

```sh
pnpm dev
```

### 生产环境构建

```sh
pnpm build
```



### nginx部署


```
server {
    listen 80;
    server_name localhost;
    root /usr/share/nginx/html;
    index index.html;

    location / {
        try_files $uri $uri/ /index.html;
    }
}
```

## 注意

浏览器调试的时候，可以关闭sw.js的注册

application--> service workers


## 视频教程

https://www.youtube.com/watch?v=L_sii6bwnEs