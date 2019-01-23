---
title: remoteAction 枚举类型
description: 远程操作 Intune 支持。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3177ea43599cd155e11af1786636111a8578d29b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405539"
---
# <a name="remoteaction-enum-type"></a>remoteAction 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

远程操作 Intune 支持。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|用户启动未知的操作。|
|factoryReset|1|用户启动某项操作到中心重置设备。 |
|removeCompanyData|2|用户启动要从设备中删除公司数据的操作。 |
|resetPasscode|3|用户启动某项操作删除 iOS 设备密码或重置密码的 Android / Windows 设备。 |
|remoteLock|4|用户启动远程锁定操作设备。|
|enableLostMode|5|用户启动某项操作来启用监管的 iOS 设备上丢失的模式。|
|disableLostMode|6|用户启动某项操作来禁用监管的 iOS 设备上丢失的模式。|
|locateDevice|7|用户启动某项操作来查找监管的 iOS 设备。|
|rebootNow|8|用户启动某项操作可重新启动 Windows 设备。|
|recoverPasscode|9|用户启动操作以重置 passport 用于在 windows phone 设备上的 pin。|
|cleanWindowsDevice|10|用户启动 windows 设备清理操作。|
|logoutSharedAppleDeviceActiveUser|11|用户启动要注销共享的 apple 设备上的当前用户的操作。|
|quickScan|12|用户启动操作以在设备上运行快速扫描。|
|fullScan|13|用户启动操作以在设备上运行完全扫描。|
|windowsDefenderUpdateSignatures|14|用户启动某项操作来更新设备上的恶意软件签名。|
|factoryResetKeepEnrollmentData|15|用户启动确保注册数据操作远程擦除设备。|
|updateDeviceAccount|16|用户启动某项操作来更新设备上的帐户。|
|automaticRedeployment|17|用户启动 automatice 重新部署设备操作|
|关闭|18|用户启动要关闭设备的操作。|




