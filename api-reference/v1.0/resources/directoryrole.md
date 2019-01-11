---
title: directoryRole 资源类型
description: 表示 Azure AD 目录角色。 Azure AD 目录角色也称为是*管理员角色*。 有关目录 （管理员） 角色的详细信息，请参阅 Azure AD 中分配管理员角色。 使用 Microsoft Graph 中，可以将用户分配到目录角色授予他们的目标角色的权限。 若要读取目录角色或更新其成员，它必须首先激活在租户中。 默认情况下已激活公司管理员的目录角色。 若要激活发送一个 POST 请求 id 为基于目录角色 directoryRoleTemplate 其他可用的目录角色。 继承自 directoryObject。
localization_priority: Priority
ms.openlocfilehash: 05d897d6426b2feab7c08adaa125788590675f66
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820865"
---
# <a name="directoryrole-resource-type"></a>directoryRole 资源类型

表示 Azure AD 目录角色。 Azure AD 目录角色也称为是*管理员角色*。 有关目录 （管理员） 角色的详细信息，请参阅[Azure AD 中的分配管理员角色](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)。 使用 Microsoft Graph 中，可以将用户分配到目录角色授予他们的目标角色的权限。 若要读取目录角色或更新其成员，它必须首先激活在租户中。 默认情况下已激活公司管理员的目录角色。 若要激活其他可用的目录角色将发送一个 POST 请求[directoryRoleTemplate](directoryroletemplate.md)目录角色所基于的 id。 继承自 [directoryObject](directoryobject.md)。
该资源支持：

- 通过提供 [delta](../api/directoryrole-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 directoryRole](../api/directoryrole-get.md) | [directoryRole](directoryrole.md) | 读取 directoryRol 对象的属性和关系。 |
|[列出 directoryRoles](../api/directoryrole-list.md) | [directoryRole](directoryrole.md) 集合 | 列出租户中激活的目录角色。 |
|[添加成员](../api/directoryrole-post-members.md) |[directoryObject](directoryobject.md)| 通过发布到成员导航属性将用户添加到目录角色。|
|[列出成员](../api/directoryrole-list-members.md) |[directoryObject](directoryobject.md) 集合| 从成员导航属性获取该目录角色成员的用户。|
|[删除成员](../api/directoryrole-delete-member.md) |[directoryObject](directoryobject.md)| 删除目录角色中的用户。|
|[激活 directoryRole](../api/directoryrole-post-directoryroles.md) |[directoryRole](directoryrole.md) | 激活目录角色。|
|[delta](../api/directoryrole-delta.md)|directoryRole 集合| 获得目录角色增量更改。 |

## <a name="properties"></a>属性
| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
|说明|String|目录角色说明。只读。 |
|displayName|String|目录角色的显示名称。只读。 |
|id|String|目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。|
|roleTemplateId|String| 此角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) 的 **id**。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。 |

## <a name="relationships"></a>关系
| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|members|[directoryObject](directoryobject.md) 集合|是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
