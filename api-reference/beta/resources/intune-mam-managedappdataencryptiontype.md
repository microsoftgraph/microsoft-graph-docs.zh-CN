---
title: managedAppDataEncryptionType 枚举类型
description: 代表向其应用程序数据进行加密托管应用程序的级别
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 00174e7fba8a8da7490d04815b07a794a966179c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413687"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

代表向其应用程序数据进行加密托管应用程序的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useDeviceSettings|0|应用程序数据进行加密根据设备上的默认设置。|
|afterDeviceRestart|1|应用程序数据进行加密时重新启动设备。|
|whenDeviceLockedExceptOpenFiles|2|与此策略关联的应用程序数据进行加密时设备锁定，除打开的文件中的数据|
|whenDeviceLocked|3|与此策略关联的应用程序数据进行加密时设备锁定|




