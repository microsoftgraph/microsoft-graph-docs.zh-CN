---
title: managedAppDataEncryptionType 枚举类型
description: 表示为托管应用程序加密应用程序数据的级别
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b3e2cc44e1d548a1abe2a4d34c02fef9db7750a1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356385"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 枚举类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示为托管应用程序加密应用程序数据的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useDeviceSettings|0|应用程序数据根据设备上的默认设置进行加密。|
|afterDeviceRestart|1|重新启动设备时对应用数据进行加密。|
|whenDeviceLockedExceptOpenFiles|双面|设备锁定时，与此策略关联的应用数据将被加密，但打开的文件中的数据除外|
|whenDeviceLocked|第三章|设备锁定时，与此策略关联的应用数据将被加密|




