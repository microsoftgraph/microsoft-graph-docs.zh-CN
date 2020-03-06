---
title: directoryObject 资源类型
description: 表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b90e81a9337cef51af4bfded50eaaf494e4ebca7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507028"
---
# <a name="directoryobject-resource-type"></a>directoryObject 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。

该资源支持：

- 通过提供 [delta](../api/directoryobject-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 directoryObject](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |读取 directory 对象的属性。|
|[删除](../api/directoryobject-delete.md) | 无 |删除 directory 对象。 |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|String collection|检查组列表中的成员身份。检查是可传递的。|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|String collection|返回 user、group 或 directory 对象所属的所有组。检查是可传递的。|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|String collection| 返回 user、group 或 directory 对象所属的所有组和目录角色。检查是可传递的。 |
|[getByIds](../api/directoryobject-getbyids.md) | [directoryObject](directoryobject.md) 集合 | 基于提供的 ID 集获取目录对象集。 |
|[validateProperties](../api/directoryobject-validateproperties.md)|Json| 验证 Office 365 组的显示名称或邮件别名是否符合命名策略。 |
|[delta](../api/directoryobject-delta.md)|[directoryObject](directoryobject.md) collection| 获取目录对象的增量更改。 支持按派生类型筛选。 |

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|String|用作此对象的唯一标识符的 Guid；例如，12345678-9abc-def0-1234-56789abcde12。 密钥。 不可为 null。 只读。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject",
  "openType": true
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
