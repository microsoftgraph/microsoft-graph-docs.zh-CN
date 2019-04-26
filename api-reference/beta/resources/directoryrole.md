---
title: directoryRole 资源类型
description: 表示 Azure AD 目录角色。 Azure AD 目录角色也称为*管理员角色*。 有关目录 (管理员) 角色的详细信息, 请参阅在 Azure AD 中分配管理员角色。 使用 Microsoft Graph, 可以将用户分配到目录角色, 以向他们授予目标角色的权限。 要读取目录角色或更新其成员，首先必须在租户中将其激活。 默认情况下仅激活公司管理员目录角色。 若要激活其他可用的目录角色, 请使用目录角色所基于的 directoryRoleTemplate 的 ID 发送 POST 请求。 继承自 directoryObject。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 110febf3213431a0a44941a4cdd2bd9bca255bff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334572"
---
# <a name="directoryrole-resource-type"></a>directoryRole 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure AD 目录角色。 Azure AD 目录角色也称为*管理员角色*。 有关目录 (管理员) 角色的详细信息, 请参阅[在 Azure AD 中分配管理员角色](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)。 使用 Microsoft Graph, 可以将用户分配到目录角色, 以向他们授予目标角色的权限。 要读取目录角色或更新其成员，首先必须在租户中将其激活。 默认情况下仅激活公司管理员目录角色。 若要激活其他可用的目录角色, 请使用目录角色所基于的[directoryRoleTemplate](directoryroletemplate.md)的 ID 发送 POST 请求。 继承自 [directoryObject](directoryobject.md)。

默认情况下, 目录角色的作用域为 "租户范围"。  但是, 目录角色 (目前只有*用户帐户管理员*和*支持人员管理员*) 也可能作用于[管理单元](administrativeunit.md)。

该资源支持：

- 通过提供 [delta](../api/directoryrole-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 directoryRole](../api/directoryrole-get.md) | [directoryRole](directoryrole.md) |读取 directoryRol 对象的属性和关系。|
|[列出 directoryRoles](../api/directoryrole-list.md) | [directoryRole](directoryrole.md) 集合 | 列出租户中激活的目录角色。 |
|[Add member](../api/directoryrole-post-members.md) |[directoryObject](directoryobject.md)| 通过发布到成员导航属性将用户添加到目录角色。|
|[List members](../api/directoryrole-list-members.md) |[directoryObject](directoryobject.md) 集合| 从成员导航属性获取该目录角色成员的用户。|
|[删除成员](../api/directoryrole-delete-member.md) |[directoryObject](directoryobject.md)| 从目录角色中删除用户。|
|[列出作用域内的角色成员](../api/directoryrole-list-members.md) |[scopedRoleMembership](scopedrolemembership.md) 集合| 通过 scopedRoleMembership 资源集合列出此目录角色的范围限定为[管理单元](administrativeunit.md)的成员。|
|[delta](../api/directoryrole-delta.md)|directoryRole 集合| 获取目录角色的增量更改。 |

## <a name="properties"></a>属性
| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|说明|String|目录角色说明。只读。 |
|displayName|字符串|目录角色的显示名称。只读。 |
|id|字符串|目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。|
|roleTemplateId|String| 此角色所基于的 **directoryRoleTemplate** 的 [id](directoryroletemplate.md)。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。 |

## <a name="relationships"></a>关系
| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
|members|[directoryObject](directoryobject.md) 集合|是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 NULL。|
|scopedMembers|[scopedRoleMembership](scopedrolemembership.md) 集合| 此目录角色的作用域为 "[管理单元](administrativeunit.md)" 的成员。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
