---
title: deliveryOptimizationBandwidthBusinessHoursLimit 资源类型
description: 带宽业务时间和百分比类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a21a81ebc18616b9d072ba9bba39ec4a1e1ee7db
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231645"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a>deliveryOptimizationBandwidthBusinessHoursLimit 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

带宽业务时间和百分比类型

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|bandwidthBeginBusinessHours|Int32|使用24小时制 (0-23) 指定营业时间的开始时间。 有效值为0到23|
|bandwidthEndBusinessHours|Int32|使用24小时制 (0-23) 指定营业时间的结束时间。 有效值为0到23|
|bandwidthPercentageDuringBusinessHours|Int32|指定在营业时间 (0-100) 时要限制的带宽百分比。 有效值为 0 至 100|
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




