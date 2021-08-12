---
title: serviceHealth 资源类型
description: 表示服务的运行状况信息。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 254702516d536617ef5afa114bc7a41761ce3499a932b4c7e2d8560ac7f92441
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54195591"
---
# <a name="servicehealth-resource-type"></a>serviceHealth 资源类型

命名空间：microsoft.graph

表示租户订阅的服务的运行状况信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 serviceHealth](../api/servicehealth-get.md)|[serviceHealth](../resources/servicehealth.md)|检索 [serviceHealth 对象的属性和](../resources/servicehealth.md) 关系。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|服务 ID。|
|service|String|服务名称。 使用 [列表 healthOverviews](../api/serviceannouncement-list-healthoverviews.md) 操作获取租户订阅的服务的确切字符串名称。|
|status|serviceHealthStatus|显示一性服务运行状况状态。 可能的值是 `serviceOperational` `investigating` `restoringService` ：、、、、、、、、、 `verifyingService` `serviceRestored` `postIncidentReviewPublished` `serviceDegradation` `serviceInterruption` `extendedRecovery` `falsePositive` `investigationSuspended` `resolved` `mitigatedExternal` `mitigated` `resolvedExternal` `confirmed` `reported` `unknownFutureValue` 。|

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

