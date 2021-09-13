---
title: 目录资源类型（已删除的项目）
description: . 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9f337a8a516dbd1bc3bd772a52f74000d412c071
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59072552"
---
# <a name="directory-resource-type"></a>目录资源类型

命名空间：microsoft.graph

表示目录中已删除的项目。 删除某个项目后，它会被添加到已删除项目“容器”中。 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。

目前，仅应用程序、组和用户资源支持[已删除项目功能](user.md)。 [](group.md) [](application.md)

继承自 [实体](entity.md)。

## <a name="methods"></a>方法

| 方法         | 返回类型 | 说明 |
|:---------------|:------------|:------------|
|[Get deleted item](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | 获取已删除项目的属性。 |
|[Restore deleted item](../api/directory-deleteditems-restore.md) |[directoryObject](directoryobject.md)| 还原最近删除的项目。 |
|[List deleted items](../api/directory-deleteditems-list.md) |[directoryObject](directoryobject.md) 集合| 获取最近删除的项目列表。 |
|[Permanently delete an item](../api/directory-deleteditems-delete.md) | 无 | 永久删除项目。 |
|[列出用户拥有的已删除项目](../api/directory-deleteditems-user-owned.md) | [directoryObject](directoryobject.md) 集合 | 列出用户拥有的目录项。 |


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
  "keyProperty":"id",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "@odata.type": "#microsoft.graph.directory"
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

