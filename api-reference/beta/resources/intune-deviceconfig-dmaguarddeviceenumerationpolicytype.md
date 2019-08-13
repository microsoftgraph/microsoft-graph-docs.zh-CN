---
title: dmaGuardDeviceEnumerationPolicyType 枚举类型
description: DmaGuardDeviceEnumerationPolicy 的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 484e7ffbd13234a24be983af1d94e8dca0d55f34
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332692"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>dmaGuardDeviceEnumerationPolicyType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DmaGuardDeviceEnumerationPolicy 的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|默认值。 具有 DMA 重新映射的设备将仅在用户解锁屏幕后枚举不兼容驱动程序。|
|blockAll|1|具有 DMA 重新映射的设备不支持的驱动程序在任何时候都不能随时启动和执行 DMA。|
|allowAll|双面|所有支持外部 DMA 的 PCIe 设备将在任何时候枚举。|



