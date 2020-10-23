---
title: managedAppDataEncryptionType 枚举类型
description: 表示为托管应用程序加密应用程序数据的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e57afb0a878248e761d11434825f1d0c9403a6c5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684622"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示为托管应用程序加密应用程序数据的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useDeviceSettings|0|应用程序数据根据设备上的默认设置进行加密。|
|afterDeviceRestart|1|重新启动设备时对应用数据进行加密。|
|whenDeviceLockedExceptOpenFiles|双面|设备锁定时，与此策略关联的应用数据将被加密，但打开的文件中的数据除外|
|whenDeviceLocked|第三章|设备锁定时，与此策略关联的应用数据将被加密|





