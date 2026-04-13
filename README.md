# SystemProxy - Free Clash Subscribe

[![Python](https://img.shields.io/badge/Python-3.8+-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Clash](https://img.shields.io/badge/Clash-Compatible-7B1FA2?logo=amilia)](https://github.com/Dreamacro/clash)

自动更新 Clash 订阅配置，支持手动和 crontab 两种运行方式。

> All Proxies Are Collected From Public Content On The Internet.

## Features

| Feature | Description |
|---------|-------------|
| 🚀 **Auto Update** | 自动抓取并更新代理节点 |
| ⏰ **Crontab Support** | 支持定时任务，自动化运行 |
| 🌐 **Multi-Config** | 提供普通配置、美国节点配置等多种订阅 |
| 📦 **YAML Ready** | 输出 Clash 原生 YAML 格式，导入即用 |

## Quick Start

### 方式一：Clash 订阅（推荐）

直接在 Clash 客户端中添加以下订阅链接：

| 配置类型 | 订阅链接 |
|---------|---------|
| **标准节点** | `https://raw.githubusercontent.com/SnapdragonLee/SystemProxy/master/dist/clash_config.yaml` |
| **Extra（不推荐）** | `https://raw.githubusercontent.com/SnapdragonLee/SystemProxy/master/dist/clash_config_extra.yaml` |
| **美国节点** | `https://raw.githubusercontent.com/SnapdragonLee/SystemProxy/master/dist/clash_config_extra_US.yaml` |

> 💡 **提示**：导入后可在 Clash 客户端中选择节点或开启自动选择。

### 方式二：本地运行

```bash
# 克隆仓库
git clone https://github.com/SnapdragonLee/SystemProxy.git
cd SystemProxy

# 安装依赖
pip install -r requirements.txt

# 运行脚本
python clash.py           # 生成标准配置
python clash_extra_xx.py   # 生成 Extra 配置
```

运行后，生成的 YAML 文件会保存在 `./dist/` 目录，导入到 Clash 客户端即可使用。

## Clash 订阅 URL 速查

```
标准订阅：
https://raw.githubusercontent.com/SnapdragonLee/SystemProxy/master/dist/clash_config.yaml

美国节点：
https://raw.githubusercontent.com/SnapdragonLee/SystemProxy/master/dist/clash_config_extra_US.yaml
```

## 目录结构

```
SystemProxy/
├── clash.py              # 主脚本 - 生成标准配置
├── clash_extra_xx.py      # Extra 配置脚本
├── dist/                  # 生成的 YAML 配置输出目录
│   ├── clash_config.yaml
│   ├── clash_extra_xx.yaml
│   └── clash_config_extra_US.yaml
└── requirements.txt      # Python 依赖
```

## 常见问题

**Q: 订阅链接无法使用？**
A: 尝试使用镜像地址（如 ghfast.top）或手动运行脚本生成配置。

**Q: 如何定时自动更新？**
A: 在服务器上设置 crontab 定时任务，每日自动运行脚本更新配置。

**Q: Clash 客户端推荐？**
A: Windows 推荐 [Clash for Windows](https://github.com/Fndroid/clash_for_windows_pkg)，macOS 推荐 [ClashX](https://github.com/yichengchen/clashX)，Android 推荐 [Clash for Android](https://github.com/Kr328/ClashForAndroid)。

## License

MIT License

---

*README optimized with [Gingiris README Generator](https://gingiris.github.io/github-readme-generator/)*
