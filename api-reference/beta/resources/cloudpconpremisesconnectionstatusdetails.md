---
title: cloudPcOnPremisesConnectionStatusDetails 资源类型
description: 云 PC 本地连接的状态详细信息。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: db40df3bcd89ac21eb50870e82fe6a34ced86828
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563770"
---
# <a name="cloudpconpremisesconnectionstatusdetails-resource-type"></a>cloudPcOnPremisesConnectionStatusDetails 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[CloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)的状态详细信息。

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|startDateTime|DateTimeOffset|连接运行状况检查的开始时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。|
|endDateTime|DateTimeOffset|连接运行状况检查的结束时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：“2014-01-01T00:00:00Z”。|
|healthChecks|[cloudPcOnPremisesConnectionHealthCheck](../resources/cloudpconpremisesconnectionhealthcheck.md) 集合|对连接进行的所有检查。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionStatusDetails"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnectionStatusDetails",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "healthChecks": [
    {
      "@odata.type": "microsoft.graph.cloudPcOnPremisesConnectionHealthCheck",
      "displayName": "String",
      "status": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)",
      "errorType": "String",
      "recommendedAction": "String",
      "additionalDetails": "String"
    }
  ]
}
```
