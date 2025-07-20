# Adobe_Proxy

**Languages / 语言选择：** [🇺🇸 English](README_EN.md) | [🇨🇳 中文](README.md)

## 📋 项目简介

本项目旨在收集和整合所有Adobe相关的域名规则，为代理工具（如Clash、Surge等）提供完整的Adobe服务域名列表。通过使用本规则集，可以有效管理Adobe软件的网络访问行为。

## 🎯 项目目标

- **域名整合**：将所有Adobe相关域名统一收集整理
- **规则优化**：提供高效的代理规则配置
- **持续更新**：跟进Adobe服务变化，及时更新域名列表
- **兼容性强**：支持主流代理工具的规则格式

## 📊 规则统计

- **规则类型**：DOMAIN-SUFFIX
- **规则数量**：290条
- **最后更新**：2024-12-19
- **覆盖范围**：Adobe全系列产品和服务

## 🛠️ 使用方法

### Clash配置

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

### Surge配置

```
[Rule]
RULE-SET,https://raw.githubusercontent.com/LilQit7/Adobe_Proxy/main/Adobe.yml,PROXY
```

### Quantumult X配置

```
[filter_remote]
https://raw.githubusercontent.com/LilQit7/Adobe_Proxy/main/Adobe.yml, tag=Adobe, force-policy=proxy, update-interval=86400, opt-parser=false, enabled=true
```

## 📝 规则说明

本规则集包含以下Adobe服务域名：

- **激活验证服务**：licenses.adobe.com, activate.adobe.com等
- **云服务接口**：各种*.adobe.io域名
- **CDN加速域名**：cc-cdn.adobe.com等
- **分析统计服务**：adobe.demdex.net等
- **地理位置服务**：geo2.adobe.com等
- **安全验证域名**：genuine.adobe.com等

## 🔧 自定义配置

您可以根据需要调整规则：

1. **阻断模式**：将策略设置为`REJECT`以阻止访问
2. **代理模式**：将策略设置为`PROXY`以通过代理访问
3. **直连模式**：将策略设置为`DIRECT`以直接访问

## ⚠️ 注意事项

- 使用前请确保了解各域名的具体用途
- 某些域名的阻断可能影响Adobe软件正常功能
- 建议在测试环境中先验证规则效果
- 定期检查更新以获取最新的域名列表

## 🤝 贡献指南

欢迎提交新的Adobe域名或改进建议：

1. Fork本项目
2. 创建新的分支
3. 提交您的更改
4. 发起Pull Request

## 📄 许可证

本项目采用MIT许可证，详情请参阅LICENSE文件。

## 🔗 相关链接

- [Clash官方文档](https://github.com/Dreamacro/clash)
- [Surge官方文档](https://nssurge.com/)
- [Quantumult X官方文档](https://quantumult.app/)

---

**最后更新时间：2024-12-19**
