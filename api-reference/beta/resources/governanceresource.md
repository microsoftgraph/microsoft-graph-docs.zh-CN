---
title: governanceResource 资源类型
description: 表示由 PIM Privileged Identity Management (管理) 。 对于 Azure 资源，它可以是订阅、资源组和资源（如虚拟机、SQL数据库等）。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: 5eacdb75d6607827eaf288b3eed17d41cce07f66
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510560"
---
# <a name="governanceresource-resource-type"></a>governanceResource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

表示由 PIM Privileged Identity Management (管理) 。 对于 Azure 资源，它可以是订阅、资源组和资源（如虚拟机、SQL数据库等）。


## <a name="methods"></a>方法

| 方法          | 返回类型 |Description|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | [governanceResource](../resources/governanceresource.md) 集合|列出请求者有权访问的资源集合。|
|[Get](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |读取由 id 指定的资源实体的属性和关系。|
|[注册](../api/governanceresource-register.md) | |将非托管 Azure 订阅或管理组注册到 PIM 服务。 |

目前`POST`，`PUT`实体`PATCH``DELETE`集不支持 `roleDefinitions` 、 。

## <a name="properties"></a>属性
| 属性          |类型         |说明|
|:------------------|:----------|:----------|
|id                 |String     |资源的 ID。 它采用 GUID 格式。|
|externalId           |String   |资源的外部 ID，表示其外部系统中的原始 ID。 例如，订阅资源的外部 ID 可以是"/subscriptions/c14ae696-5e0c-4e5d-88cc-bef6637737ac"。 |
|type               |String     |必需。 资源类型。 例如，对于 Azure 资源，类型可以是"Subscription"、"ResourceGroup"、"Microsoft.Sql/server"等。|
|displayName        |String     |资源的显示名称。|
|状态             |字符串     |给定资源的状态。 例如，它可以表示资源是否已锁定 (值： `Active`/`Locked`) 。 注意：以后可能会扩展此属性以支持更多方案。|
|registeredDateTime|DateTimeOffset      |表示在 PIM 中注册资源的日期时间。|
|registeredRoot|String      |在 PIM 中注册的资源根范围的 externalId。 根范围可以是父级、上级或更高上级资源。|
|roleAssignmentCount|Int32      |可选。 给定资源的角色分配数。 若要获取 属性，请在查询中 `$select=roleAssignmentCount` 明显使用 。|
|roleDefinitionCount|Int32      |可选。 给定资源的角色定义的数量。 若要获取 属性，请在查询中 `$select=roleDefinitionCount` 明显使用 。|
|permissions|[governancePermission](../resources/governancepermission.md)      |可选。 它表示请求者对资源的访问权限的状态。若要获取 属性，请在查询中 `$select=permissions` 明显使用 。|

## <a name="relationships"></a>关系
| 关系   | 类型                                         |说明|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md) 集合|资源的角色分配集合。|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md) 集合|资源的角色定义集合。|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) 集合|资源角色分配请求的集合。|
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


