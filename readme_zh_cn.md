# Notepad4-ML (Notepad4-MultiLabel)

[English](readme.md) | **简体中文**

![Notepad4-ML](docs/Notepad4-ml-bar.png)

Notepad4-ML 是基于 [Notepad4](https://github.com/zufuliu/notepad4) 的多标签分支版本，
为这个原本单文档的轻量编辑器增加了标签页与滚动条匹配标记。

  
- **版本**：0.2.1
- **基于上游**：Notepad4 v26.10 (r6392, 7b269f54)
- **上游基线提交**：`3afea94b18c469b95b504553a5ece1a9e4c57d9e`（2026-10-23）
- **许可**：BSD 3-Clause，见 [LICENSE](LICENSE)（全文）与 [NOTICE](NOTICE)（上游版权与分支说明）  

  
> [!IMPORTANT]
> Notepad4-ML **不是** Notepad4 官方版本，也不由 Notepad4 作者维护。  
> 上游项目：<https://github.com/zufuliu/notepad4>  

  
> [!WARNING]
> **本项目的代码改动主要由 AI（大型语言模型）生成，并经人工审阅与自动化测试验证。**
> **如果你需要最稳定、经过长期检验的版本，请使用上游 Notepad4。**  

  
## 本分支新增的功能

**多标签页**
   - 顶部多开文件标签栏，显示文件名与未保存标记 `*`
   - `Ctrl+Tab` / `Ctrl+Shift+Tab` 切换，`Ctrl+W` 关闭，`Ctrl+N` 新建
   - 每个标签独立保存内容、撤销历史、光标、滚动位置、编码、换行符、只读状态
   - 左右拖动标签可调整标签顺序
   - 把标签拖出窗口、放进另一个 Notepad4-ML 窗口即可把该标签移过去（未保存内容一并携带；源标签关闭且不弹保存框）
   - 工具栏：关闭当前标签、在新窗口中打开
   - 此功能你可以自由启用/关闭

  
**垂直滚动条上的匹配标记**
   - “标记全部匹配”或“查找全部”时，在真正的垂直滚动条上按行位置画出标记
   - 滚动时标记保持可见
   - 可设置颜色与不透明度  

## 反馈问题前请先区分责任

提交 issue 前，**请先确认上游 Notepad4 是否也存在同样的问题，上游问题不接受处理**：

1. 从 <https://github.com/zufuliu/notepad4/releases> 下载最新官方 Notepad4
2. 用同样的步骤复现一次
3. 按下表判断应该提交到哪里：

| 现象 | 提交位置 |
| --- | --- |
| 官方 Notepad4 也能复现（语法高亮、编码、打印、词法分析等） | 上游 <https://github.com/zufuliu/notepad4/issues> |
| 只在 Notepad4-ML 出现（标签、滚动条标记、新窗口相关） | 本项目 issue |
| 不确定 | 先在本项目 issue 中说明“官方版本是否复现” |

请在 issue 中写明：

- Notepad4-ML 版本
- Windows 版本
- 复现步骤
- 是否已在官方 Notepad4 上复现

## 下载与使用

Release 中提供 32 /64 位构建  

支持的语言：英语、简体中文、繁体中文、日语、韩语、德语、法语、意大利语、
波兰语、葡萄牙语（巴西）、俄语、斯洛文尼亚语。


## 从源码构建

本分支使用 zig + LLVM-MinGW 工具链构建（脚本不在本仓库内）。
上游原始的构建方式（MSVC / MinGW Makefile）依然可用，见
[上游 Wiki](https://github.com/zufuliu/notepad4/wiki/Build-Notepad4)。

上游项目依赖：Scintilla 5.6.7、Lexilla 5.5.4、Boost.Regex 1.91。

## 其他

请去查阅上游项目  

## 许可证

BSD 3-Clause。本分支保留上游全部版权声明，详见 [LICENSE](LICENSE)。

上游 Notepad4、matepath、Notepad2、Notepad2-mod 的版权归各自作者所有。
