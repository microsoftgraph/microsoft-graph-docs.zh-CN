---
title: governanceResource 资源类型
description: 表示无法管理特权标识管理 (PIM) 的资源。 有关 Azure 资源，它可以是订阅和资源组，如虚拟机、 SQL 数据库等资源。
ms.openlocfilehash: 6a048680c3b9bb614287e764d547a20bd09b5d25
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191128"
---
# <a name="governanceresource-resource-type"></a>governanceResource 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示无法管理特权标识管理 (PIM) 的资源。 有关 Azure 资源，它可以是订阅和资源组，如虚拟机、 SQL 数据库等资源。


## <a name="methods"></a>方法

| 方法          | 返回类型 |说明|
|:---------------|:--------|:----------|
|[List](../api/governanceresource-list.md) | [governanceResource](../resources/governanceresource.md)集合|列出请求者有权访问的资源的集合。|
|[Get](../api/governanceresource-get.md) | [governanceResource](../resources/governanceresource.md) |读取属性并由 id 指定的资源实体的关系。|
|[注册](../api/governanceresource-register.md) | |注册 PIM 服务非托管 Azure 订阅或管理组。 |

不`POST`， `PUT`， `PATCH`，`DELETE`支持`roleDefinitions`现在实体集。

## <a name="properties"></a>属性
| 属性          |类型         |说明|
|:------------------|:----------|:----------|
|id                 |字符串     |资源的 id。 处于 GUID 格式。|
|externalId           |String   |外部资源，表示其原始 id 外部系统中的 id。 例如，订阅资源的外部 id 可以是"/ 订阅/c14ae696-5e0c-4e5d-88cc-bef6637737ac"。 |
|type               |字符串     |必需。 资源类型。 例如，对于 Azure 资源，键入无法为"订阅"、"ResourceGroup"、"Microsoft.Sql/server"等。|
|displayName        |字符串     |资源的显示名称。|
|状态             |字符串     |给定资源的状态。 例如，它可能表示是否资源被锁定或未 (值： `Active` / `Locked`)。 注意： 该属性可能进行扩展，以便将来以支持更多方案。|
|registeredDateTime|DateTimeOffset      |代表资源中 PIM 的注册时的日期时间。|
|registeredRoot|字符串      |PIM 中注册的资源的根范围 externalId。 根范围可以是父、 祖父或更高版本上级资源。|
|roleAssignmentCount|Int32      |可选。 给定资源的角色分配的数目。 若要获取的属性，请是明确使用`$select=roleAssignmentCount`查询中。|
|roleDefinitionCount|Int32      |可选。 给定资源的角色定义的数目。 若要获取的属性，请是明确使用`$select=roleDefinitionCount`查询中。|
|permissions|[governancePermission](../resources/governancepermission.md)      |可选。 它表示对资源的请求者的访问状态。若要获取的属性，请是明确使用`$select=permissions`查询中。|

## <a name="relationships"></a>Relationships
| 关系   | 类型                                         |说明|
|:---------------|:---------------------------------------------|:----------|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md)集合|角色分配资源的集合。|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md)集合|资源的角色定义的集合。|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)集合|角色分配请求资源的集合。|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md)集合|资源角色设置的集合。|
|父          |[governanceResource](../resources/governanceresource.md)           |只读。 父资源。 为`pimforazurerbac`方案中，它可以表示资源所属的订阅。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
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
  "registeredRoot": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
