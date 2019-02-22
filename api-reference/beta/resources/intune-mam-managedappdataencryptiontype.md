---
title: managedAppDataEncryptionType 枚举类型
description: 表示为托管应用程序加密应用程序数据的级别
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47396f32ed23234c5fe758a29b6e97ee3602234f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159078"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示为托管应用程序加密应用程序数据的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useDeviceSettings|0|应用程序数据根据设备上的默认设置进行加密。|
|afterDeviceRestart|1|重新启动设备时对应用数据进行加密。|
|whenDeviceLockedExceptOpenFiles|双面|设备锁定时, 与此策略关联的应用数据将被加密, 但打开的文件中的数据除外|
|whenDeviceLocked|第三章|设备锁定时, 与此策略关联的应用数据将被加密|




