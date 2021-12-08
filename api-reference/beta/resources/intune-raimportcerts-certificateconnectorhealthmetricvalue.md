---
title: certificateConnectorHealthMetricValue 资源类型
description: 响应 GetHealthMetricTimeSeries 请求时返回的指标快照值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e6201f79b302378d1452284ed52d14dab4eccc94
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341003"
---
# <a name="certificateconnectorhealthmetricvalue-resource-type"></a>certificateConnectorHealthMetricValue 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

响应 GetHealthMetricTimeSeries 请求时返回的指标快照值。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|dateTime|DateTimeOffset|此指标数据点的时间戳。|
|successCount|Int64|成功的请求/操作计数。|
|failureCount|Int64|失败的请求/操作计数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorHealthMetricValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorHealthMetricValue",
  "dateTime": "String (timestamp)",
  "successCount": 1024,
  "failureCount": 1024
}
```




