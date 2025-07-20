# 部署说明 🚀

这个文档将指导你如何部署你的GitBook项目。

## 方式1：GitHub Pages自动部署（推荐）

我已经为你配置了GitHub Actions，可以自动构建和部署：

### 启用步骤：

1. **启用GitHub Pages**
   - 进入仓库的 `Settings` 页面
   - 找到 `Pages` 选项
   - 在 `Source` 中选择 `GitHub Actions`

2. **自动触发部署**
   - 每次推送代码到 `main` 分支都会自动触发部署
   - 在 `Actions` 页面可以查看部署进度

3. **访问你的GitBook**
   - 部署完成后，可以通过以下地址访问：
   - `https://scudfei.github.io/my-new-repo/`

### 部署状态检查：
- 进入仓库的 `Actions` 标签页
- 查看工作流运行状态
- 如果有错误，可以点击查看详细日志

## 方式2：GitBook官网部署

### 步骤：

1. **注册GitBook账号**
   - 访问 https://www.gitbook.com/
   - 注册或登录账号

2. **连接GitHub仓库**
   - 点击 "Import from GitHub"
   - 授权GitBook访问你的GitHub
   - 选择 `my-new-repo` 仓库

3. **配置和发布**
   - GitBook会自动识别你的文档结构
   - 选择发布设置
   - 点击发布

## 方式3：本地预览

如果你想在本地预览GitBook：

### 安装GitBook CLI：
```bash
npm install -g gitbook-cli
```

### 在仓库目录运行：
```bash
# 安装插件
gitbook install

# 本地预览（默认端口4000）
gitbook serve

# 构建静态文件
gitbook build
```

### 访问本地预览：
- 打开浏览器访问 `http://localhost:4000`

## 自定义配置

### 修改book.json配置：
- 可以添加更多插件
- 修改主题设置
- 调整语言和样式

### 常用插件推荐：
- `search` - 搜索功能
- `sharing` - 分享按钮
- `copy-code-button` - 代码复制按钮
- `back-to-top-button` - 返回顶部
- `expandable-chapters` - 可折叠章节

## 故障排除

### 如果GitHub Actions部署失败：
1. 检查 `book.json` 格式是否正确
2. 确保所有引用的文件都存在
3. 查看Actions日志中的具体错误信息

### 如果页面无法访问：
1. 确认GitHub Pages已正确配置
2. 等待几分钟让部署完成
3. 检查仓库是否为公开状态

### 如果本地预览失败：
1. 确保Node.js版本兼容（推荐14+）
2. 重新安装gitbook-cli
3. 清除缓存：`gitbook install --gitbook-version=3.2.3`

## 下一步

✅ **你的GitBook已经准备就绪！**

1. 🔧 启用GitHub Pages部署
2. 📝 开始编辑你的内容
3. 🎨 自定义样式和配置
4. 📤 分享你的文档链接

---

**恭喜！** 你现在拥有了一个功能完整的GitBook项目！🎉