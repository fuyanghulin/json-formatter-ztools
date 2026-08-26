# JSON 格式化（ZTools 插件）

一个完全离线的 JSON/JSON5 格式化、校验与树形查看工具。项目结构参考同级的 `sql-formatter-ztools`，交互能力参考 JSON-handle，但实现为独立、无广告、无网络权限的 ZTools 插件。

## 功能

- 标准 JSON 与 JSON5（注释、尾逗号、未加引号 key）解析
- 固定 2 空格缩进与递归 Key 排序
- 可折叠树形视图、类型着色、节点路径/值复制与节点编辑
- 清晰的解析错误行列提示
- 粘贴自动识别、输入自动格式化、本地偏好保存与快捷键
- 浅色/深色主题与自适应全屏布局，所有数据仅在本地处理

## 开发与打包

```bash
npm install
npm run dev
npm test
npm run build
npm run package
npm run verify
```

发布产物位于 `release/`：

- `json-formatter-1.0.0.zpx`：ZTools 安装包
- `json-formatter-1.0.0.zip`：兼容 ZIP 安装包

快捷键：`Ctrl + Enter` 立即格式化，`Ctrl + Shift + C` 复制结果，`Ctrl + Shift + V` 从剪贴板粘贴。
