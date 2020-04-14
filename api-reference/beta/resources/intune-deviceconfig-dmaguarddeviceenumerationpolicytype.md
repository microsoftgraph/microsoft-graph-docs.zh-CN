---
title: dmaGuardDeviceEnumerationPolicyType 枚举类型
description: DmaGuardDeviceEnumerationPolicy 的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f735a5ce77c0162899d7e93974a07de4f0be137b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469161"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>dmaGuardDeviceEnumerationPolicyType 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DmaGuardDeviceEnumerationPolicy 的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|默认值。 具有 DMA 重新映射的设备将仅在用户解锁屏幕后枚举不兼容驱动程序。|
|blockAll|1|具有 DMA 重新映射的设备不支持的驱动程序在任何时候都不能随时启动和执行 DMA。|
|allowAll|双面|所有支持外部 DMA 的 PCIe 设备将在任何时候枚举。|



