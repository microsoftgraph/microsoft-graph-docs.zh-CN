---
title: deliveryOptimizationBandwidthBusinessHoursLimit 资源类型
description: 带宽业务时间和百分比类型
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 83e0402e7b63925e8c02c87a5c1abd9b08c9c8c6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794387"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a>deliveryOptimizationBandwidthBusinessHoursLimit 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

带宽业务时间和百分比类型

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|bandwidthBeginBusinessHours|Int32|指定使用24小时制的营业时间的开始时间（0-23）。 有效值为0到23|
|bandwidthEndBusinessHours|Int32|指定使用24小时制的营业时间结束（0-23）。 有效值为0到23|
|bandwidthPercentageDuringBusinessHours|Int32|指定在营业时间内要限制的带宽百分比（0-100）。 有效值为 0 至 100|
|bandwidthPercentageOutsideBusinessHours|Int32|指定要限制 outsidse 营业时间（0-100）的带宽百分比。 有效值为 0 至 100|

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



