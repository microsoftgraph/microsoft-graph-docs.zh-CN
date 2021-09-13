---
title: remoteAction 枚举类型
description: Intune 支持的远程操作。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 70e7d5ac0734f791f79915524565012393b6f90d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59081085"
---
# <a name="remoteaction-enum-type"></a>remoteAction 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Intune 支持的远程操作。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|用户启动未知操作。|
|factoryReset|1|用户启动操作以恢复设备出厂设置。 |
|removeCompanyData|2|用户启动操作以从设备中删除公司数据。 |
|resetPasscode|3|用户启动删除 iOS 设备密码的操作，或重置 Android/Windows密码。 |
|remoteLock|4 |用户启动远程锁定设备的操作。|
|enableLostMode|5 |用户启动操作以在受监督的 iOS 设备上启用丢失模式。|
|disableLostMode|6 |用户启动操作以在受监督的 iOS 设备上禁用丢失模式。|
|locateDevice|7 |用户启动操作以查找受监督的 iOS 设备。|
|rebootNow|8 |用户启动操作以重新启动Windows设备。|
|recoverPasscode|9 |用户启动操作以重置 Passport 的 pin，以在 Windows Phone 设备上工作。|
|cleanWindowsDevice|10 |用户启动清理 Windows 设备的操作。|
|logoutSharedAppleDeviceActiveUser|11|用户启动操作以注销共享 Apple 设备上当前用户。|
|quickScan|12 |用户启动操作以在设备上运行快速扫描。|
|fullScan|13|用户启动操作以在设备上运行完全扫描。|
|windowsDefenderUpdateSignatures|14 |用户启动操作以更新设备上恶意软件签名。|
|factoryResetKeepEnrollmentData|15 |用户通过保留注册数据启动远程擦除设备操作。|
|updateDeviceAccount|16 |用户启动操作以更新设备上的帐户。|
|automaticRedeployment|17 |用户启动操作以自动重新部署设备|
|shutDown|18 |用户启动操作以关闭设备。|
|rotateBitLockerKeys|19|用户启动在设备上旋转 BitLockerKeys 的操作。|
|rotateFileVaultKey|20|用户启动在 mac 上旋转 FileVaultKey 的操作。|
|getFileVaultKey| 21|用户启动在 mac 上获取 FileVaultKey 的操作。|
|setDeviceName|22|用户启动在设备上设置设备名称的操作。|
|activateDeviceEsim|23|用户启动在设备上激活 eSIM 的操作。|



