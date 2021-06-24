---
title: serviceHealth 资源类型
description: 表示服务的运行状况信息。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: c11750bbffe64315c6263a26d7dbab333f42b7cf
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109097"
---
# <a name="servicehealth-resource-type"></a>serviceHealth 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示服务的运行状况信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 serviceHealth](../api/servicehealth-get.md)|[serviceHealth](../resources/servicehealth.md)|检索 [serviceHealth 对象的属性和](../resources/servicehealth.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串|服务 ID。|
|service|String|服务名称。|
|状态|serviceHealthStatus|显示一性服务运行状况状态。 可能的值是 `serviceOperational` `investigating` `restoringService` ：、、、、、、、、、 `verifyingService` `serviceRestored` `postIncidentReviewPublished` `serviceDegradation` `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` `reported` `unknownFutureValue` 。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|问题|collection ([serviceHealthIssue) ](../resources/servicehealthissue.md)|服务上发生的问题集合，以及每个问题的详细信息。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceHealth",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceHealth",
  "service": "String",
  "status": "String",
  "id": "String (identifier)"
}
```

