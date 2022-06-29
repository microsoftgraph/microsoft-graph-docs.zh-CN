---
title: directoryAudit 资源类型
description: 介绍 Microsoft 图形 API (REST) 的 directoryAudit 资源 (实体) ，它可帮助审核目录 (租户) 活动 (beta 版本) 。
author: SarahBar
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: ed1582886ed67ecc090a1866db1ecf3589c0bb11
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436559"
---
# <a name="directoryaudit-resource-type"></a>directoryAudit 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示目录审核项及其集合。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |列出集合中的目录审核项及其属性。|
|[获取 directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |获取特定目录审核项及其属性。|


## <a name="properties"></a>属性
| 属性|类型|  说明  |
|:--------------------|:------------------|:------------|
| activityDateTime    | DateTimeOffset                                      | 指示执行活动的日期和时间。 时间戳类型始终为 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。                                                                              |
| activityDisplayName | String                                              | 指示活动名称或操作名称（例如， “创建用户”、“向组中添加成员”）。 有关记录的活动列表，请参阅 [Azure Ad 活动列表](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)。 |
| additionalDetails   | [keyValue](keyvalue.md) 集合                  | 指示活动的其他详细信息。                                                                                                                                                                                                                          |
| category            | String                                              | 指示活动所针对的资源类别。 （例如：用户管理、组管理等。）                                                                                                                                              |
| correlationId       | Guid                                                | 指示有助于关联跨各种服务的活动的唯一 ID。 可用于跨服务跟踪日志。                                                                                                                                    |
| id                  | String                                              | 指示活动的唯一 ID。                                                                                                                                                                                                            |
| initiatedBy         | [auditActivityInitiator](auditactivityinitiator.md) | 指示有关启动活动的用户或应用的信息。                                                                                                                                                                                                    |
| loggedByService     | String                                              | 指示启动活动的服务的信息（例如：自助服务密码管理、核心目录、B2C、受邀用户、Microsoft Identity Manager、Privileged Identity Management）。                                                          |
| operationType       | String                                              | 指示已执行的操作的类型。 可能的值包括但不限于以下内容：`Add`、`Assign`、`Update`和 `Unassign``Delete`。                                                                                   |
| result              | operationResult                                              | 指示活动的结果。 可能的值是：`success`、`failure`、`timeout`、`unknownFutureValue`。                                                                                                                                                       |
| resultReason        | String                                              | 指示失败的原因（如果 **结果** 为 `failure` 或 `timeout`）。                                                                                                                                                                                              |
| targetResources     | [targetResource](targetresource.md) 集合      | 有关因活动而更改的资源的信息。  | 
| userAgent | String | 活动中用户使用的用户代理类型。 |                                                                                                      

## <a name="relationships"></a>关系
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
  "operationType": "String",
  "result": "string",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}],
  "userAgent": "String"
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


