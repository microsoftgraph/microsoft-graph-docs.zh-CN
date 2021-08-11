---
author: JeremyKelley
title: site 资源
description: site 资源提供 Sharepoint 网站的元数据和关系。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b0ce021bbc07170879a11cab2d23a66efc45b82d9881d5157bcc9d44d34549e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126275"
---
# <a name="site-resource"></a>site 资源

命名空间：microsoft.graph

**site** 资源提供 SharePoint 网站的元数据和关系。

## <a name="methods"></a>方法

| 方法                | 返回类型 | 说明
|:-------------------------|:-------------|:----------
| [获取根网站][]        | 网站 | 访问租户内的根 SharePoint 网站。
| [获取网站][]             | 网站 | 使用 siteId 访问 SharePoint 网站。
| [根据路径获取网站][]     | 网站 | 通过相对路径访问根 SharePoint 网站。
| [获取组的网站][] | 网站 | 访问组的团队网站。
| [获取分析结果][]              | [itemAnalytics][] | 对此资源可获取分析。 
| [按间隔获取活动][] | [itemActivityStat][] | 在指定的时间间隔内获取 **itemActivityStats** 的集合。
| [搜索网站][]     | 网站集合 | 在 SharePoint 租户中搜索与所提供的关键字匹配的 网站。
| [关注网站][]          | 网站集合 | 关注用户的网站或多个网站。
| [取消关注网站][]        | 网站集合 | 关注用户的网站或多个网站。
| [关注网站列表][]  | 网站集合 | 已登录用户的关注网站列表。
| [获取权限][]             | GET /sites/{site-id}/permissions/{permission-id}
| [列出权限][]           | GET /sites/{site-id}/permissions
| [创建权限][]         | POST /sites/{site-id}/permissions
| [删除权限][]         | DELETE /sites/{site-id}/permissions/{permission-id}
| [更新权限][]         | PATCH /sites/{site-id}/permissions/{permission-id}

[获取网站]: ../api/site-get.md
[获取根网站]: ../api/site-get.md
[根据路径获取网站]: ../api/site-getbypath.md
[获取组的网站]: ../api/site-get.md
[获取分析结果]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivitystat-getactivitybyinterval.md
[搜索网站]: ../api/site-search.md
[itemActivityStat]: itemactivitystat.md
[关注网站]: ../api/site-follow.md
[取消关注网站]: ../api/site-unfollow.md
[关注网站列表]: ../api/sites-list-followed.md
[获取权限]: ../api/site-get-permission.md
[列出权限]: ../api/site-list-permissions.md
[创建权限]: ../api/site-post-permissions.md
[删除权限]: ../api/site-delete-permission.md
[更新权限]: ../api/site-update-permission.md

## <a name="properties"></a>属性

| 属性            | 类型                                | 说明                                                                                    |
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

### <a name="id-property"></a>id 属性
**site** 由一个唯一 ID 标识，此唯一 ID 由以下值组成：
* 网站集主机名称 (contoso.sharepoint.com)
* 网站集的唯一 ID (GUID)
* 网站的唯一 ID (GUID)
  
`root` 标识符经常用于引用给定目标的根网站，如下所示：

* `/sites/root`：租户根网站。
* `/groups/{group-id}/sites/root`：该组的团队网站。
  
## <a name="relationships"></a>关系

| 关系      | 类型                             | 说明
|:------------------|:---------------------------------|:----------------------
| **analytics**     | [itemAnalytics][] 资源       | 此网站上发生的查看活动的相关分析。
| **columns**       | Collection([columnDefinition][]) | 可以在此网站下方的列表中重复使用的列定义集合。
| **contentTypes**  | Collection([contentType][])      | 为此网站定义的内容类型集合。
| **drive**         | [drive][]                        | 此网站的默认驱动器（文档库）。
| **驱动器**        | 集合（[drive][]）            | 网站下方的驱动器集合（文档库）。
| **项目**         | 集合 ([baseItem][])         | 用于处理包含在此网站中的任何项目。不能枚举该集合。
| **lists**         | Collection([list][])             | 此网站下方的列表集合。
| **权限**   | 集合([权限][])         | 与网站关联的权限。空。
| **sites**         | 集合（[网站][]）             | 网站下方的子网站的集合。
| **onenote**       | [onenote][]                      | 调用 OneNote 服务执行笔记本相关操作。

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[权限]: permission.md
[网站]: site.md
[onenote]: onenote.md

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
    "permissions",
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
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "permissions": [ { "@odata.type": "microsoft.graph.permission" }],
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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
