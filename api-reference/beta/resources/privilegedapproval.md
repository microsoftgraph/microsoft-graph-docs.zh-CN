---
title: privilegedApproval 资源类型
description: 表示在用于获取角色的特权标识管理中请求的审批。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: c4148e5740c9b31368be336a615524ced426a560
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219226"
---
# <a name="privilegedapproval-resource-type"></a>privilegedApproval 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在用于获取角色的特权标识管理中请求的审批。


## <a name="methods"></a>Methods

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 privilegedApproval](../api/privilegedapproval-get.md) | [privilegedApproval](privilegedapproval.md) |读取 privilegedApproval 对象的属性和关系。|
|[列出 privilegedApproval 对象](../api/privilegedapproval-list.md) | [privilegedApproval](privilegedapproval.md) 集合|获取 privilegedApproval 的集合。|
|[创建 privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |创建 privilegedApproval 对象。 |
|[更新 privilegedApproval](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |更新 privilegedApproval 对象。 |
|[Myrequests](../api/privilegedapproval-myrequests.md)|[privilegedApproval](privilegedapproval.md)|获取请求者的审批请求。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|approvalDuration|持续时间||
|approvalState|string| 可取值为：`pending`、`approved`、`denied`、`aborted`、`canceled`。|
|approvalType|字符串||
|approverReason|字符串||
|endDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|id|字符串| 只读。|
|requestorReason|字符串||
|roleId|字符串||
|startDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|userId|String||

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| 只读。 可为 Null。|
|申请|[privilegedRoleAssignmentRequest](privilegedroleassignmentrequest.md)| 只读。 此审批对象的角色分配请求|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedApproval"
}-->

```json
{
  "approvalDuration": "string (timestamp)",
  "approvalState": "string",
  "approvalType": "string",
  "approverReason": "String",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "requestorReason": "String",
  "roleId": "String",
  "startDateTime": "String (timestamp)",
  "userId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedApproval resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
