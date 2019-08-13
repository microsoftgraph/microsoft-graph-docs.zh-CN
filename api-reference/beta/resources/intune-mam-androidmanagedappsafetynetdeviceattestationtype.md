---
title: androidManagedAppSafetyNetDeviceAttestationType 枚举类型
description: 管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: eb21ce8d54b006db4e98828eb7c8240dd2810b14
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332321"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a>androidManagedAppSafetyNetDeviceAttestationType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理员在托管应用上强制实施了 Android SafetyNet 设备证明要求。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无要求集|
|basicIntegrity|1|要求 Android 设备通过 SafetyNet 基本完整性验证|
|basicIntegrityAndDeviceCertification|双面|要求 Android 设备传递 SafetyNet 基本完整性和设备认证验证|



