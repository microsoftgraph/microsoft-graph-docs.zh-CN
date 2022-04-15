---
title: directoryAudit 资源类型
description: 表示目录审核项及其集合。
author: SarahBar
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 08a723f5d26e6d45b6cb4e7ede6b2d5a496dab86
ms.sourcegitcommit: b21ad24622e199331b6ab838a949ddce9726b41b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2022
ms.locfileid: "64848732"
---
# <a name="directoryaudit-resource-type"></a>directoryAudit 资源类型

命名空间：microsoft.graph

表示目录审核项及其集合。

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 directoryAudits](../api/directoryaudit-list.md) | [directoryAudit](directoryaudit.md) |列出集合中的目录审核项及其属性。|
|[获取 directoryAudit](../api/directoryaudit-get.md) | [directoryAudit](directoryaudit.md) |获取特定目录审核项及其属性。|

## <a name="properties"></a>属性

| 属性            | 类型                                                | 说明                                                                                                                                                                                                                                                                        |
|:--------------------|:----------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| activityDateTime    | DateTimeOffset                                      | 指示执行活动的日期和时间。 时间戳类型始终为 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。                                                                                          |
| activityDisplayName | String                                              | 指示活动名称或操作名称 (示例：“创建用户”和“将成员添加到组”) 。 有关完整列表，请参阅[Azure AD活动列表](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)。 |
| additionalDetails   | [keyValue](keyvalue.md) 集合                  | 指示活动的其他详细信息。                                                                                                                                                                                                                                      |
| category            | String                                              | 指示活动所针对的资源类别。 （例如：用户管理、组管理等。）                                                                                                                                                          |
| correlationId       | Guid                                                | 指示有助于关联跨各种服务的活动的唯一 ID。 可用于跨服务跟踪日志。                                                                                                                                                |
| id                  | String                                              | 指示活动的唯一 ID。 这是 GUID。                                                                                                                                                                                                                          |
| initiatedBy         | [auditActivityInitiator](auditactivityinitiator.md) | 指示有关启动活动的用户或应用的信息。                                                                                                                                                                                                                |
| operationType       | 字符串                                              | 指示已执行的操作的类型。 可能的值包括但不限于以下内容：`Add`、`Assign`、`Update`和 `Unassign``Delete`。                                                                                   |
| loggedByService     | String                                              | 指示有关哪个服务启动了活动的信息 (例如： `Self-service Password Management`， ， `Core Directory``B2C`， `Invited Users`， 。 `Privileged Identity Management``Microsoft Identity Manager`                                                                      |
| result              | operationResult                                              | 指示活动的结果。 可能的值是：`success`、`failure`、`timeout`、`unknownFutureValue`。                                                                                                                                                                   |
| resultReason        | String                                              | 指示失败的原因（如果 **结果** 为 `failure` 或 `timeout`）。                                                                                                                                                                                                                                 |
| targetResources     | [targetResource](targetresource.md) 集合      | 指示由于活动而更改的资源的信息。 目标资源类型可以是`User`、`Device`、`Directory`、`App`、`Role`或 `Group``Policy` `Other`。                                                                                                                   |

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
  "result": "String",
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
