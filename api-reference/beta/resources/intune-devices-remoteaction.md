---
title: remoteAction 枚举类型
description: 远程操作 Intune 支持。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58561626423046abe9e0d8832c82c714519ea46f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963868"
---
# <a name="remoteaction-enum-type"></a>remoteAction 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

远程操作 Intune 支持。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|用户启动未知操作。|
|factoryReset|1|用户启动一个操作以出厂重置设备。 |
|removeCompanyData|双面|用户启动一个操作, 以从设备中删除公司数据。 |
|resetPasscode|第三章|用户启动一个操作以删除 iOS 设备的密码, 或重置 Android/Windows 设备的密码。 |
|remoteLock|4|用户启动一个操作, 以远程锁定设备。|
|enableLostMode|5|用户启动一个操作, 以在受监督的 iOS 设备上启用丢失模式。|
|disableLostMode|型|用户启动一个操作, 以在受监督的 iOS 设备上禁用丢失模式。|
|locateDevice|步|用户启动操作以查找受监督的 iOS 设备。|
|rebootNow|utf-8|用户启动操作以重新启动 Windows 设备。|
|recoverPasscode|第|用户启动一个操作以重置用于 windows phone 设备上的 passport 的 pin 以供工作。|
|cleanWindowsDevice|10 |用户启动操作以清理 windows 设备。|
|logoutSharedAppleDeviceActiveUser|11x17|用户启动一个操作以注销共享 apple 设备上的当前用户。|
|quickScan|12|用户启动操作以在设备上运行快速扫描。|
|fullScan|13|用户启动操作以在设备上运行完全扫描。|
|windowsDefenderUpdateSignatures|日|用户启动操作以更新设备上的恶意软件签名。|
|factoryResetKeepEnrollmentData|个|用户使用保留注册数据的远程擦除设备启动操作。|
|updateDeviceAccount|位|用户启动操作以更新设备上的帐户。|
|automaticRedeployment|×|用户启动操作以 automatice 重新部署设备|
|关闭|18|用户启动一种关闭设备的操作。|
|rotateFileVaultKey|20|用户启动一个操作以在 mac 上旋转 FileVaultKey。|
|getFileVaultKey|不足|用户启动一个操作以在 mac 上获取 FileVaultKey。|





