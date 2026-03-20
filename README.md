# 🛡️ APT Tools - 高级持续性威胁工具箱

![Badge](https://img.shields.io/badge/Language-Python-blue)
![Badge](https://img.shields.io/badge/License-MIT-green)
![Badge](https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20macOS-brightgreen)
![Badge](https://img.shields.io/badge/Status-Active-brightgreen)

一个功能强大的现代化 **APT（高级持续性威胁）工具集成平台**，集成了业界领先的安全工具与渗透测试框架。提供 Web 界面和桌面 GUI 两种使用方式，支持工具管理、参数配置和实时执行。

> ⚠️ **免责声明**: 本工具仅供在获得授权的测试环境中进行合法安全研究和渗透测试。未经授权对他人系统的任何操作都是违法的。使用者应自行承担所有法律责任。

> ⚠️ **注意**：本工具箱含有部分专业工具，请务必查看文档使用，或购买同步课程《APT单兵作战指南》了解使用。

---

## ✨ 核心特性

- 📊 **统一管理界面** - 集中管理 70+ 个安全工具，按功能分类组织
- 🎨 **现代化 UI** - 响应式设计，支持亮暗主题切换
- ⚡ **实时执行** - Web 界面和 PyQt6 桌面应用，实时显示命令输出
- 🔧 **灵活配置** - 支持工具参数自定义，命令模板替换
- 💾 **持久化存储** - 自动保存用户配置和默认参数
- 🌐 **双界面** - Flask Web 版本 + PyQt6 本地应用选择
- 🔒 **安全设计** - 默认仅允许本地访问，支持命令限制

---

## 📦 工具分类概览

### 1️⃣ **信息收集** | info-gathering
收集目标系统、网络和应用的各种信息

| 工具 | 功能描述 |
|------|--------|
| **Maltego** | 功能强大的开源情报（OSINT）工具，支持数据挖掘和关联分析 |
| **reNgine** | Web 应用自动化侦察框架，构建完整的攻击面 |
| **amass** | 深入的攻击面映射和资产发现工具 |
| **OpenDoor** | OWASP Web 目录扫描器 |
| **Shadowbroker** | 全球开源情报集合，追踪重要事件和资产 |
| **SpiderFoot** | 自动执行 OSINT 威胁情报收集 |

### 2️⃣ **漏洞扫描** | vuln-scan
自动化漏洞检测与评估

| 工具 | 功能描述 |
|------|--------|
| **Nuclei** | 快速可定制的漏洞扫描器，支持 YAML DSL 规则 |
| **ZAP** | OWASP Zed Attack Proxy，全球最广泛使用的 Web 扫描器 |

### 3️⃣ **漏洞利用** | exploitation
漏洞防御绕过与利用工具

| 工具 | 功能描述 |
|------|--------|
| **PayloadsAllTheThings** | Web 攻击有效载荷库和绕过方法集合 |
| **XSS-Payloads** | XSS 跨站脚本攻击有效载荷库 |
| **phpggc** | PHP 反序列化漏洞利用工具 |
| **SSTImap** | 服务器端模板注入（SSTI）检测和利用 |
| **Web-Cache-Vulnerability-Scanner** | Web 缓存中毒漏洞检测 |
| **hetty** | HTTP 安全研究工具包 |

### 4️⃣ **权限提升** | priv-esc
本地权限提升工具与技巧

#### Windows
| 工具 | 功能描述 |
|------|--------|
| **winPEAS** | Windows 权限提升枚举工具 |
| **JuicyPotato** | Windows Token 劫持权限提升 |
| **SpoolFool** | CVE-2022-21999 打印后台处理程序漏洞利用 |
| **accesschk** | Windows 权限检查工具 |

#### Linux
| 工具 | 功能描述 |
|------|--------|
| **LinPEAS** | Linux 权限提升路径枚举 |
| **linux-exploit-suggester** | Linux 漏洞建议工具 |
| **linux-smart-enumeration** | 系统安全信息收集 |

### 5️⃣ **C2 通信** | c2
命令与控制框架

| 工具 | 功能描述 |
|------|--------|
| **Cobalt Strike** | 专业 C2 框架（v4.9.1） |
| **BruteRatel** | 轻量级 C2 框架（v1.4.5） |
| **PoshC2** | PowerShell 驱动的 C2 框架 |
| **Quasar** | 开源 C2 框架 |
| **pupy** | Python 编写的 C2 框架 |

### 6️⃣ **域名/Active Directory** | domain
域环境信息收集与攻击

| 工具 | 功能描述 |
|------|--------|
| **SharpHound** | Active Directory 环境映射工具 |
| **Rubeus** | Kerberos 票证操纵工具 |
| **adPEAS** | AD 权限提升枚举脚本 |
| **Certify** | 活目录证书滥用检测 |
| **Whisker** | 证书操纵工具 |

### 7️⃣ **钓鱼与社工** | Fhish
社会工程学与钓鱼工具

| 工具 | 功能描述 |
|------|--------|
| **GoPhish** | 开源钓鱼框架 |
| **SharpLocker** | Windows 登录屏幕浏览器 |
| **HtmlSmuggling** | HTML 隐写技术 |
| **Real-Time-Voice-Cloning** | 实时语音克隆 |

### 8️⃣ **横向移动** | lateral-movement
网络内部横向移动工具

| 工具 | 功能描述 |
|------|--------|
| **mimikatz** | Windows 凭证提取工具 |
| **nxc** | NetExec，网络协议利用框架 |
| **PSTools** | Windows 远程执行工具集 |
| **ruler** | Exchange 邮件服务器攻击工具 |
| **SharpDPAPI** | Windows DPAPI 操纵工具 |

### 9️⃣ **持久化** | Persistence
后门持久化与隐蔽执行

| 工具 | 功能描述 |
|------|--------|
| **PowerSploit** | PowerShell 渗透测试框架 |
| **Diamorphine** | Linux 内核隐蔽后门 |
| **KoviD** | Linux 提权与隐蔽工具 |
| **TitanHide** | 进程隐蔽工具 |

### 🔟 **云安全** | Cloud
云环境安全工具

| 工具 | 功能描述 |
|------|--------|
| **cloud-enum** | 云平台账户枚举工具 |
| **cloudfox** | AWS、Azure 安全配置审计 |
| **GhostLeak** | 云环境敏感数据泄露检测 |

### 1️⃣1️⃣ **人工智能攻击** | ai
AI/ML 相关的安全工具

| 工具 | 功能描述 |
|------|--------|
| **TextAttack** | 文本对抗性攻击工具 |
| **PyRIT** | AI 安全评估框架 |
| **promptfoo** | LLM 提示词注入测试 |

### 1️⃣2️⃣ **Web Shell** & 其他
| 工具 | 功能描述 |
|------|--------|
| **Web Shell** | Web 服务器后门集合 |
| **Block Chain** | 区块链安全工具 |

---

## 🚀 快速开始

### 前置要求
- Windows 11

### 下载地址



### 使用方式

#### 方式 1: Web 界面
```bash
web.exe
```
打开浏览器访问 `http://localhost:5000`

**特性：**
- 精美的 Web 界面
- 支持浏览器访问
- 实时命令预览和参数配置
- 主题切换（亮/暗）

#### 方式 2: 桌面应用（推荐）
```bash
APT_Tools.exe
```

**特性：**
- 原生桌面应用
- 更好的系统集成
- 实时输出流
- 系统托盘支持

---

## 📖 详细使用指南

### 工具执行流程

1. **工具选择** - 从左侧分类菜单选择工具
2. **参数配置** - 在工具详情页输入必要参数
3. **命令预览** - 查看将要执行的完整命令
4. **启用/禁用自定义命令**
   - 禁用（默认）：使用预定义命令模板
   - 启用：可直接编辑命令后执行
5. **执行** - 点击"运行工具"按钮
6. **查看结果** - 实时显示命令输出

### 自定义工具配置

编辑 `data/tools.json` 添加新工具：
```json
{
  "id": "my-tool-id",
  "name": "我的工具",
  "description": "工具描述",
  "path": "tools/path/to/tool",
  "start": {
    "mode": "command",
    "cmd": "my-command {param1} {param2}"
  }
}
```

---

## 🔐 安全性说明

### ⚠️ 重要安全警告

1. **仅本地访问** - 默认只允许 127.0.0.1 和 ::1 访问
2. **不要暴露到网络** - 不要在不受信任的网络上暴露该服务
3. **权限管理** - 运行该工具的用户拥有执行任意命令的能力
4. **命令注入风险** - 启用自定义命令功能时需谨慎

---

## 📝 许可证

MIT License - 详见 [LICENSE](LICENSE) 文件

---

## 📧 联系与支持

- 📌 **问题报告**: [GitHub Issues](https://github.com/GhostWolfLab/APT_Tools/issues)
- 💬 **QQ群**: 816112115

---

## 📜 更新日志

### v1.0.0 (2026-03-20)
- ✨ 初始版本发布
- ✅ 70+ 工具集成
- ✅ Web 和 PyQt6 双界面
- ✅ 实时命令执行

---

<div align="center">

**⭐ 如果这个项目对你有帮助，请给个 Star ⭐**

Made with ❤️ by Security Researchers

![GitHub stars](https://img.shields.io/github/stars/GhostWolfLab/APT_Tools?style=social)
![GitHub forks](https://img.shields.io/github/forks/GhostWolfLab/APT_Tools?style=social)

</div>
