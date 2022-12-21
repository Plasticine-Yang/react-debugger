# react-debugger

让你轻松调试 react 源码

## Usage

1. 安装依赖

```shell
npm i
```

2. 修改 sourcemap 路径映射

修改 `react/scripts/rollup/build.js` 中的 `getRollupOutputOptions` 函数，在返回的 `sourcemapPathTransform` 方法中配置映射路径

3. 构建 react 源码

```shell
cd react
yarn
yarn build
```

> 执行 yarn 时出现 https 错误不影响 yarn build 的执行
