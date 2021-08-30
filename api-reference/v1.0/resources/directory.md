---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d4a68680c62fd97229190bac921a22246e01b79f
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695292"
---
# <a name="directory-resource-type-deleted-items"></a>目录资源类型（已删除的项目）

命名空间：microsoft.graph

表示目录中已删除的项目。 删除某个项目后，它会被添加到已删除项目“容器”中。 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。

目前，仅应用程序、组和用户资源支持已删除的项目[](application.md)功能。 [](group.md) [](user.md)

继承自 [实体](entity.md)。

## <a name="methods"></a>方法

| 方法         | 返回类型 | 说明 |
|:---------------|:------------|:------------|
|[Get deleted item](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | 获取已删除项目的属性。 |
|[Restore deleted item](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| 还原最近删除的项目。 |
|[List deleted items](../api/directory-deleteditems-list.md) |[directoryObject](directoryobject.md) 集合| 获取最近删除的项目列表。 |
|[Permanently delete an item](../api/directory-deleteditems-delete.md) | 无 | 永久删除项目。 |
|[列出用户拥有的已删除项目](../api/directory-deleteditems-user-owned.md) | [directoryObject](directoryobject.md) collection | 列出用户拥有的目录项。 |


## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|String| 对象的唯一标识符;例如， `12345678-9abc-def0-1234-56789abcde` 。 键。 不可为 null。 只读。 继承自 [实体](entity.md)。|


## <a name="relationships"></a>关系

| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|administrativeUnits|[administrativeUnit](administrativeunit.md) 集合| 用户和组目录对象的概念容器。|
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
```http
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

