---
title: managedAppDataEncryptionType 枚举类型
description: 代表向其应用程序数据进行加密托管应用程序的级别
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 08ac7a36e142a1d19dbaaeb0263ef095072a9e01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956813"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

代表向其应用程序数据进行加密托管应用程序的级别
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|useDeviceSettings|0|应用程序数据进行加密根据设备上的默认设置。|
|afterDeviceRestart|1|应用程序数据进行加密时重新启动设备。|
|whenDeviceLockedExceptOpenFiles|2|与此策略关联的应用程序数据进行加密时设备锁定，除打开的文件中的数据|
|whenDeviceLocked|3|与此策略关联的应用程序数据进行加密时设备锁定|



