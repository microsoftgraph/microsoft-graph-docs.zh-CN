---
title: governanceResource 资源类型
description: 表示可由特权标识管理（PIM）管理的资源。 对于 Azure 资源，它可以是订阅、资源组和资源（如虚拟机、SQL 数据库等）。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 28af0f6ca55881bd0f0848cda27cfe56bd1d5eb5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497613"
---
# <a name="governanceresource-resource-type"></a>governanceResource 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可由特权标识管理（PIM）管理的资源。 对于 Azure 资源，它可以是订阅、资源组和资源（如虚拟机、SQL 数据库等）。


## <a name="methods"></a>方法

| 方法          | 返回类型 |说明|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | [governanceResource](../resources/governanceresource.md)集合|列出请求者有权访问的资源的集合。|
|[获取](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |读取由 id 指定的资源实体的属性和关系。|
|[报名](../api/governanceresource-register.md) | |将非托管 Azure 订阅或管理组注册到 PIM 服务。 |

目前`POST`， `PUT`entity `PATCH`set `DELETE`上`roleDefinitions`不支持，，。

## <a name="properties"></a>属性
| 属性          |类型         |说明|
|:------------------|:----------|:----------|
|id                 |String     |资源的 id。 它采用 GUID 格式。|
|externalId           |String   |资源的外部 id，表示其在外部系统中的原始 id。 例如，订阅资源的外部 id 可以是 "/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"。 |
|type               |String     |必填。 资源类型。 例如，对于 Azure 资源，类型可以是 "订阅"、"ResourceGroup"、"Microsoft .Sql/服务器" 等。|
|displayName        |String     |资源的显示名称。|
|status             |String     |给定资源的状态。 例如，它可以表示资源是否已锁定（values： `Active` / `Locked`）。 注意：将来可能会扩展此属性以支持更多方案。|
|registeredDateTime|DateTimeOffset      |表示在 PIM 中注册资源的日期时间。|
|registeredRoot|String      |在 PIM 中注册的资源的根作用域的 externalId。 根作用域可以是父级、祖父或更高的上级资源。|
|roleAssignmentCount|Int32      |可选。 给定资源的角色分配数。 若要获取属性，请明确在`$select=roleAssignmentCount`查询中使用。|
|roleDefinitionCount|Int32      |可选。 给定资源的角色定义的数量。 若要获取属性，请明确在`$select=roleDefinitionCount`查询中使用。|
|permissions|[governancePermission](../resources/governancepermission.md)      |可选。 它表示请求者对资源的访问状态。若要获取属性，请明确在`$select=permissions`查询中使用。|

## <a name="relationships"></a>关系
| 关系   | 类型                                         |说明|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md)集合|资源的角色分配的集合。|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md)集合|资源的角色 defintions 集合。|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合|资源的角色分配请求的集合。|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md)集合|资源的角色设置的集合。|
|母语          |[governanceResource](../resources/governanceresource.md)           |只读。 父资源。 对于`pimforazurerbac`方案，它可以表示资源所属的订阅。|

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
