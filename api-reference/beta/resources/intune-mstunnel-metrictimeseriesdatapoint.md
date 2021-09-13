---
title: metricTimeSeriesDataPoint 资源类型
description: 指标时间系列数据点
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c550f145d99b82307f1ec3ed88040ff1c2357609
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068695"
---
# <a name="metrictimeseriesdatapoint-resource-type"></a>metricTimeSeriesDataPoint 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指标时间系列数据点

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|dateTime|DateTimeOffset|指标时间系列数据点的时间|
|值|Int64|指标时间系列数据点的值|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.metricTimeSeriesDataPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.metricTimeSeriesDataPoint",
  "dateTime": "String (timestamp)",
  "value": 1024
}
```



