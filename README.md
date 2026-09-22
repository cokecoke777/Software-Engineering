# 任务看板

课堂实践项目：支持任务管理、三列看板、拖拽、深色模式和浏览器本地持久化。

## 运行

直接打开 `index.html`，或在项目目录运行 `python -m http.server 8000` 后访问 `http://localhost:8000`。项目无需安装依赖。

## 开发记录

每轮遵循「计划 → 执行 → 浏览器确认 → Git commit」。详细目标与确认记录见 [ITERATIONS.md](ITERATIONS.md)。

## 功能与演示

任务可新增、编辑、删除，标题必填、描述选填。看板有待办、进行中、完成三列，卡片可以拖拽。高、中、低优先级分别显示红、黄、绿。深色模式和任务数据保存在当前浏览器。

课堂演示顺序：展示 Git 提交历史；新建高优先级任务；编辑并拖动到进行中；切换深色模式并刷新；确认内容保留；删除任务。

课件推荐 Vue 3、Vite、Tailwind CSS，本项目采用无依赖 HTML、CSS、JavaScript，直接打开 `index.html` 即可运行。

## 浏览器验证

运行 `python -m http.server 8000`，访问 `http://localhost:8000/tests/browser-smoke.html`，页面显示 PASS 表示核心交互通过。测试会清除当前站点的任务数据，请用独立浏览器配置运行。
