---
title: directoryObject 资源类型
description: 表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。
localization_priority: Priority
ms.openlocfilehash: a03ec966f966df556ab0122958b0b8f5464cf4fc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889717"
---
# <a name="directoryobject-resource-type"></a>directoryObject 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示 Azure Active Directory 对象。**directoryObject** 类型是其他许多目录实体类型的基类型。

该资源支持：

- 通过提供 [delta](../api/directoryobject-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 directoryObject](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |读取 directory 对象的属性。|
|[删除](../api/directoryobject-delete.md) | 无 |删除 directory 对象。 |
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|String collection|检查组列表中的成员身份。检查是可传递的。|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|String collection|返回 user、group 或 directory 对象所属的所有组。检查是可传递的。|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|String collection| 返回 user、group 或 directory 对象所属的所有组和目录角色。检查是可传递的。 |
|[getByIds](../api/directoryobject-getbyids.md) | [directoryObject](directoryobject.md) 集合 | 基于提供的 ID 集获取目录对象集。 |
|[validateProperties](../api/directoryobject-validateproperties.md)|JSON| 验证 Office 365 组的显示名称或邮件昵称符合命名策略。 |
|[delta](../api/directoryobject-delta.md)|directoryObject 集合| 获得目录对象的增量更改。 按 derrived 类型筛选的支持。 |

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|字符串|Guid 对象; 的唯一标识符例如，12345678-9abc-def0-1234年-56789abcde12。 键。 不可为 null。 只读。|

## <a name="relationships"></a>Relationships

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObject"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
