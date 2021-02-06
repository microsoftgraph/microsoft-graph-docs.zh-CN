---
title: scopedRoleMembership 资源类型
description: 作用域角色成员身份描述目录角色的用户成员身份，该角色的范围进一步缩小到 AU (管理) 。  这提供了一种机制，允许租户范围的公司管理员将管理权限委派给用户，以管理组织子集中的用户和组 (由 AU 管理员定义的子集) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: abhijeetsinha
ms.openlocfilehash: ffd1e616d94ccf959b8535f46f79a2c7c57e00c2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134696"
---
# <a name="scopedrolemembership-resource-type"></a>scopedRoleMembership 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

作用域角色成员身份描述目录角色的用户成员身份，该角色的范围进一步缩小到 AU (管理) 。  这提供了一种机制，允许租户范围的公司管理员将管理权限委派给用户，以管理组织子集中的用户和组 (该子集由 AU) 。

## <a name="methods"></a>方法
不支持直接查询此资源。  请参阅管理 [单元](administrativeunit.md) 主题，了解如何查询作用域角色成员身份以及添加和删除作用域角色成员身份。

## <a name="properties"></a>属性
| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
|administrativeUnitId|string|目录角色作用域为的管理单元的唯一标识符|
|id|string| 作用域角色成员身份的唯一标识符。 只读。|
|roleId|string| 成员位于的目录角色的唯一标识符。|
|roleMemberInfo|[identity](identity.md)| 角色成员标识信息。 表示是此作用域角色的成员的用户。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedRoleMembership"
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
  "suppressions": []
}
-->


