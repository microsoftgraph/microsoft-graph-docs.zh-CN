---
title: scopedRoleMembership 资源类型
description: 作用域角色成员身份描述用户目录角色的成员身份，该角色的成员将进一步限定为管理单元 (AU) 。  这提供了一种机制，允许租户范围内的公司 adminsistrator 将管理权限委派给用户，以管理由 AU) 定义的一部分组织中的用户和组 (。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abhijeetsinha
ms.openlocfilehash: 27eae463ab0f5fe0718a6d97602e366d32b11b86
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46812440"
---
# <a name="scopedrolemembership-resource-type"></a>scopedRoleMembership 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

作用域角色成员身份描述用户目录角色的成员身份，该角色的成员将进一步限定为管理单元 (AU) 。  这提供了一种机制，允许租户范围内的公司管理员将管理权限委派给用户，以管理由 AU) 定义的部分组织中的用户和组 (。

## <a name="methods"></a>方法
不支持直接向此资源进行查询。  请参阅 " [管理单元](administrativeunit.md) " 主题，查看有关如何查询作用域内角色成员身份以及如何添加和删除作用域角色成员身份的信息。

## <a name="properties"></a>属性
| 属性   | 类型 | 说明 |
|:---------------|:--------|:----------|
|administrativeUnitId|string|目录角色作用域的管理单元的唯一标识符|
|id|string| 作用域角色成员身份的唯一标识符。 只读。|
|roleId|string| 成员所在目录角色的唯一标识符。|
|roleMemberInfo|[identity](identity.md)| 角色成员标识信息。 表示属于此作用域角色的成员的用户。|

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
