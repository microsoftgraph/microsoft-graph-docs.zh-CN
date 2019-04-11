---
title: deliveryOptimizationBandwidthBusinessHoursLimit 资源类型
description: 带宽业务时间和百分比类型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1115029cd7106f19a2a8a706540278a5282ca18d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776253"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a>deliveryOptimizationBandwidthBusinessHoursLimit 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

带宽业务时间和百分比类型

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|bandwidthBeginBusinessHours|Int32|指定使用24小时制的营业时间的开始时间 (0-23)。 有效值为0到23|
|bandwidthEndBusinessHours|Int32|指定使用24小时制的营业时间结束 (0-23)。 有效值为0到23|
|bandwidthPercentageDuringBusinessHours|Int32|指定在营业时间内要限制的带宽百分比 (0-100)。 有效值为 0 至 100|
|bandwidthPercentageOutsideBusinessHours|Int32|指定要限制 outsidse 营业时间 (0-100) 的带宽百分比。 有效值为 0 至 100|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationBandwidthBusinessHoursLimit",
  "bandwidthBeginBusinessHours": 1024,
  "bandwidthEndBusinessHours": 1024,
  "bandwidthPercentageDuringBusinessHours": 1024,
  "bandwidthPercentageOutsideBusinessHours": 1024
}
```





