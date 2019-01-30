---
title: scopedRoleMembership 资源类型
description: 作用域角色成员资格介绍目录角色，进一步范围限定到管理单元 (AU) 的用户的成员的身份。  这提供了一种机制，以允许租户范围公司 adminsistrator 以委派用户管理用户和组的子集组织 （由 AU 正在定义的子集） 的管理权限。
localization_priority: Normal
ms.openlocfilehash: 2d51ad696487e7daafb9b0f4fcef0934e4f6d6e2
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640789"
---
# <a name="scopedrolemembership-resource-type"></a>scopedRoleMembership 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

作用域角色成员资格介绍目录角色，进一步范围限定到管理单元 (AU) 的用户的成员的身份。  这提供了一种机制，以允许租户范围公司 adminsistrator 以委派用户管理用户和组的子集组织 （由 AU 正在定义的子集） 的管理权限。

## <a name="methods"></a>Methods
不支持直接查询到此资源。  请参阅[管理单元](administrativeunit.md)主题，若要查看有关如何查询范围角色成员身份，以及添加和移除范围角色成员身份信息。 

## <a name="properties"></a>属性
| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
|administrativeUnitId|string|唯一标识符的目录角色范围限定为管理单元|
|id|string| 作用域角色成员身份的唯一标识符。 只读。|
|roleId|string| 为目录角色中的成员的唯一标识符。|
|roleMemberInfo|[identity](identity.md)| 角色成员身份信息。 表示此作用域角色的成员的用户。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedrolemembership"
}-->

```json
{
  "administrativeUnitId": "string",
  "id": "string (identifier)",
  "roleId": "string",
  "roleMemberInfo": {"@odata.type": "microsoft.graph.identity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scopedrolemembership.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
