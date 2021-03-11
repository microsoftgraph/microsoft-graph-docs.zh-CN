---
title: privilegedApproval 资源类型
description: 表示在 Privileged Identity Management 中请求获取角色的审批。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 7d7842b89bce06d582aa827b853e4170b0693ff8
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721605"
---
# <a name="privilegedapproval-resource-type"></a>privilegedApproval 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在 Privileged Identity Management 中请求获取角色的审批。


## <a name="methods"></a>方法

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
|approvalType|String||
|approverReason|String||
|endDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|id|String| 只读。|
|requestorReason|String||
|roleId|String||
|startDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|userId|String||

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| 只读。 可为 NULL。|
|request|[privilegedRoleAssignmentRequest](privilegedroleassignmentrequest.md)| 只读。 此角色分配审批对象的请求|

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


