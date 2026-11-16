# 隐私政策 / Privacy Policy

**生效日期 / Effective Date:** 2026-11-14  
**应用名称 / Application:** 右键菜单管理器 / Context Menu Manager Neo (CMMN)  

---

## 简体中文 (Chinese Simplified)

### 1. 概述
**右键菜单管理器 (Context Menu Manager Neo / CMMN)**（以下简称“本应用”）是一款运行于 Windows 操作系统的纯本地桌面系统工具，用于查看、管理、备份与诊断 Windows 资源管理器（Explorer）右键关联菜单项。

我们高度重视您的隐私。**本应用完全在您的本地设备上离线运行，不收集、不存储、不上传、不共享任何个人身份信息（PII）或设备遥测数据。**

### 2. 信息收集与网络使用
- **零数据收集**：本应用不包含任何数据统计分析 SDK（Analytics）、崩溃遥测上报组件或广告追踪器。
- **零网络访问**：本应用不发起任何互联网连接，在 MSIX 安装包清单中亦未声明 `internetClient` 等任何网络权限。

### 3. 本地数据处理与存储
为了实现右键菜单的管理、配置与备份恢复功能，本应用产生和处理的所有数据均严格保存在您的本地计算机上。

### 4. 系统权限声明
本应用在 Windows 系统中声明了以下权限，全部仅用于实现本地功能：
- **`runFullTrust` 与 `unvirtualizedResources`**：用于直接读取和管理 Windows 资源管理器真实的右键菜单注册表项，并启动独立的 COM 沙箱分析探测子进程（`Prober.exe`）。
- **`allowElevation`（管理员提权）**：当您需要修改系统级（`HKEY_LOCAL_MACHINE`）右键菜单项时，后台伴侣进程（`Backend.exe`）需通过 Windows 标准 UAC 弹窗向您请求管理员权限。

### 5. 第三方共享
由于本应用不收集任何数据且不具备联网功能，您的任何信息均绝不会被出售、传输或共享给开发者或任何第三方。

### 6. 数据保留与清除
本应用创建的所有数据均保存在您的本地设备上，完全受您的控制。您可以随时通过以下方式彻底清除本地数据：
- 在 Windows“设置 -> 应用 -> 已安装的应用”中卸载本应用；
- 以及/或者手动删除本地目录 `%LocalAppData%\CMMN`（便携模式下直接删除程序所在文件夹）及注册表项 `HKEY_CURRENT_USER\Software\CMMN`。

### 7. 政策变更与联系方式
如本隐私政策发生变更，我们将在此页面发布修订版本并更新上方的生效日期。  
如果您对本隐私政策有任何疑问，请通过本项目的 GitHub Issues 页面或微软应用商店页面列出的技术支持邮箱与我们取得联系。

---

## English

### 1. Overview
**Context Menu Manager Neo (CMMN)** ("the Application") is a standalone, local Windows desktop utility designed to inspect, manage, back up, and diagnose Windows Explorer context menu registrations.

We take your privacy seriously. **The Application operates 100% offline on your local device. It does not collect, transmit, store on external servers, or share any personal data, personal identifiable information (PII), or telemetry.**

### 2. Data Collection and Network Usage
- **No Data Collection**: The Application contains no analytics SDKs, no telemetry reporters, no crash uploaders, and no advertising or tracking modules.
- **No Internet Access**: The Application makes zero network connections and does not request the `internetClient` capability in its MSIX package manifest.

### 3. Local Data Processing and Storage
To provide context menu management and backup/restore functionality, the Application processes and stores data strictly on your local computer.

### 4. System Permissions Disclosure
The Application declares the following Windows desktop capabilities solely for local functionality:
- **`runFullTrust` & `unvirtualizedResources`**: Required to read and manage real Windows Shell context menu registry keys and to launch the isolated COM sandbox prober (`Prober.exe`).
- **`allowElevation`**: Required so the companion backend process (`Backend.exe`) can request standard Windows UAC elevation when you choose to modify system-wide (`HKEY_LOCAL_MACHINE`) context menu entries.

### 5. Third-Party Sharing
Because the Application collects no information and has no network functionality, no data is ever sold, transferred, or shared with the developer or any third party.

### 6. Data Retention and Deletion
All data created by the Application resides on your local device under your full control. You can remove all local settings and backups at any time by:
- Uninstalling the Application via **Windows Settings -> Apps -> Installed apps**; and/or
- Deleting the `%LocalAppData%\CMMN` directory (or the application folder in Portable Mode) and the `HKEY_CURRENT_USER\Software\CMMN` registry key.

### 7. Changes and Contact Us
If we update this Privacy Policy, we will post the revised version on this page and update the Effective Date above.  
If you have any questions about this Privacy Policy, please contact us via the project's repository Issues page or the publisher support email listed on the Microsoft Store page.
