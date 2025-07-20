# Adobe_Proxy

**Languages / 语言选择：** [🇺🇸 English](README_EN.md) | [🇨🇳 中文](README.md)

## 📋 Project Overview

This project aims to collect and integrate all Adobe-related domain rules, providing a comprehensive Adobe service domain list for proxy tools (such as Clash, Surge, etc.). By using this ruleset, you can effectively manage the network access behavior of Adobe software.

## 🎯 Project Goals

- **Domain Integration**: Unified collection and organization of all Adobe-related domains
- **Rule Optimization**: Provide efficient proxy rule configurations
- **Continuous Updates**: Keep up with Adobe service changes and update domain lists timely
- **Strong Compatibility**: Support mainstream proxy tool rule formats

## 📊 Rule Statistics

- **Rule Type**: DOMAIN-SUFFIX
- **Rule Count**: 290 rules
- **Last Updated**: 2024-12-19
- **Coverage**: Adobe full product suite and services

## 🛠️ Usage

### Clash Configuration

```yaml
rule-providers:
  adobe:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/LilQit7/Adobe_Proxy/main/Adobe.yml"
    path: ./ruleset/adobe.yaml
    interval: 86400

rules:
  - RULE-SET,adobe,PROXY
```

### Surge Configuration

```
[Rule]
RULE-SET,https://raw.githubusercontent.com/LilQit7/Adobe_Proxy/main/Adobe.yml,PROXY
```

### Quantumult X Configuration

```
[filter_remote]
https://raw.githubusercontent.com/LilQit7/Adobe_Proxy/main/Adobe.yml, tag=Adobe, force-policy=proxy, update-interval=86400, opt-parser=false, enabled=true
```

## 📝 Rule Description

This ruleset contains the following Adobe service domains:

- **Activation & Licensing**: licenses.adobe.com, activate.adobe.com, etc.
- **Cloud Service APIs**: Various *.adobe.io domains
- **CDN Domains**: cc-cdn.adobe.com, etc.
- **Analytics Services**: adobe.demdex.net, etc.
- **Geolocation Services**: geo2.adobe.com, etc.
- **Security Verification**: genuine.adobe.com, etc.

## 🔧 Custom Configuration

You can adjust the rules according to your needs:

1. **Block Mode**: Set policy to `REJECT` to block access
2. **Proxy Mode**: Set policy to `PROXY` to access through proxy
3. **Direct Mode**: Set policy to `DIRECT` for direct access

## ⚠️ Important Notes

- Please ensure you understand the specific purpose of each domain before use
- Blocking certain domains may affect normal Adobe software functionality
- It is recommended to test the rule effects in a test environment first
- Check for updates regularly to get the latest domain list

## 🤝 Contributing

Welcome to submit new Adobe domains or improvement suggestions:

1. Fork this project
2. Create a new branch
3. Submit your changes
4. Create a Pull Request

## 📄 License

This project is licensed under the MIT License. See the LICENSE file for details.

## 🔗 Related Links

- [Clash Official Documentation](https://github.com/Dreamacro/clash)
- [Surge Official Documentation](https://nssurge.com/)
- [Quantumult X Official Documentation](https://quantumult.app/)

---

**Last Updated: 2024-12-19** 