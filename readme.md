monorepo可以很好地管理多个项目的依赖关系，提高开发效率. 这在有前后端的项目中有很大帮助. 即使不是前后端分离的传统项目, 在需要SSR的项目中(比如NextJS), 后端的使用和管理也是非常有必要的

monorepo主要使用pnpm来管理依赖关系. 可以在根目录下的pnpm-workspace.yaml文件中配置多个项目的路径. 虽然也可以npm, 但是效果没有pnpm好.  

在根目录下执行依赖安装
```bash
pnpm install
```

启动:
```bash
## 启动前端
pnpm dev:fastlane-vue

## 启动后端
pnpm dev:paypal-nest-server
```