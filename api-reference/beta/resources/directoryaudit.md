---
title: directoryAudit 资源类型
description: 此资源表示的目录审核项，并且其集合
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1f980208788731206dc58870635644a1f3edc4c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991781"
---
# <a name="directoryaudit-resource-type"></a>directoryAudit 资源类型
此资源表示的目录审核项，并且其集合


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列表 directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |列表中的集合，及其属性的目录审核项。|
|[获取 directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |获取特定目录审核项和其属性。|


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|activityDateTime|DateTimeOffset|指示的日期和时间执行活动。 时间戳类型始终为 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|activityDisplayName|字符串|指示活动名称或操作名称 （例如 "创建用户"，"向组添加成员")。 有关记录的活动的列表，请参阅[Azure Ad 活动列表](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)。|
|additionalDetails|[keyValue](keyvalue.md)集合|指示活动的其他详细信息。|
|category|String|指示活动所针对的资源类别。 (例如： 用户管理、 组管理等。。)|
|correlationId|GUID|指示帮助关联跨越各种服务的活动的唯一 ID。 可以使用跟踪日志服务。|
|id|字符串| 指示活动的唯一 ID。 这是一个 GUID。|
|initiatedBy|[auditActivityInitiator](auditactivityinitiator.md)|指示信息的用户或应用程序启动活动。|
|loggedByService|字符串|指示服务在其启动活动的信息 (例如： 自助服务密码管理、 核心目录、 B2C、 邀请用户、 Microsoft Identity Manager、 特权身份管理。|
|结果|string| 指示活动的结果。可能的值为： `success`， `failure`， `timeout`， `unknownFutureValue`。||
|resultReason|字符串|如果结果为"Failure"或"超时"，指示失败的原因。|
|targetResources|[targetResource](targetresource.md)集合|指示由于活动更改资源的信息。 目标资源类型可以是用户、 设备、 目录、 应用程序、 角色、 组、 策略或其他。

## <a name="relationships"></a>Relationships
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryAudit"
}-->

```json
{
  "activityDateTime": "String (timestamp)",
  "activityDisplayName": "String",
  "additionalDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "category": "String",
  "correlationId": "Guid",
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.auditActivityInitiator"},
  "loggedByService": "String",
  "result": "string",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryAudit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
