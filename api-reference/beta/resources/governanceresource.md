---
title: governanceResource 资源类型
description: 表示可由 Privileged Identity Management (PIM) 管理的资源。 对于 Azure 资源，它可以是订阅、资源组和资源（例如虚拟机、SQL数据库等）。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 0be4deb0ae3e96ff1c5a19b7d398ff980c2760ae
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397479"
---
# <a name="governanceresource-resource-type"></a>governanceResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

表示可由 Privileged Identity Management (PIM) 管理的资源。 对于 Azure 资源，它可以是订阅、资源组和资源（例如虚拟机、SQL数据库等）。


## <a name="methods"></a>方法

| 方法          | 返回类型 |Description|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | [governanceResource](../resources/governanceresource.md) 集合|列出请求者有权访问的资源集合。|
|[Get](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |读取 ID 指定的资源实体的属性和关系。|
|[注册](../api/governanceresource-register.md) | |将非托管 Azure 订阅或管理组注册到 PIM 服务。 |

`PUT``PATCH`目前，实体集支持`roleDefinitions`“否`POST`”，`DELETE`即“不”。

## <a name="properties"></a>属性
| 属性          |类型         |说明|
|:------------------|:----------|:----------|
|id                 |字符串     |资源的 ID。 它采用 GUID 格式。|
|externalId           |String   |资源的外部 ID，表示其在外部系统中的原始 ID。 例如，订阅资源的外部 ID 可以是“/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac”。 |
|type               |String     |必填。 资源类型。 例如，对于 Azure 资源，类型可以是“Subscription”、“ResourceGroup”、“Microsoft.Sql/server”等。|
|displayName        |String     |资源的显示名称。|
|status             |String     |给定资源的状态。 例如，它可以表示资源是否已锁定 (值： `Active`/`Locked`) 。 注意：将来可能会扩展此属性以支持更多方案。|
|registeredDateTime|DateTimeOffset      |表示在 PIM 中注册资源的日期时间。|
|registeredRoot|String      |在 PIM 中注册的资源根范围的 externalId。 根范围可以是父级、祖父母或上级资源。|
|roleAssignmentCount|Int32      |可选。 给定资源的角色分配数。 若要获取属性，请在查询中隐式使用 `$select=roleAssignmentCount` 。|
|roleDefinitionCount|Int32      |可选。 给定资源的角色定义数。 若要获取属性，请在查询中隐式使用 `$select=roleDefinitionCount` 。|
|permissions|[governancePermission](../resources/governancepermission.md)      |可选。 它表示请求者对资源的访问状态。若要获取属性，请在查询中隐式使用 `$select=permissions` 。|

## <a name="relationships"></a>关系
| 关系   | 类型                                         |说明|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md) 集合|资源的角色分配集合。|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md) 集合|资源的角色缺陷的集合。|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 集合|资源的角色分配请求的集合。|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md) 集合|资源的角色设置集合。|
|父级          |[governanceResource](../resources/governanceresource.md)           |只读。 父资源。 对于 `pimforazurerbac` 方案，它可以表示资源所属的订阅。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceResource"
}-->
```json
{
  "id": "String (identifier)",
  "externalId": "String",
  "type": "String",
  "displayName": "String",
  "status": "String",
  "registeredDateTime": "String (timestamp)",
  "registeredRoot": "String",
  "roleAssignmentCount": 12356,
  "roleDefinitionCount": 12356,
  "permissions": {
    "@odata.type": "microsoft.graph.governancePermission"
  }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


