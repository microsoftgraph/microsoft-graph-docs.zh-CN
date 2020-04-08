---
title: directoryAudit 资源类型
description: 介绍了 Microsoft Graph API （REST）的 directoryAudit 资源（实体），它可帮助审核目录（租户）活动（测试版）。
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 723c9089ed19e6d69375bd815b4233594be286a2
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181970"
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
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|activityDateTime|DateTimeOffset|指示执行活动的日期和时间。 时间戳类型始终为 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|activityDisplayName|String|指示活动名称或操作名称（例如， “创建用户”、“向组中添加成员”）。 有关记录的活动列表，请参阅 [Azure AD 活动列表](/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)。|
|additionalDetails|[keyValue](keyvalue.md) 集合|指示活动的其他详细信息。|
|category|字符串|指示活动所针对的资源类别。 （例如：用户管理、组管理等。）|
|correlationId|GUID|指示有助于关联跨各种服务的活动的唯一 ID。 可用于跨服务跟踪日志。|
|id|String| 指示活动的唯一 ID。 这是 GUID。|
|initiatedBy|[auditActivityInitiator](auditactivityinitiator.md)|指示有关启动活动的用户或应用的信息。|
|loggedByService|String|指示启动活动的服务的信息（例如：自助服务密码管理、核心目录、B2C、受邀用户、Microsoft Identity Manager、Privileged Identity Management）。|
|result|string| 指示活动的结果。可取值为：`success`、`failure`、`timeout`、`unknownFutureValue`。||
|resultReason|String|如果结果为“失败”或“超时”，指示失败的原因。|
|targetResources|[targetResource](targetresource.md) 集合|指示由于活动而更改的资源的信息。 目标资源类型可以是用户、设备、目录、应用、角色、组、策略或其他。

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
