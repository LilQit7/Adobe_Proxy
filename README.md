# 🚫 Adobe_Proxy - Adobe域名代理规则集 🛡️

[![GitHub Stars](https://img.shields.io/github/stars/LilQit7/Adobe_Proxy?style=social)](https://github.com/LilQit7/Adobe_Proxy/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/LilQit7/Adobe_Proxy?style=social)](https://github.com/LilQit7/Adobe_Proxy/network/members)
[![GitHub Issues](https://img.shields.io/github/issues/LilQit7/Adobe_Proxy)](https://github.com/LilQit7/Adobe_Proxy/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/LilQit7/Adobe_Proxy)](https://github.com/LilQit7/Adobe_Proxy/pulls)
[![License](https://img.shields.io/github/license/LilQit7/Adobe_Proxy)](https://github.com/LilQit7/Adobe_Proxy/blob/main/LICENSE)

[![🇨🇳 中文](https://img.shields.io/badge/🇨🇳_中文-当前-blue)](README.md)
[![🇺🇸 English](https://img.shields.io/badge/🇺🇸_English-Available-green)](README_EN.md)

> **⚠️ 免责声明：**
> 
> 本项目仅供学习和研究使用，请遵守相关法律法规和Adobe软件服务条款。用户应当了解各域名的具体用途，并承担使用本规则集可能产生的任何后果。开发者不承担因使用本项目而导致的任何直接或间接损失。

## 📖 项目简介

一个专业的**Adobe全产品线域名代理规则集**，为网络代理工具提供完整的Adobe服务域名管理方案。通过精心整理和分类，帮助用户有效控制Adobe软件的网络访问行为。

### 🎯 核心特性
- **🔍 全面覆盖**：涵盖Adobe全系列产品和服务域名
- **🚀 即插即用**：支持主流代理工具直接使用
- **⚡ 高效精准**：290条精选规则，去重优化
- **🔄 持续维护**：跟踪Adobe服务变化，及时更新

## ✨ 功能矩阵

| 功能特性 | 支持状态 | 描述 |
|----------|----------|------|
| 🛡️ 激活验证阻断 | ✅ | 阻止Adobe软件激活验证 |
| 📊 数据统计拦截 | ✅ | 阻止用户行为数据收集 |
| 🌐 CDN加速控制 | ✅ | 管理Adobe CDN访问 |
| 🔐 安全验证管理 | ✅ | 控制软件安全检查 |
| 📍 地理位置服务 | ✅ | 阻止地理位置相关请求 |
| ☁️ 云服务接口 | ✅ | 管理Adobe云服务访问 |

## 📊 规则统计

<div align="center">

| 📋 项目信息 | 📈 数据统计 |
|-------------|-------------|
| **规则类型** | DOMAIN-SUFFIX |
| **规则数量** | 290条 |
| **最后更新** | 2024-12-19 |
| **覆盖产品** | Adobe全系列 |
| **支持工具** | Clash/Surge/QuantumultX |

</div>

## 🛠️ 快速开始

### 🔧 Clash配置

```yaml
rule-providers:
  adobe:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/LilQit7/Adobe_Proxy/main/Adobe.yml"
    path: ./ruleset/adobe.yaml
    interval: 86400

rules:
  - RULE-SET,adobe,REJECT  # 阻断模式
  # - RULE-SET,adobe,PROXY   # 代理模式
  # - RULE-SET,adobe,DIRECT  # 直连模式
```

### ⚙️ Surge配置

```ini
[Rule]
RULE-SET,https://raw.githubusercontent.com/LilQit7/Adobe_Proxy/main/Adobe.yml,REJECT
```

### 🚀 Quantumult X配置

```ini
[filter_remote]
https://raw.githubusercontent.com/LilQit7/Adobe_Proxy/main/Adobe.yml, tag=Adobe阻断, force-policy=reject, update-interval=86400, opt-parser=false, enabled=true
```

## 📝 域名分类详解

<details>
<summary>🔍 点击展开查看详细分类</summary>

### 🛡️ 激活验证服务
```
licenses.adobe.com, activate.adobe.com, genuine.adobe.com
```

### ☁️ 云服务接口
```
各种 *.adobe.io 域名 (如: p13n.adobe.io, photos.adobe.io)
```

### 📊 分析统计服务
```
adobe.demdex.net, sstats.adobe.com, adobe.tt.omtrdc.net
```

### 🌐 CDN加速域名
```
cc-cdn.adobe.com, assets.adobedtm.com, ssl-delivery.adobe.com
```

### 📍 地理位置服务
```
geo2.adobe.com, presence-ue1.adobe.com
```

### 🔐 安全验证域名
```
auth.services.adobe.com, ims-na1-prprod.adobelogin.com
```

</details>

## 🎛️ 使用模式

| 使用场景 | 策略配置 | 适用情况 |
|----------|----------|----------|
| 🚫 **完全阻断** | `REJECT` | 防止激活验证和数据收集 |
| 🌐 **代理访问** | `PROXY` | 通过代理服务器访问 |
| ⚡ **直接连接** | `DIRECT` | 绕过代理直接访问 |

## ⚠️ 重要提醒

<div align="center">

| ⚠️ 注意事项 | 📝 说明 |
|-------------|----------|
| 🔍 **了解用途** | 使用前请确保了解各域名的具体功能 |
| 🧪 **测试环境** | 建议先在测试环境中验证规则效果 |
| ⚡ **软件功能** | 某些规则可能影响Adobe软件正常功能 |
| 🔄 **定期更新** | 及时检查更新以获取最新规则 |

</div>

## 🤝 参与贡献

我们欢迎所有形式的贡献！

### 🌟 如何贡献

1. **🍴 Fork** 本项目
2. **🌿 创建** 新的功能分支
3. **💻 提交** 您的更改
4. **📤 发起** Pull Request

### 💡 贡献内容

- 🆕 新的Adobe域名发现
- 🐛 规则错误修复
- 📚 文档改进建议
- 🎨 项目优化方案

## 📄 开源协议

本项目采用 [MIT License](LICENSE) 开源协议。

## 🔗 相关资源

| 🛠️ 代理工具 | 📚 官方文档 |
|-------------|-------------|
| **Clash** | [GitHub 仓库](https://github.com/Dreamacro/clash) |
| **Surge** | [官方网站](https://nssurge.com/) |
| **Quantumult X** | [应用主页](https://quantumult.app/) |

## ⭐ Star 历史

如果这个项目对您有帮助，请给个 ⭐ Star 支持一下！

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=LilQit7/Adobe_Proxy&type=Date)](https://star-history.com/#LilQit7/Adobe_Proxy&Date)

</div>

---

<div align="center">

**💻 Made with ❤️ by [LilQit7](https://github.com/LilQit7)**

**⏰ 最后更新时间：2024-12-19**

![Adobe](https://img.shields.io/badge/Adobe-FF0000?style=for-the-badge&logo=adobe&logoColor=white)
![Proxy](https://img.shields.io/badge/Proxy-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![Network](https://img.shields.io/badge/Network-FF6B6B?style=for-the-badge&logo=network&logoColor=white)

</div>
