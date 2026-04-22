# WebInvert-DarkMode (网页颜色反转 - 深色模式)

A lightweight Tampermonkey userscript that allows you to manually toggle color inversion on any website, providing an instant dark mode experience to protect your eyes. 一款轻量级的 Tampermonkey 篡改猴脚本，允许你手动切换网页的颜色反转，提供即时的深色模式体验，保护你的眼睛。

## ✨ Features (功能特点)

- **Manual Toggle (手动控制)**: Toggle dark mode on or off via the Tampermonkey extension menu. (通过篡改猴菜单栏手动开启或关闭深色模式。)
- **Domain-Specific Memory (域名记忆)**: The script remembers your preference for each specific website domain. (脚本会独立记住你在每个域名的开关设置。)
- **Smart Media Handling (智能媒体处理)**: Images, videos, and canvas elements are double-inverted to retain their original colors. (智能处理图片、视频和画布元素，保持其原本颜色不失真。)
- **Zero Impact on Unused Sites (零性能损耗)**: Only injects styles when enabled, keeping your browsing fast and clean. (仅在开启状态下注入样式，不影响未开启网页的加载速度。)

## 🚀 Installation (安装说明)

1. First, install the [Tampermonkey](https://www.tampermonkey.net/) extension for your browser. (首先，在你的浏览器上安装 Tampermonkey 扩展插件。)
2. Click **Create a new script** in the Tampermonkey dashboard. (在篡改猴管理面板中点击**添加新脚本**。)
3. Copy the script code and paste it into the editor. (复制本项目中的脚本代码并粘贴到编辑器中。)
4. Save the script (Ctrl+S or Cmd+S). (保存脚本。)

## 💡 Usage (使用方法)

1. Open any website you want to read in dark mode. (打开任何你想使用深色模式阅读的网站。)
2. Click the Tampermonkey icon in your browser toolbar. (点击浏览器工具栏中的篡改猴图标。)
3. Click on **🌙 开启反转模式** (Turn on Invert Mode). (点击菜单中的 **🌙 开启反转模式**。)
4. The page will instantly reload with dark mode applied. To turn it off, simply click **✨ 恢复正常模式** (Restore Normal Mode) from the same menu. (页面会自动刷新并应用深色模式。如需关闭，再次点击菜单中的 **✨ 恢复正常模式** 即可。)

## 🛠️ Technical Details (技术细节)

This script uses CSS `filter: invert(1) hue-rotate(180deg)` to invert the lightness of the page while preserving the original color hues as much as possible. It runs at `document-start` to ensure the styles are applied as early as possible to prevent bright flashes.

此脚本利用 CSS 的 `filter: invert(1) hue-rotate(180deg)` 属性，在反转页面亮度的同时最大程度地保留原始色相。脚本在 `document-start` 阶段运行，确保尽早应用样式，防止页面加载时出现刺眼的白光。

## 📄 License (开源协议)

[MIT License](https://www.google.com/search?q=LICENSE) - Feel free to use, modify, and distribute this script! (基于 MIT 协议开源，欢迎自由使用、修改和分发！)
