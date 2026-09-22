# 任务看板

一个用于课堂实践展示的前端任务管理系统，支持任务增删改查、状态看板、优先级、搜索、拖拽移动、深色模式和浏览器本地持久化。

## 在线访问

GitHub Pages：<https://cokecoke777.github.io/Software-Engineering/>

GitHub 仓库：<https://github.com/cokecoke777/Software-Engineering>

## 主要功能

- 新增、查看、编辑、删除任务
- 按任务标题或描述实时搜索
- 待办、进行中、已完成三列看板
- 任务卡片拖拽切换状态
- 高、中、低优先级视觉区分
- 深色模式切换和持久化
- 使用 `localStorage` 保存任务数据
- 适配桌面端和移动端浏览器

## 本地运行

项目是纯前端静态页面，无需安装依赖。

直接打开 `index.html` 即可运行；也可以在项目目录启动本地服务：

```bash
python -m http.server 8000
```

然后访问：

```text
http://localhost:8000
```

## 技术说明

课件推荐技术选型包括 Vue 3、Vite、Tailwind CSS 和 `localStorage`。本项目采用无依赖的 HTML、CSS、JavaScript 实现前端交互，并使用 `localStorage` 完成数据持久化。

这样处理的原因是项目规模较小，原生实现更直接，GitHub Pages 可以直接部署，课堂演示时不需要安装依赖或运行构建命令。

## 验证方式

浏览器打开 `tests/browser-smoke.html` 可以运行核心交互冒烟测试。测试覆盖新增、编辑、删除、拖拽、搜索、深色模式和刷新持久化。

如果使用本地服务，测试地址为：

```text
http://localhost:8000/tests/browser-smoke.html
```

## 迭代记录

项目按“计划 - 执行 - 确认 - 提交”的流程分轮开发，每轮目标、执行内容、确认方式和可复用提示词见 [ITERATIONS.md](ITERATIONS.md)。

## 演示建议

课堂演示时可以按这个顺序展示：打开线上页面，新增一个高优先级任务，编辑任务内容，把任务拖到进行中，使用搜索栏查询任务，切换深色模式并刷新页面，最后删除任务。
