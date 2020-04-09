---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 739fb380a6686bd6e68694be88c91df548972890
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181879"
---
# <a name="directory-resource-type-deleted-items"></a>目录资源类型（已删除的项目）

命名空间：microsoft.graph

表示目录中已删除的项目。 删除某个项目后，它会被添加到已删除项目“容器”中。 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。

目前，仅支持[应用程序](application.md)、[组](group.md)和[用户](user.md)资源的 "已删除邮件" 功能。

## <a name="methods"></a>方法

| 方法         | 返回类型 | 说明 |
|:---------------|:------------|:------------|
|[Get deleted item](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | 获取已删除项目的属性。 |
|[Restore deleted item](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| 还原最近删除的项目。 |
|[List deleted items](../api/directory-deleteditems-list.md) |[directoryObject](directoryobject.md) 集合| 获取最近删除的项目列表。 |
|[Permanently delete an item](../api/directory-deleteditems-delete.md) | 无 | 永久删除项目。 |
|[列出用户拥有的已删除项目](../api/directory-deleteditems-user-owned.md) | [directoryObject](directoryobject.md) collection | 列出用户拥有的目录项。 |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|deletedItems|[directoryObject](directoryobject.md) 集合| 最近删除的项目。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
}
```

## <a name="example"></a>示例

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/directory
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.directory"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
