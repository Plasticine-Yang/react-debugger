# React Debugger

A convenient react debugger.

## Usage

For example, let's take debugging React version 18.2.0.

```shell
yarn
yarn install:18-2-0
yarn build:18-2-0
yarn debug:18-2-0
```

Open VSCode, select the desired configuration for the React version you want to debug, and run it. Isn't it simple!

## 问题记录

### Node.js 版本

建议使用 16

### yarn install:18-2-0 的问题

- electron 安装问题
  执行 `yarn install:18-2-0` 会安装 electron，建议通过环境变量配置一下 electron 的镜像源再安装

  ```shell
  export ELECTRON_MIRROR="https://npmmirror.com/mirrors/electron/"
  ```

- 代理问题
  如果设置了 `HTTP_PROXY`, `HTTPS_PROXY`, `ALL_PROXY` 等环境变量，建议先将它们取消掉，否则会出现 `Protocol "https:" not supported. Expected "http:"` 报错
