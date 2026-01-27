

## 运行步骤

### 安装依赖

```sh
pnpm install
```

### 开发环境编译与热重载

```sh
pnpm dev
```

### 生产环境类型检查、编译与压缩

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

