---
title: androidManagedAppSafetyNetDeviceAttestationType 枚举类型
description: 管理员对托管应用强制执行 Android SafetyNet 设备证明要求。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a466567752db4fe880bcb9af72b6be6625d0df4c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075268"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a>androidManagedAppSafetyNetDeviceAttestationType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

管理员对托管应用强制执行 Android SafetyNet 设备证明要求。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|无要求集|
|basicIntegrity|1|要求 Android 设备通过 SafetyNet 基本完整性验证|
|basicIntegrityAndDeviceCertification|2|要求 Android 设备通过 SafetyNet 基本完整性和设备认证验证|



