---
title: managedAppFlaggedReason 枚举类型
description: 用户已被标记的原因
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 64f78ca8a074d35687f50e232a104b87717a6462
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527919"
---
# <a name="managedappflaggedreason-enum-type"></a>managedAppFlaggedReason 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用户已被标记的原因

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无问题。|
|rootedDevice|1 |应用注册在根/解锁设备上运行。|
|androidBootloaderUnlocked|2 |应用注册在解锁了启用程序的 Android 设备上运行。|
|androidFactoryRomModified|3 |应用注册在已修改出厂 ROM 的 Android 设备上运行。|



