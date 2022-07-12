---
title: managedAppDataEncryptionType 枚举类型
description: 表示为托管应用加密应用数据的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d7480b7db8a28ef36a2ec0402de5024790881da
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734674"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示为托管应用加密应用数据的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useDeviceSettings|0|应用数据基于设备上的默认设置进行加密。|
|afterDeviceRestart|1|重启设备时，将加密应用数据。|
|whenDeviceLockedExceptOpenFiles|2|锁定设备时，将加密与此策略关联的应用数据，打开的文件中的数据除外|
|whenDeviceLocked|3|锁定设备时，将加密与此策略关联的应用数据|





