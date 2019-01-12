---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: cd0631d8426dffa6ea731fabe024a1028e080f1c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937010"
---
# <a name="site-resource"></a>Site 资源

**网站**资源提供 SharePoint 网站的元数据和关系。

## <a name="tasks"></a>任务

下面的所有示例都相对于 `https://graph.microsoft.com/v1.0`。

| 任务名称                | 示例请求
|:-------------------------|:--------------------------------------------------
| [获取根网站][]        | GET /sites/root
| [获取网站][]             | GET /sites/{site-id}
| [根据路径获取网站][]     | GET /sites/{hostname}:/{site-path}
| [获取组的网站][] | GET /groups/{group-id}/sites/root
| [搜索网站][]     | GET /sites?search={query}

[获取网站]: ../api/site-get.md
[获取根网站]: ../api/site-get.md
[根据路径获取网站]: ../api/site-getbypath.md
[获取组的网站]: ../api/site-get.md
[搜索网站]: ../api/site-search.md

## <a name="json-representation"></a>JSON 表示形式

下面是 **site** 资源的 JSON 表示形式。

**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "sites"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.site"
}-->

```json
{
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},
  "displayName": "string",

  /* relationships */
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "onenote": { "@odata.type": "microsoft.graph.onenote"},

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

## <a name="properties"></a>属性

| 属性名称            | 类型                                | 说明                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| **id**                   | string                              | 项的唯一标识符。只读。                                                  |
| **createdDateTime**      | DateTimeOffset                      | 创建项目的日期和时间。只读。                                             |
| **说明**          | string                              | 网站的描述性文本。                                                             |
| **displayName**          | string                              | 网站的完整标题。只读。                                                        |
| **eTag**                 | string                              | 该项目的 ETag。只读。                                                                  |
| **lastModifiedDateTime** | DateTimeOffset                      | 上次修改项目的日期和时间。只读。                                       |
| **name**                 | string                              | 项目名称/标题。                                                                  |
| **根**                 | [根](root.md)                     | 如果存在，则表示这是网站集中的根网站。只读。            |
| **sharepointIds**        | [sharepointIds](sharepointids.md)   | 返回对 SharePoint REST 兼容性有用的标识符。只读。                       |
| **siteCollection**       | [siteCollection](sitecollection.md) | 提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。 |
| **webUrl**               | string (url)                        | 在浏览器中显示此项目的 URL。只读。                                          |

## <a name="relationships"></a>关系

| 关系名称 | 类型                             | 说明
|:------------------|:---------------------------------|:----------------------
| **columns**       | Collection([columnDefinition][]) | 可以在此网站下方的列表中重复使用的列定义集合。
| **contentTypes**  | Collection([contentType][])      | 为此网站定义的内容类型集合。
| **drive**         | [驱动器][]                        | 此网站的默认驱动器（文档库）。
| **驱动器**        | 集合（[drive][]）            | 网站下方的驱动器集合（文档库）。
| **项目**         | 集合 ([baseItem][])         | 用于处理包含在此网站中的任何项目。不能枚举该集合。
| **lists**         | Collection([list][])             | 此网站下方的列表集合。
| **sites**         | 集合（[网站][]）             | 网站下方的子网站的集合。
| **onenote**       | [onenote][]                      | 调用 OneNote 服务执行笔记本相关操作。

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[list]: list.md
[site]: site.md
[onenote]: onenote.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
