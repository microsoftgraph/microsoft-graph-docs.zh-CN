---
title: deviceScopeStatus 枚举类型
description: 指示设备范围启用后的设备范围状态。 可能的值为：none、computing、insufficientData 或 completed。 默认值为无。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8347440c0c02f0f6c148717457616a19c22bc03f
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858557"
---
# <a name="devicescopestatus-enum-type"></a>deviceScopeStatus 枚举类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示设备范围启用后的设备范围状态。 可能的值为：none、computing、insufficientData 或 completed。 默认值为无。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|指示设备范围未启用，并且没有正在进行的计算。|
|计算|1|指示设备范围已启用，并且服务正在重新计算报表指标数据。|
|insufficientData|2|指示设备范围已启用，但数据不足以计算结果。 系统需要至少 5 台设备提供信息，然后才能进行计算。|
|完成|3|设备范围已启用并完成对报表指标的重新计算。 设备范围现已准备就绪，可供使用。|
|unknownFutureValue|4|将来扩展的占位符值。|




