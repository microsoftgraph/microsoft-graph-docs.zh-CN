---
title: androidManagedAppSafetyNetDeviceAttestationType 枚举类型
description: 管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 285389d07f4ea6f667a0e12260fe5a5296808923
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524362"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a>androidManagedAppSafetyNetDeviceAttestationType 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无要求集|
|basicIntegrity|1 |要求 Android 设备通过 SafetyNet 基本完整性验证|
|basicIntegrityAndDeviceCertification|2 |要求 Android 设备传递 SafetyNet 基本完整性和设备认证验证|



