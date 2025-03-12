# 搬瓦工重装系统及修改 Root 密码完整教程

搬瓦工是一款性价比很高的 VPS 产品，不仅可以用来搭建网站，还能用作其他用途。为了防止忘记相关操作，这里整理了一份详细教程分享给大家，帮助您快速掌握重置系统或者修改 Root 密码的方法。

---

## 一、第一次使用搬瓦工时重装系统教程

当您第一次购买搬瓦工 VPS 后，需要重新安装系统以完成基础配置操作。以下是完整步骤：

1. **登录 KiwiVM 控制面板**  
   在购买完成后，进入搬瓦工官网，点击 `Services → My Services → KiwiVM Control Panel`。  

   👉 [【建议收藏】2025年搬瓦工最新优惠套餐整理汇总 - 每日更新最新可用优惠码](https://bit.ly/banwagon)

2. **停止 VPS 服务**  
   进入控制面板页面后，点击 `Stop` 按钮停止当前运行的 VPS 服务。如果不执行此操作，将无法开始系统重装。  

3. **安装新系统**  
   在面板中找到 `Install new OS`，选择一个较新的 CentOS 系统版本（例如 CentOS 7），推荐选择带有 `bbr` 的版本，以提升网络性能。同时勾选 `I agree` 后点击 `Reload`，开始重装系统。  

4. **记录 SSH 信息**  
   系统重装完成后，会生成新的 SSH 端口和 Root 密码，这些信息用于后续远程登录 VPS，请务必妥善保存。

完成以上步骤后，您可以根据需要开始搭建网站或配置其他功能。

---

## 二、重置或修改 Root 密码的操作指南

如果您的 VPS 已经安装了系统，但忘记了 Root 密码，则可以通过以下方法进行重置。

### 1. 停止 VPS 服务
进入 KiwiVM 控制面板。如果 VPS 正在运行状态，直接修改 Root 密码会提示失败：

> Failed to reset root password (739102)  
> Additional information: 992800002 VPS is currently running. Please stop the VPS before attempting to modify root password.

点击面板首页的 `Stop` 按钮关闭 VPS 服务后再继续操作。

### 2. 进入密码修改菜单
在 KiwiVM 面板左侧，点击 `Root password modification` 菜单项。

### 3. 生成新密码
在重置密码界面，点击 `Generate and set new root password` 按钮。系统会自动生成一组新的 Root 密码。

### 4. 保存新密码
生成后的 Root 密码会显示在新页面中，请妥善保存，后续登录 VPS 将需要使用该密码。

---

完成以上操作后，无论是重装系统还是重置密码，您都可以方便快捷地继续使用搬瓦工 VPS 进行各种配置。