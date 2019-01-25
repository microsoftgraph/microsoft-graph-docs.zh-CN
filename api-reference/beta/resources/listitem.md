---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 2a405ad8a71c766642bd23adbce64c2b57b72e23
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517440"
---
# <a name="listitem-resource"></a>ListItem 资源

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

此资源表示 SharePoint **[list][]** 中的项目。
该列表中的列值可通过 `fieldValueSet` 字典获得。

## <a name="tasks-on-a-listitem"></a>listItem 上的任务

下列任务可用于 **listItem** 资源。
下面的所有示例都与**[list][]** 相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`。

| 常见任务                    | HTTP 方法
|:-------------------------------|:------------------------
| [获取][]                        | GET /items/{item-id}
| [获取列值][Get]       | GET /items/{item-id}?expand=fields
| [获取分析结果][]              | GET /items/ {项目-id} / 分析
| [按间隔获取活动][] | GET /items/ {项目-id} / getActivitiesByInterval
| [Create][]                     | POST /items
| [删除][]                     | DELETE /items/{item-id}
| [Update][]                     | PATCH /items/{item-id}
| [更新列值][Update] | PATCH /items/{item-id}/fields

[获取]: ../api/listitem-get.md
[获取分析结果]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[删除]: ../api/listitem-delete.md
[更新]: ../api/listitem-update.md

## <a name="json-representation"></a>JSON 表示形式

下面是 **listItem** 资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "url"
}
```

## <a name="properties"></a>属性

**listItem** 资源具有以下属性。

| 属性名称 | 类型                | 说明
|:--------------|:--------------------|:-------------------------------
| contentType   | [contentTypeInfo][] | 此列表项的内容类型

以下属性继承自 ** [baseItem][]**。

| 属性名称        | 类型              | 说明
|:---------------------|:------------------|:----------------------------------
| id                   | string            | 项的唯一标识符。只读。
| name                 | string            | 项目名称/标题。
| createdBy            | [identitySet][]   | 此项的创建者的标识。 只读。
| createdDateTime      | DateTimeOffset    | 创建项目的日期和时间。只读。
| 说明          | string            | 项目的描述性文本。
| eTag                 | 字符串            | 该项目的 ETag。只读。                                                          |
| lastModifiedBy       | [identitySet][]   | 此项的最后一个修饰符的标识。 只读。
| lastModifiedDateTime | DateTimeOffset    | 上次修改项目的日期和时间。只读。
| parentReference      | [itemReference][] | 父信息（如果此项具有父级）。读写。
| sharepointIds        | [sharepointIds][] | 返回对 SharePoint REST 兼容性有用的标识符。只读。
| WebUrl               | string (url)      | 在浏览器中显示此项目的 URL。只读。

## <a name="relationships"></a>关系

 **listItem** 资源与其他资源具有以下关系。

| 关系名称 | 类型                           | 说明
|:------------------|:-------------------------------|:-------------------------------
| activities        | [itemActivity][] 集合    | 最近发生在此项上的活动的列表。
| analytics         | [itemAnalytics][] 资源     | 有关此项发生查看活动的分析。
| driveItem         | [driveItem][]                  | 对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。
| fields            | [fieldValueSet][]              | 在此列表项上设置的列的值。
| 版本          | [listItemVersion][]集合 | 早期版本的列表项的列表。

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/listitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
