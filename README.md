# Web Security Writeups

> 本仓库收录了我在学习 Web 安全过程中的实验报告与漏洞复现记录，涵盖 OWASP Top 10 核心漏洞类型。

**在线浏览**：https://github.com/m0N1sey/Web-Security-Writeups

---

##  仓库简介

从零开始，系统性地复现了 SQLi-Labs、DVWA、Upload-Labs、Pikachu、WebGoat、PortSwigger 等多个靶场的漏洞实例。每份报告均包含：

-  **漏洞原理**：通俗解释漏洞产生的根本原因
-  **复现步骤**：完整的操作流程与 Payload
-  **防御方案**：对应漏洞的修复建议与代码示例
-  **过程截图**：关键步骤可视化记录

---

##  报告索引

### SQLi-Labs（SQL 注入系列）

| 实验 | 漏洞类型 | 报告 |
|------|---------|------|
| Less-1 | 字符型联合查询注入 | [📄 查看](./reports/sqli-labs/Less-1_字符型联合查询注入.md) |
| Less-5 | 报错注入（无回显） | [📄 查看](./reports/sqli-labs/Less-5_报错注入.md) |
| Less-8 | 布尔盲注 | [📄 查看](./reports/sqli-labs/Less-8_布尔盲注.md) |

### XSS（跨站脚本攻击）

| 实验 | 漏洞类型 | 报告 |
|------|---------|------|
| DVWA + PortSwigger | 反射型 / 存储型 / DOM 型 | [📄 查看](./reports/xss/XSS跨站脚本攻击全类型实验报告.md) |

### 文件上传漏洞

| 实验 | 漏洞类型 | 报告 |
|------|---------|------|
| Upload-Labs Pass-01 ~ 06 | 前端绕过 / MIME 绕过 / .htaccess / 大小写 / 点空点 | [📄 查看](./reports/file-upload/文件上传漏洞实验报告.md) |

### 文件包含漏洞（LFI / RFI）

| 实验 | 漏洞类型 | 报告 |
|------|---------|------|
| DVWA File Inclusion | 本地文件包含 / 远程文件包含 / 日志注入 / 伪协议 | [📄 查看](./reports/lfi-rfi/文件包含漏洞实验报告.md) |

### 命令注入

| 实验 | 漏洞类型 | 报告 |
|------|---------|------|
| DVWA Command Injection | 连接符注入 / str_replace 顺序绕过 | [📄 查看](./reports/cmd-injection/命令注入实验报告.md) |

### CSRF（跨站请求伪造）

| 实验 | 漏洞类型 | 报告 |
|------|---------|------|
| DVWA CSRF | GET 请求劫持 / Referer 绕过 / data:URL | [📄 查看](./reports/csrf/CSRF跨站请求伪造实验报告.md) |

### 失效的访问控制

| 实验 | 漏洞类型 | 报告 |
|------|---------|------|
| WebGoat Broken Access Control | IDOR 越权 / 垂直越权 / 会话劫持 / Cookie 伪造 | [📄 查看](./reports/broken-access-control/失效的访问控制实验报告.md) |

### 业务逻辑漏洞

| 实验 | 漏洞类型 | 报告 |
|------|---------|------|
| 自建环境 + Pikachu | 支付逻辑篡改 / 优惠券复用 / 验证码绕过 | [📄 查看](./reports/business-logic/业务逻辑漏洞实验报告.md) |

---

## 🛠️ 技术栈与工具

| 类别 | 工具 / 技术 |
|------|-------------|
| 靶场环境 | SQLi-Labs、DVWA、Upload-Labs、Pikachu、WebGoat、PortSwigger |
| 代理工具 | Burp Suite（Proxy / Repeater / Intruder / Decoder） |
| 本地环境 | PHPStudy（Apache + MySQL + PHP）、Kali Linux |
| 编程语言 | PHP、Python、JavaScript（用于构造 Payload） |
| 版本控制 | Git + GitHub |

---

## 📝 学习路线

```
基础靶场（SQLi-Labs / DVWA）
        ↓
文件上传 / 命令注入 / XSS / CSRF
        ↓
文件包含 / 越权访问
        ↓
业务逻辑漏洞 / 验证码绕过
        ↓
综合靶场（WebGoat / PortSwigger）
```

---

##  许可证

[MIT License](./LICENSE)

---

## 🙋 关于作者

安全初学者，正在 Web 安全与渗透测试方向不断学习中。

- GitHub：[m0N1sey](https://github.com/m0N1sey)
- 持续更新中...

---

> ⭐ 如果这个仓库对你有帮助，欢迎 Star 支持一下！