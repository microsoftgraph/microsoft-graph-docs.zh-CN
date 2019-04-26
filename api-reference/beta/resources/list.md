---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5e078c79603235059cbe326c850e51dfa33d2f8e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345331"
---
# <a name="list-resource"></a>List 资源

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**list** 资源表示 [site][] 中的列表。
此资源包含列表的顶级属性，其中包括模板和字段定义。

## <a name="tasks-on-a-list"></a>list 上的任务

下面列出了可执行的 list 资源任务。
**注意：** 此测试版只允许导航列表，不允许创建或更新列表。
但是，可以创建或更新[列表项][listItem]。

下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}`。

| 常见任务               | HTTP 方法
|:--------------------------|:------------------------------
| [获取列表][]              | GET /lists/{list-id}
| [枚举列表项][]  | GET /lists/{list-id}/items
| [更新列表项][]      | PATCH /lists/{list-id}/items/{item-id}
| [删除列表项][]      | DELETE /lists/{list-id}/items/{item-id}
| [创建列表项][]      | POST /lists/{list-id}
| [获取最近的活动][] | GET /lists/{list-id}/activities

[获取列表]: ../api/list-get.md
[枚举列表项]: ../api/listitem-list.md
[更新列表项]: ../api/listitem-update.md
[删除列表项]: ../api/listitem-delete.md
[创建列表项]: ../api/listitem-create.md
[获取最近的活动]: ../api/activities-list.md

## <a name="json-representation"></a>JSON 表示形式

下面是 **list** 资源的 JSON 表示形式。

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template": "documentLibrary | genericList | survey | links | announcements | contacts ..."
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
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a>属性

**list **资源具有以下属性。

| 属性名称    | 类型                             | 说明
|:-----------------|:---------------------------------|:---------------------------
| **columns**      | Collection([columnDefinition][]) | 此列表的字段定义集合。
| **contentTypes** | Collection([contentType][])      | 此列表中出现的内容类型的集合。
| **displayName**  | string                           | 列表的可显示标题。
| **list**         | [listInfo][]                     | 提供关于列表的其他详细信息。
| **system**       | [systemFacet][]                  | 如果存在，则表示这是系统管理的列表。 只读。

以下属性继承自 ** [baseItem][]**。

| 属性名称            | 类型             | 说明
|:-------------------------|:-----------------|:-------------------------------
| **id**                   | string           | 项的唯一标识符。只读。
| **名称**                 | string           | 项目名称。
| **createdBy**            | [identitySet][]  | 此项的创建者的标识。 只读。
| **createdDateTime**      | DateTimeOffset   | 创建项目的日期和时间。只读。
| **说明**          | string           | 项目的描述性文本。
| **lastModifiedBy**       | [identitySet][]  | 此项的最后一个修饰符的标识。 只读。
| **lastModifiedDateTime** | DateTimeOffset   | 上次修改项目的日期和时间。只读。
| **webUrl**               | string (url)     | 在浏览器中显示此项目的 URL。只读。

## <a name="relationships"></a>关系

**list** 资源与其他资源具有以下关系。

| 关系名称 | 类型                        | 说明
|:------------------|:----------------------------|:------------------------------
| **activities**    | [itemActivity][] 集合 | 最近发生在此列表内的活动。
| **驱动器**         | [drive][]                   | 仅存在于文档库中。 允许访问作为具有 [driveItems][driveItem] 的 [drive][] 资源的列表。
| **items**         | Collection([listItem][])    | 列表中包含的所有项。

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[site]: site.md
[systemFacet]: systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  },
  "suppressions": []
}
-->
