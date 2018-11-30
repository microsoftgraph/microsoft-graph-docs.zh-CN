---
title: managedAppDataEncryptionType 枚举类型
description: 代表向其应用程序数据进行加密托管应用程序的级别
ms.openlocfilehash: 7efda037bc2b4d5794c575823845c0955be46477
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010461"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

代表向其应用程序数据进行加密托管应用程序的级别
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useDeviceSettings|0|应用程序数据进行加密根据设备上的默认设置。|
|afterDeviceRestart|1|应用程序数据进行加密时重新启动设备。|
|whenDeviceLockedExceptOpenFiles|2|与此策略关联的应用程序数据进行加密时设备锁定，除打开的文件中的数据|
|whenDeviceLocked|3|与此策略关联的应用程序数据进行加密时设备锁定|



