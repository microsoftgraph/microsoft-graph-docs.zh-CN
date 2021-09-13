---
title: deliveryOptimizationBandwidthBusinessHoursLimit 资源类型
description: 带宽工作时间和百分比类型
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 428ed64455e0c403a4ea198a1cc367576d94b0a2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147981"
---
# <a name="deliveryoptimizationbandwidthbusinesshourslimit-resource-type"></a>deliveryOptimizationBandwidthBusinessHoursLimit 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

带宽工作时间和百分比类型

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|bandwidthBeginBusinessHours|Int32|指定使用 24 小时制的工作时间的开始 (0-23) 。 有效值为 0 到 23|
|bandwidthEndBusinessHours|Int32|指定使用 24 小时制的工作时间结束， (0-23) 。 有效值为 0 到 23|
|bandwidthPercentageDuringBusinessHours|Int32|指定在工作时间限制的带宽百分比， (0-100) 。 有效值为 0 至 100|
|bandwidthPercentageOutsideBusinessHours|Int32|指定限制工作时间的带宽百分比， (0-100) 。 有效值为 0 至 100|

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



