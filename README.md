# 文件格式转换器

一个现代化的文件格式转换工具，界面基于 PySide6 和 PySide6-Fluent-Widgets 开发，支持多种文件格式的转换。

## 功能特点

- 现代化的 Fluent Design 界面设计（基于 PySide6 + PySide6-Fluent-Widgets）
- 支持多种文件格式转换：
  - 视频格式：MP4, AVI, MOV, FLV, MKV, WMV, WEBM, M4V, 3GP
  - 音频格式：MP3, WAV, AAC, FLAC, M4A, OGG, WMA
  - 图片格式：JPG, PNG, BMP, GIF, WEBP, TIFF, ICO, SVG
  - 文档格式：PDF, DOCX, DOC, TXT, RTF, ODT, PAGES
  - 演示格式：PPT, PPTX, KEY, ODP
  - 表格格式：XLS, XLSX, CSV, ODS
- 支持拖拽文件到主窗口直接新建转换任务，拖拽方式与手动新建任务等价
- 双主题切换(支持浅色和深色主题)，界面元素自适应主题变化
- 弹窗带有丝滑遮罩与淡入淡出动画，体验与系统 MessageBox 一致
- 卡片、按钮等控件样式自适应主题，界面风格统一
- 开机自启动选项
- 检测安装ffmpeg（可在程序内安装）

## 从Microsoft Store下载安装

- 点击后将自动跳转Microsoft Store进行安装
<a href="https://apps.microsoft.com/detail/9nstl7thhqzj?referrer=appbadge&launch=true&mode=full">
	<img src="https://get.microsoft.com/images/en-us%20dark.svg" width="200"/>
</a>

## 源代码运行说明

1. 确保已安装 Python 3.7 或更高版本
2. 克隆或下载本项目
3. 安装依赖：
   ```bash
   pip install -r requirements.txt
   ```
4. 运行程序：
   ```bash
   python format_converter.py
   ```

## 使用说明

1. 启动程序后，点击"新建任务"或直接拖放文件到程序窗口
2. 选择要转换的文件
3. 从可用的目标格式列表中选择需要转换的格式
4. 选择保存位置（默认为源文件位置）
5. 点击"开始转换"按钮
6. 在任务列表中查看转换进度
7. **开发者邮箱:2713615817@qq.com**

### FFmpeg说明

本软件使用FFmpeg进行音视频转换，您无需手动安装FFmpeg：

1. 打开运行时，软件会自动检测系统是否已安装FFmpeg
2. 如果未检测到FFmpeg，软件会提示安装并在用户点击确定安装后自动完成全过程
3. 安装过程包括：
   - 下载FFmpeg（优先从官方源下载，网络问题时使用内置备用包）
   - 解压并配置FFmpeg
   - 自动添加到用户环境变量
4. FFmpeg安装完成后可立即使用，无需重启软件或系统

您也可以在"设置"界面手动检测、安装或卸载FFmpeg。

## 系统要求

- 操作系统：Windows 10+
- Python 3.7+
- FFmpeg（用于音视频转换,可在程序内安装）

## 开发说明

本项目使用以下主要技术：

- PySide6：Qt for Python
- PySide6-Fluent-Widgets：Fluent Design 风格的 Qt 控件
- ffmpeg：音视频处理

## 许可证

本项目采用 GNU 通用公共许可证第3版（GPLv3）。这意味着：

1. 自由使用：您可以自由地使用、修改和分发本软件。
2. 开放源代码：如果您分发本软件的修改版本，您必须同时提供源代码。
3. 相同方式共享：任何基于本软件的衍生作品必须使用相同的许可证（GPLv3）。
4. 专利授权：本许可证明确授予专利权利。
5. 无担保声明：本软件按"原样"提供，不提供任何形式的保证。

详见 [LICENSE](LICENSE) 文件或访问 [GNU GPLv3](https://www.gnu.org/licenses/gpl-3.0.html)。

## 开源声明

本软件是一个完全开源的文件格式转换工具，基于自由软件精神构建：

1. 开源协议
   - 本软件是自由软件，任何人都可以自由使用、修改和分发
   - 修改版本必须同样采用 GPLv3 许可证
   - 分发时必须提供完整的源代码

2. 使用建议
   - 建议在进行批量转换时先测试单个文件
   - 建议在转换重要文件前进行备份
   - 如遇到问题，欢迎在项目仓库提交 issue 或贡献代码

## 免责声明

1. 基本声明
   - 本软件是一个自由的文件格式转换工具
   - 按"现状"免费提供，不提供任何形式的保证

2. 文件安全
   - 建议在转换重要文件前进行备份
   - 某些格式转换可能会损失部分格式信息

3. 第三方依赖
   - 本软件使用了多个开源第三方库
   - 这些库的使用遵循其各自的开源协议

注意：这是一个自由软件的文件格式转换工具，目的是帮助用户便捷地进行文件格式转换。使用过程中如有任何问题或建议，欢迎在项目仓库参与讨论和贡献。 
