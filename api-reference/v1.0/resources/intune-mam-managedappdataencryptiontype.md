---
title: managedAppDataEncryptionType 枚举类型
description: 表示为托管应用程序加密应用程序数据的级别
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c2a4c9b713d2b91645cf210df60ec8d3ba642a20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533344"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示为托管应用程序加密应用程序数据的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useDeviceSettings|0|应用程序数据根据设备上的默认设置进行加密。|
|afterDeviceRestart|1 |重新启动设备时对应用数据进行加密。|
|whenDeviceLockedExceptOpenFiles|2 |设备锁定时，与此策略关联的应用数据将被加密，但打开的文件中的数据除外|
|whenDeviceLocked|3 |设备锁定时，与此策略关联的应用数据将被加密|




