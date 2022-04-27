---
author: JeremyKelley
description: 网站资源提供 SharePoint 网站的元数据和关系。
title: site 资源类型
ms.localizationpriority: high
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 423986ac43de3558836660a1684978784db724eb
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65059968"
---
# <a name="site-resource-type"></a>site 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**site** 资源提供 SharePoint 网站的元数据和关系。

## <a name="methods"></a>方法

| 方法                                            | REST 路径                                                   |
| :------------------------------------------------ | :---------------------------------------------------------- |
| [获取根网站][]                                 | GET /sites/root                                             |
| [获取网站][]                                      | GET /sites/{site-id}                                        |
| [根据路径获取网站][]                              | GET /sites/{hostname}:/{site-path}                          |
| [获取组的网站][]                          | GET /groups/{group-id}/sites/root                           |
| [获取分析结果][]                                 | GET /sites/{site-id}/analytics                              |
| [按间隔获取活动][]                    | GET /sites/{site-id}/getActivitiesByInterval                |
| [列出页面][]                                    | GET /sites/{site-id}/pages                                  |
| [列出根网站][]                               | GET /sites?filter=root ne null&select=siteCollection,webUrl |
| [搜索网站][]                              | GET /sites?search={query}                                   |
| [关注网站][]                                   | POST /users/{user-id}/followedSites/add                     |
| [取消关注网站][]                                 | POST /users/{user-id}/followedSites/remove                  |
| [关注网站列表][]                           | GET /me/followedSites                                       |
| [获取权限][]                                | GET /sites/{site-id}/permissions/{permission-id}            |
| [列出权限][]                              | GET /sites/{site-id}/permissions                            |
| [创建权限][]                            | POST /sites/{site-id}/permissions                           |
| [删除权限][]                             | DELETE /sites/{site-id}/permissions/{permission-id}         |
| [更新权限][]                             | PATCH /sites/{site-id}/permissions/{permission-id}          |
| [列表内容类型][]                            | GET /sites/{site-id}/contentTypes                           |
| [创建 contentType][]                            | POST/sites/{site-id}/contentTypes                          |
| [List columns][]                                  | 获取 /sites/{site-id}/columns                                |
| [创建列][]                                 | 发布 /sites/{site-id}/columns                               |
| [列举操作](../api/site-list-operations.md) | GET /sites/{site-id}/operations                             |
| [获取网站设置][]                             | GET /sites/{site-id}/settings                               |

[获取网站]: ../api/site-get.md
[获取根网站]: ../api/site-get.md
[根据路径获取网站]: ../api/site-getbypath.md
[获取组的网站]: ../api/site-get.md
[获取分析结果]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivity-getbyinterval.md
[列出页面]: ../api/sitepage-list.md
[列出根网站]: ../api/site-list.md
[搜索网站]: ../api/site-search.md
[关注网站]: ../api/site-follow.md
[取消关注网站]: ../api/site-unfollow.md
[关注网站列表]: ../api/sites-list-followed.md
[获取权限]: ../api/site-get-permission.md
[列出权限]: ../api/site-list-permissions.md
[创建权限]: ../api/site-post-permissions.md
[删除权限]: ../api/site-delete-permission.md
[更新权限]: ../api/site-update-permission.md
[列表内容类型]: ../api/site-list-contenttypes.md
[创建 contentType]: ../api/site-post-contenttypes.md
[List columns]: ../api/site-list-columns.md
[创建列]: ../api/site-post-columns.md
[获取网站设置]: ../api/sitesettings-get.md

## <a name="properties"></a>属性

| 属性                 | 类型               | 说明                                                                                    |
| :----------------------- | :----------------- | :--------------------------------------------------------------------------------------------- |
| **id**                   | string             | 项的[唯一标识符](#id-property)。只读。                                  |
| **createdDateTime**      | DateTimeOffset     | 创建项目的日期和时间。只读。                                             |
| **说明**          | string             | 网站的描述性文本。                                                             |
| **eTag**                 | string             | 该项目的 ETag。只读。                                                                  |
| **displayName**          | string             | 网站的完整标题。只读。                                                        |
| **lastModifiedDateTime** | DateTimeOffset     | 上次修改项目的日期和时间。只读。                                       |
| **name**                 | string             | 项目名称/标题。                                                                  |
| **根**                 | [根][]           | 如果存在，则表示这是网站集中的根网站。只读。            |
| **设置**             | [siteSettings]     | 此网站上的设置。 只读。                                |
| **sharepointIds**        | [sharepointIds][]  | 返回对 SharePoint REST 兼容性有用的标识符。只读。                       |
| **siteCollection**       | [siteCollection][] | 提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。 |
| **webUrl**               | string (url)       | 在浏览器中显示此项目的 URL。只读。                                          |

### <a name="id-property"></a>id 属性

**site** 由一个唯一 ID 标识，此唯一 ID 由以下值组成：
* 网站集主机名称 (contoso.sharepoint.com)
* 网站集的唯一 ID (GUID)
* 网站的唯一 ID (GUID)

`root` 标识符经常用于引用给定目标的根网站，如下所示：

* `/sites/root`：租户根网站。
* `/groups/{group-id}/sites/root`：该组的团队网站。

## <a name="relationships"></a>关系

| 关系        | 类型                                                                            | 说明                                                                                                                                |
| :------------------ | :------------------------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------- |
| **analytics**       | [itemAnalytics][] 资源                                                      | 此网站上发生的查看活动的相关分析。                                                                          |
| **columns**         | Collection([columnDefinition][])                                                | 可以在此网站下方的列表中重复使用的列定义集合。                                                                |
| **contentTypes**    | Collection([contentType][])                                                     | 为此网站定义的内容类型集合。                                                                                     |
| **drive**           | [drive][]                                                                       | 此网站的默认驱动器（文档库）。                                                                                        |
| **驱动器**          | 集合（[drive][]）                                                           | 网站下方的驱动器集合（文档库）。                                                                             |
| **项目**           | 集合 ([baseItem][])                                                        | 用于处理包含在此网站中的任何项目。不能枚举该集合。                                                     |
| **lists**           | Collection([list][])                                                            | 此网站下的列表集合。                                                                                                   |
| **operations**      | [richLongRunningOperation](../resources/richlongrunningoperation.md) 集合 | 站点长时间运行操作的集合。                                                                                    |
| **pages**           | Collection([sitePage][])                                                        | 此网站的 SitePages 列表中的页面集合。                                                                                |
| **权限**     | 集合([权限][])                                                      | 与网站关联的权限。空。                                                                                        |
| **sites**           | 集合（[网站][]）                                                            | 网站下方的子网站的集合。                                                                                           |
| **termStore**       | [microsoft.graph.termStore.store]                                               | 此站点下的术语库。                                                                                                             |
| **externalColumns** | 集合（[columnDefinition][]）                                                | 网站中可用列定义的集合，从当前网站的父层次结构中的网站引用。 |

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[permission]: permission.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[siteSettings]: sitesettings.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md
[microsoft.graph.termStore.store]: termstore-store.md

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

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
  "displayName": "string",
  "id": "string",
  "root": { "@odata.type": "microsoft.graph.root" },
  "settings": { "@odata.type": "microsoft.graph.sitesettings" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "siteCollection": {"@odata.type": "microsoft.graph.siteCollection"},

  /* relationships */
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "externalColumns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "permissions": [ { "@odata.type": "microsoft.graph.permission" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "termStore": { "@odata.type": "microsoft.graph.termStore.store" },

  /* inherited from baseItem */
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "webUrl": "url"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": {
    "Resources/Site": "#"
  },
  "suppressions": []
}
-->
