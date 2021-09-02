---
title: timeSeriesParameter 资源类型
description: 请求快照时间系列时传递给 GetHealthMetricTimeSeries 的参数。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da593d882a0ab4fb4681c06bbb1c40cbb03a86ba
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58762990"
---
# <a name="timeseriesparameter-resource-type"></a>timeSeriesParameter 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

请求快照时间系列时传递给 GetHealthMetricTimeSeries 的参数。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|metricName|String|请求时间序列的指标的名称。|
|startDateTime|DateTimeOffset|所请求的系列的开始时间。|
|endDateTime|DateTimeOffset|所请求的系列的结束时间。 可选;如果未指定，则使用当前时间。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.timeSeriesParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.timeSeriesParameter",
  "metricName": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```



