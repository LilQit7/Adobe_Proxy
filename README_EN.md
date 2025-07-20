# 🚫 Adobe_Proxy - Adobe Domain Proxy Ruleset 🛡️

[![GitHub Stars](https://img.shields.io/github/stars/LilQit7/Adobe_Proxy?style=social)](https://github.com/LilQit7/Adobe_Proxy/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/LilQit7/Adobe_Proxy?style=social)](https://github.com/LilQit7/Adobe_Proxy/network/members)
[![GitHub Issues](https://img.shields.io/github/issues/LilQit7/Adobe_Proxy)](https://github.com/LilQit7/Adobe_Proxy/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/LilQit7/Adobe_Proxy)](https://github.com/LilQit7/Adobe_Proxy/pulls)
[![License](https://img.shields.io/github/license/LilQit7/Adobe_Proxy)](https://github.com/LilQit7/Adobe_Proxy/blob/main/LICENSE)

[![🇺🇸 English](https://img.shields.io/badge/🇺🇸_English-Current-blue)](README_EN.md)
[![🇨🇳 中文](https://img.shields.io/badge/🇨🇳_中文-Available-green)](README.md)

> **⚠️ Disclaimer:**
> 
> This project is for educational and research purposes only. Please comply with relevant laws, regulations, and Adobe software service terms. Users should understand the specific purpose of each domain and assume any consequences that may arise from using this ruleset. The developer does not assume any direct or indirect liability resulting from the use of this project.

## 📖 Project Overview

A professional **Adobe full product line domain proxy ruleset** that provides comprehensive Adobe service domain management solutions for network proxy tools. Through careful organization and classification, it helps users effectively control the network access behavior of Adobe software.

### 🎯 Core Features
- **🔍 Comprehensive Coverage**: Covers all Adobe products and service domains
- **🚀 Plug & Play**: Direct support for mainstream proxy tools
- **⚡ Efficient & Precise**: 290 curated rules, deduplicated and optimized
- **🔄 Continuous Maintenance**: Track Adobe service changes and update timely

## ✨ Feature Matrix

| Feature | Support Status | Description |
|---------|----------------|-------------|
| 🛡️ Activation Blocking | ✅ | Block Adobe software activation verification |
| 📊 Data Analytics Blocking | ✅ | Prevent user behavior data collection |
| 🌐 CDN Control | ✅ | Manage Adobe CDN access |
| 🔐 Security Verification | ✅ | Control software security checks |
| 📍 Geolocation Services | ✅ | Block geolocation-related requests |
| ☁️ Cloud Service APIs | ✅ | Manage Adobe cloud service access |

## 📊 Rule Statistics

<div align="center">

| 📋 Project Info | 📈 Statistics |
|-----------------|---------------|
| **Rule Type** | DOMAIN-SUFFIX |
| **Rule Count** | 290 rules |
| **Last Updated** | 2024-12-19 |
| **Product Coverage** | Adobe Full Suite |
| **Supported Tools** | Clash/Surge/QuantumultX |

</div>

## 🛠️ Quick Start

### 🔧 Clash Configuration

```yaml
rule-providers:
  adobe:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/LilQit7/Adobe_Proxy/main/Adobe.yml"
    path: ./ruleset/adobe.yaml
    interval: 86400

rules:
  - RULE-SET,adobe,REJECT  # Block mode
  # - RULE-SET,adobe,PROXY   # Proxy mode
  # - RULE-SET,adobe,DIRECT  # Direct mode
```

### ⚙️ Surge Configuration

```ini
[Rule]
RULE-SET,https://raw.githubusercontent.com/LilQit7/Adobe_Proxy/main/Adobe.yml,REJECT
```

### 🚀 Quantumult X Configuration

```ini
[filter_remote]
https://raw.githubusercontent.com/LilQit7/Adobe_Proxy/main/Adobe.yml, tag=Adobe Block, force-policy=reject, update-interval=86400, opt-parser=false, enabled=true
```

## 📝 Domain Classification

<details>
<summary>🔍 Click to expand detailed classification</summary>

### 🛡️ Activation & Licensing
```
licenses.adobe.com, activate.adobe.com, genuine.adobe.com
```

### ☁️ Cloud Service APIs
```
Various *.adobe.io domains (e.g., p13n.adobe.io, photos.adobe.io)
```

### 📊 Analytics Services
```
adobe.demdex.net, sstats.adobe.com, adobe.tt.omtrdc.net
```

### 🌐 CDN Domains
```
cc-cdn.adobe.com, assets.adobedtm.com, ssl-delivery.adobe.com
```

### 📍 Geolocation Services
```
geo2.adobe.com, presence-ue1.adobe.com
```

### 🔐 Security Verification
```
auth.services.adobe.com, ims-na1-prprod.adobelogin.com
```

</details>

## 🎛️ Usage Modes

| Use Case | Policy Setting | Application |
|----------|----------------|-------------|
| 🚫 **Complete Block** | `REJECT` | Prevent activation and data collection |
| 🌐 **Proxy Access** | `PROXY` | Access through proxy server |
| ⚡ **Direct Connection** | `DIRECT` | Bypass proxy for direct access |

## ⚠️ Important Reminders

<div align="center">

| ⚠️ Considerations | 📝 Description |
|-------------------|-----------------|
| 🔍 **Understand Purpose** | Ensure understanding of each domain's function before use |
| 🧪 **Test Environment** | Recommended to test rule effects in a testing environment first |
| ⚡ **Software Functionality** | Some rules may affect normal Adobe software functionality |
| 🔄 **Regular Updates** | Check for updates regularly to get the latest rules |

</div>

## 🤝 Contributing

We welcome all forms of contributions!

### 🌟 How to Contribute

1. **🍴 Fork** this project
2. **🌿 Create** a new feature branch
3. **💻 Submit** your changes
4. **📤 Create** a Pull Request

### 💡 Contribution Types

- 🆕 New Adobe domain discoveries
- 🐛 Rule error fixes
- 📚 Documentation improvements
- 🎨 Project optimization suggestions

## 📄 License

This project is licensed under the [MIT License](LICENSE).

## 🔗 Related Resources

| 🛠️ Proxy Tools | 📚 Official Documentation |
|-----------------|---------------------------|
| **Clash** | [GitHub Repository](https://github.com/Dreamacro/clash) |
| **Surge** | [Official Website](https://nssurge.com/) |
| **Quantumult X** | [App Homepage](https://quantumult.app/) |

## ⭐ Star History

If this project helps you, please give it a ⭐ Star!

<div align="center">

[![Star History Chart](https://api.star-history.com/svg?repos=LilQit7/Adobe_Proxy&type=Date)](https://star-history.com/#LilQit7/Adobe_Proxy&Date)

</div>

---

<div align="center">

**💻 Made with ❤️ by [LilQit7](https://github.com/LilQit7)**

**⏰ Last Updated: 2024-12-19**

![Adobe](https://img.shields.io/badge/Adobe-FF0000?style=for-the-badge&logo=adobe&logoColor=white)
![Proxy](https://img.shields.io/badge/Proxy-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![Network](https://img.shields.io/badge/Network-FF6B6B?style=for-the-badge&logo=network&logoColor=white)

</div> 