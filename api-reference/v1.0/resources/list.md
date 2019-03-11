---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: List
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 7946346c5b872cad80eb3b8dc50109862ac15b8e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481403"
---
# <a name="list-resource"></a>List 资源

**list** 资源表示 [site][] 中的列表。
此资源包含列表的顶级属性，其中包括模板和字段定义。

## <a name="tasks-on-a-list"></a>list 上的任务

下面列出了可执行的 list 资源任务。
**注意：** 此测试版只允许导航列表，不允许创建或更新列表。
但是，可以创建或更新[列表项][listItem]。

下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/v1.0/sites/{site-id}`。

| 常见任务               | HTTP 方法
|:--------------------------|:------------------------------
| [获取列表][]              | GET /lists/{list-id}
| [枚举列表项][]  | GET /lists/{list-id}/items
| [更新列表项][]      | PATCH /lists/{list-id}/items/{item-id}
| [删除列表项][]      | DELETE /lists/{list-id}/items/{item-id}
| [创建列表项][]      | POST /lists/{list-id}

[获取列表]: ../api/list-get.md
[枚举列表项]: ../api/listitem-list.md
[更新列表项]: ../api/listitem-update.md
[删除列表项]: ../api/listitem-delete.md
[创建列表项]: ../api/listitem-create.md

## <a name="json-representation"></a>JSON 表示形式

下面是 **list** 资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "items",
    "drive"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.list"
}-->

```json
{
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template": "documentLibrary | genericList | survey | links | announcements | contacts | accessRequest ..."
  },
  "system": false,

  /* inherited from baseItem */
  "id": "string",
  "name": "name of list",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of list",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a>属性

**list **资源具有以下属性。

| 属性名称    | 类型                             | 说明
|:-----------------|:---------------------------------|:---------------------------
| **displayName**  | string                           | 列表的可显示标题。
| **list**         | [listInfo][]                     | 提供关于列表的其他详细信息。
| **system**       | [systemFacet][]                  | 如果存在，则表示这是系统管理的列表。 只读。

以下属性继承自 ** [baseItem][]**。

| 属性名称            | 类型              | 说明
|:-------------------------|:------------------|:------------------------------
| **id**                   | string            | 项的唯一标识符。只读。
| **名称**                 | string            | 项目名称。
| **createdBy**            | [identitySet][]   | 此项的创建者的标识。 只读。
| **createdDateTime**      | DateTimeOffset    | 创建项目的日期和时间。只读。
| **说明**          | string            | 项目的描述性文本。
| **eTag**                 | string            | 该项目的 ETag。只读。                                                          |
| **lastModifiedBy**       | [identitySet][]   | 此项的最后一个修饰符的标识。 只读。
| **lastModifiedDateTime** | DateTimeOffset    | 上次修改项目的日期和时间。只读。
| **parentReference**      | [itemReference][] | 父信息（如果此项具有父级）。读写。
| **sharepointIds**        | [sharepointIds][] | 返回对 SharePoint REST 兼容性有用的标识符。只读。
| **webUrl**               | string (url)      | 在浏览器中显示此项目的 URL。只读。

## <a name="relationships"></a>关系

**list** 资源与其他资源具有以下关系。

| 关系名称 | 类型                             | 说明
|:------------------|:---------------------------------|:----------------------
| **驱动器**         | [drive][]                        | 仅存在于文档库中。 允许访问作为具有 [driveItems][driveItem] 的 [drive][] 资源的列表。
| **items**         | Collection([listItem][])         | 列表中包含的所有项。
| **columns**       | Collection([columnDefinition][]) | 此列表的字段定义集合。
| **contentTypes**  | Collection([contentType][])      | 此列表中出现的内容类型的集合。

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[sharepointIds]: sharepointids.md
[site]: site.md
[systemFacet]: systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  }
} -->
