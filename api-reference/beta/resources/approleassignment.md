---
title: appRoleAssignment 资源类型
description: 用于记录时用户或组分配给应用程序。 在这种情况下，该角色分配将导致应用程序图块显示安装在用户的应用程序访问面板上。 此实体还可能用于授予对特定的角色中的资源应用程序的另一个应用程序 （作为服务主体建模） 访问权限。 您可以创建、 读取、 更新和删除角色分配。
localization_priority: Priority
ms.openlocfilehash: 3276c1f34b91dc628ed00f2ffbc64ffe56899bdf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845470"
---
# <a name="approleassignment-resource-type"></a>appRoleAssignment 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

用于记录时用户或组分配给应用程序。 在这种情况下，该角色分配将导致应用程序图块显示安装在用户的应用程序访问面板上。 此实体还可能用于授予对特定的角色中的资源应用程序的另一个应用程序 （作为服务主体建模） 访问权限。 您可以创建、 读取、 更新和删除角色分配。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approleassignment"
}-->

```json
{
  "creationTimestamp": "String (timestamp)",
  "id": "guid (identifier)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|creationTimestamp|DateTimeOffset|授予创建时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|id|Guid|已分配给主体角色 id。  必须由其**appRoles**属性中目标资源应用程序**resourceId**声明此角色。 如果资源没有声明任何权限，必须指定默认 id (零 GUID)。 键。 不可为 null。 |
|principalDisplayName|字符串|已授予访问权限的主体的显示名称。|
|principalId|Guid|要授予访问权限的主体的唯一标识符 (**id**)。 所需在创建。            |
|principalType|字符串|主体的类型。  这可以是"User"，"组"或"ServicePrincipal"。|
|resourceDisplayName|字符串|对其进行分配资源的显示名称。|
|resourceId|Guid|唯一标识符 (**id**) 为其进行工作分配的目标资源 （服务主体）。|

## <a name="relationships"></a>Relationships
无


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 appRoleAssignment](../api/approleassignment-get.md) | [appRoleAssignment](approleassignment.md) |读取属性和 appRoleAssignment 对象的关系。|
|[Update](../api/approleassignment-update.md) | [appRoleAssignment](approleassignment.md)   |更新 appRoleAssignment 对象。 |
|[删除](../api/approleassignment-delete.md) | 无 |删除 appRoleAssignment 对象。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
