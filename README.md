# 爱的告白网站

这是一个为暄暄小朋友准备的特别礼物网站。

## 如何部署到GitHub Pages

### 方法一：使用GitHub Desktop（推荐）

1. **创建GitHub仓库**
   - 在GitHub上创建一个新的仓库
   - 仓库名称可以是 `love-letter` 或任何您喜欢的名称

2. **克隆仓库到本地**
   - 使用GitHub Desktop克隆仓库到本地
   - 将本文件夹中的所有文件复制到克隆的仓库文件夹中

3. **提交和推送**
   - 在GitHub Desktop中添加所有文件
   - 填写提交信息，例如 "初始化项目"
   - 点击 "提交到main" 然后 "推送起源"

4. **启用GitHub Pages**
   - 访问GitHub上的仓库页面
   - 点击 "Settings"（设置）
   - 在侧边栏中选择 "Pages"
   - 在 "Source"（源）部分，选择 "Deploy from a branch"（从分支部署）
   - 选择 "main" 分支，然后点击 "Save"（保存）
   - 等待几分钟，GitHub将为您生成网站URL

### 方法二：使用命令行

1. **创建GitHub仓库**
   - 在GitHub上创建一个新的仓库

2. **初始化Git并推送**
   ```bash
   cd 项目文件夹路径
   git init
   git add .
   git commit -m "初始化项目"
   git remote add origin https://github.com/您的用户名/仓库名称.git
   git branch -M main
   git push -u origin main
   ```

3. **启用GitHub Pages**
   - 按照方法一中的步骤4操作

## 注意事项

1. **文件路径**
   - 确保所有资源文件（图片、音频）都与index.html在同一目录下
   - 网站使用相对路径引用资源，确保部署时路径正确

2. **音频文件**
   - 网站使用2.m4a和5.m4a作为背景音乐
   - 如果音频文件无法播放，网站功能不会受到影响，只是没有背景音乐

3. **自定义域名（可选）**
   - 如果需要使用自定义域名，请在仓库根目录创建一个名为`CNAME`的文件
   - 在CNAME文件中写入您的域名，例如 `example.com`
   - 然后在您的域名DNS设置中添加CNAME记录指向 `您的用户名.github.io`

## 故障排除

- **资源加载失败**：检查文件是否正确上传到GitHub仓库
- **页面显示不完整**：尝试清除浏览器缓存后重新加载
- **GitHub Pages未生效**：确保已正确配置Pages设置，并且等待足够时间让GitHub处理部署

祝您使用愉快！