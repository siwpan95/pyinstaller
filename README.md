# PyInstaller 批量打包工具集

## 仓库角色定位（投资组合分级 ②）

> 本仓在 siwpan 投资组合（D:/projects/repos，共 133 仓）中定级为 **② 保留**，领域 **开发者/系统工具**。
> **角色**：内部工具。
> **维护策略**：② 旗舰 / 枢纽仓库打磨保留，作为能力展示或收敛点；② 保留类仓库低优先维持、不主动扩张。
> 投资组合统一分级索引（多机可查）：[组合分级决策索引 · allin 事实源](https://gitee.com/siwpan/allin/blob/master/docs/事实源/组合分级决策索引.md)。

> 仓库：<https://gitee.com/siwpan/pyinstaller> ｜ 许可：MIT（见 [LICENSE](LICENSE)）

多功能 PyInstaller 批量打包工具箱，从基础到专业级打包。

## 功能

- **基础版 (all.py)** — Tkinter GUI，勾选 .py 文件批量打包
- **专业版 (packer_pro.py)** — 强化 GUI，支持单文件/多文件架构、PNG→ICO、数字签名 (signtool)、附加数据、隐藏导入
- **全自动 (全宝.bat)** — 自动打包当前目录所有 .py 文件
- **智能版 (全能宝.bat)** — 自动检测 tkinter/PyQt/PySide 选择 GUI 模式，支持 UPX 压缩
- **通用打包.bat** — 手动选择单个 .py 打包
- **图标.bat** — 图标格式转换工具

## 快速开始

```bash
# 安装依赖
pip install pyinstaller Pillow

# 基础 GUI
python all.py

# 专业 GUI
python packer_pro.py

# 批处理打包
全宝.bat
```

## 项目结构

```
pyinstaller/
├── all.py          # 基础版 GUI
├── packer_pro.py   # 专业版 GUI (增强功能)
├── 全宝.bat        # 全自动打包批处理
├── 全能宝.bat      # 智能打包批处理
├── 通用打包.bat    # 手动单文件打包
├── 图标.bat        # 图标转换
├── 图标.ico        # 默认图标
└── dist/           # 打包输出
```

## 依赖

- Python >= 3.8
- pyinstaller, Pillow (可选), Windows SDK signtool (可选), UPX (可选)
