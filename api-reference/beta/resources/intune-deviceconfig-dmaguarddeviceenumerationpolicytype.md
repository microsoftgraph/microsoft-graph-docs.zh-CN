---
title: dmaGuardDeviceEnumerationPolicyType 枚举类型
description: DmaGuardDeviceEnumerationPolicy 的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5baa0cfd5c80f954036e10f0e4d04d2b83e57f2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429482"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a>dmaGuardDeviceEnumerationPolicyType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

DmaGuardDeviceEnumerationPolicy 的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|默认值。 用户解除锁定的屏幕后，将仅枚举设备 DMA 重新映射不兼容的驱动程序。|
|blockAll|1|从不允许设备 DMA 重新映射不兼容的驱动程序启动并随时执行 DMA。|
|allowAll|2|在任何时候都将被枚举所有外部的 DMA 能够 PCIe 设备。|




