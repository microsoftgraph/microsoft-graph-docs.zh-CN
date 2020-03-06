---
author: JeremyKelley
description: 网站资源提供 SharePoint 网站的元数据和关系。
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: be567e1ba44790c54127ccee17dbb0d396f15e0c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520553"
---
# <a name="site-resource-type"></a><span data-ttu-id="df80d-103">site 资源类型</span><span class="sxs-lookup"><span data-stu-id="df80d-103">site resource type</span></span>

<span data-ttu-id="df80d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df80d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df80d-105">**site** 资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="df80d-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="df80d-106">方法</span><span class="sxs-lookup"><span data-stu-id="df80d-106">Methods</span></span>

| <span data-ttu-id="df80d-107">方法</span><span class="sxs-lookup"><span data-stu-id="df80d-107">Method</span></span>                         | <span data-ttu-id="df80d-108">REST 路径</span><span class="sxs-lookup"><span data-stu-id="df80d-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="df80d-109">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="df80d-109">[Get root site][]</span></span>              | <span data-ttu-id="df80d-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="df80d-110">GET /sites/root</span></span>
| <span data-ttu-id="df80d-111">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="df80d-111">[Get site][]</span></span>                   | <span data-ttu-id="df80d-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="df80d-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="df80d-113">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="df80d-113">[Get site by path][]</span></span>           | <span data-ttu-id="df80d-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="df80d-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="df80d-115">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="df80d-115">[Get site for a group][]</span></span>       | <span data-ttu-id="df80d-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="df80d-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="df80d-117">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="df80d-117">[Get analytics][]</span></span>              | <span data-ttu-id="df80d-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="df80d-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="df80d-119">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="df80d-119">[Get activities by interval][]</span></span> | <span data-ttu-id="df80d-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="df80d-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="df80d-121">[列出页面][]</span><span class="sxs-lookup"><span data-stu-id="df80d-121">[List pages][]</span></span>                 | <span data-ttu-id="df80d-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="df80d-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="df80d-123">[列出根网站][]</span><span class="sxs-lookup"><span data-stu-id="df80d-123">[List root sites][]</span></span>            | <span data-ttu-id="df80d-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="df80d-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="df80d-125">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="df80d-125">[Search for sites][]</span></span>           | <span data-ttu-id="df80d-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="df80d-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="df80d-127">[关注网站][]</span><span class="sxs-lookup"><span data-stu-id="df80d-127">[Follow Site][]</span></span>                | <span data-ttu-id="df80d-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="df80d-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="df80d-129">[取消关注网站][]</span><span class="sxs-lookup"><span data-stu-id="df80d-129">[Unfollow Site][]</span></span>              | <span data-ttu-id="df80d-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="df80d-130">POST /users/{user-id}/followedSites/remove</span></span>

[获取网站]: ../api/site-get.md
[Get site]: ../api/site-get.md
[获取根网站]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[根据路径获取网站]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[获取组的网站]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[获取分析结果]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[列出页面]: ../api/sitepage-list.md
[List pages]: ../api/sitepage-list.md
[列出根网站]: ../api/site-list.md
[List root sites]: ../api/site-list.md
[搜索网站]: ../api/site-search.md
[Search for sites]: ../api/site-search.md
[关注网站]: ../api/site-follow.md
[Follow site]: ../api/site-follow.md
[取消关注网站]: ../api/site-unfollow.md
[Unfollow site]: ../api/site-unfollow.md


## <a name="properties"></a><span data-ttu-id="df80d-142">属性</span><span class="sxs-lookup"><span data-stu-id="df80d-142">Properties</span></span>

| <span data-ttu-id="df80d-143">属性名称</span><span class="sxs-lookup"><span data-stu-id="df80d-143">Property name</span></span>            | <span data-ttu-id="df80d-144">类型</span><span class="sxs-lookup"><span data-stu-id="df80d-144">Type</span></span>               | <span data-ttu-id="df80d-145">说明</span><span class="sxs-lookup"><span data-stu-id="df80d-145">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="df80d-146">**id**</span><span class="sxs-lookup"><span data-stu-id="df80d-146">**id**</span></span>                   | <span data-ttu-id="df80d-147">string</span><span class="sxs-lookup"><span data-stu-id="df80d-147">string</span></span>             | <span data-ttu-id="df80d-148">项的[唯一标识符](#id-property)。</span><span class="sxs-lookup"><span data-stu-id="df80d-148">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="df80d-149">只读。</span><span class="sxs-lookup"><span data-stu-id="df80d-149">Read-only.</span></span>
| <span data-ttu-id="df80d-150">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="df80d-150">**createdDateTime**</span></span>      | <span data-ttu-id="df80d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df80d-151">DateTimeOffset</span></span>     | <span data-ttu-id="df80d-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="df80d-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="df80d-154">**说明**</span><span class="sxs-lookup"><span data-stu-id="df80d-154">**description**</span></span>          | <span data-ttu-id="df80d-155">string</span><span class="sxs-lookup"><span data-stu-id="df80d-155">string</span></span>             | <span data-ttu-id="df80d-156">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="df80d-156">The descriptive text for the site.</span></span>
| <span data-ttu-id="df80d-157">**eTag**</span><span class="sxs-lookup"><span data-stu-id="df80d-157">**eTag**</span></span>                 | <span data-ttu-id="df80d-158">string</span><span class="sxs-lookup"><span data-stu-id="df80d-158">string</span></span>             | <span data-ttu-id="df80d-p103">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="df80d-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="df80d-161">**displayName**</span><span class="sxs-lookup"><span data-stu-id="df80d-161">**displayName**</span></span>          | <span data-ttu-id="df80d-162">string</span><span class="sxs-lookup"><span data-stu-id="df80d-162">string</span></span>             | <span data-ttu-id="df80d-p104">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="df80d-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="df80d-165">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="df80d-165">**lastModifiedDateTime**</span></span> | <span data-ttu-id="df80d-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df80d-166">DateTimeOffset</span></span>     | <span data-ttu-id="df80d-p105">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="df80d-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="df80d-169">**name**</span><span class="sxs-lookup"><span data-stu-id="df80d-169">**name**</span></span>                 | <span data-ttu-id="df80d-170">string</span><span class="sxs-lookup"><span data-stu-id="df80d-170">string</span></span>             | <span data-ttu-id="df80d-171">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="df80d-171">The name / title of the item.</span></span>
| <span data-ttu-id="df80d-172">**根**</span><span class="sxs-lookup"><span data-stu-id="df80d-172">**root**</span></span>                 | <span data-ttu-id="df80d-173">[根][]</span><span class="sxs-lookup"><span data-stu-id="df80d-173">[root][]</span></span>           | <span data-ttu-id="df80d-p106">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="df80d-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="df80d-176">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="df80d-176">**sharepointIds**</span></span>        | <span data-ttu-id="df80d-177">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="df80d-177">[sharepointIds][]</span></span>  | <span data-ttu-id="df80d-p107">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="df80d-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="df80d-180">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="df80d-180">**siteCollection**</span></span>       | <span data-ttu-id="df80d-181">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="df80d-181">[siteCollection][]</span></span> | <span data-ttu-id="df80d-p108">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="df80d-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="df80d-185">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="df80d-185">**webUrl**</span></span>               | <span data-ttu-id="df80d-186">string (url)</span><span class="sxs-lookup"><span data-stu-id="df80d-186">string (url)</span></span>       | <span data-ttu-id="df80d-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="df80d-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="df80d-189">id 属性</span><span class="sxs-lookup"><span data-stu-id="df80d-189">id property</span></span>
<span data-ttu-id="df80d-190">**site** 由一个唯一 ID 标识，此唯一 ID 由以下值组成：</span><span class="sxs-lookup"><span data-stu-id="df80d-190">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="df80d-191">网站集主机名称 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="df80d-191">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="df80d-192">网站集的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="df80d-192">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="df80d-193">网站的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="df80d-193">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="df80d-194">`root` 标识符经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="df80d-194">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="df80d-195">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="df80d-195">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="df80d-196">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="df80d-196">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="df80d-197">关系</span><span class="sxs-lookup"><span data-stu-id="df80d-197">Relationships</span></span>

| <span data-ttu-id="df80d-198">关系名称</span><span class="sxs-lookup"><span data-stu-id="df80d-198">Relationship name</span></span> | <span data-ttu-id="df80d-199">类型</span><span class="sxs-lookup"><span data-stu-id="df80d-199">Type</span></span>                             | <span data-ttu-id="df80d-200">说明</span><span class="sxs-lookup"><span data-stu-id="df80d-200">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="df80d-201">**analytics**</span><span class="sxs-lookup"><span data-stu-id="df80d-201">**analytics**</span></span>     | <span data-ttu-id="df80d-202">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="df80d-202">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="df80d-203">此网站上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="df80d-203">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="df80d-204">**columns**</span><span class="sxs-lookup"><span data-stu-id="df80d-204">**columns**</span></span>       | <span data-ttu-id="df80d-205">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="df80d-205">Collection([columnDefinition][])</span></span> | <span data-ttu-id="df80d-206">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="df80d-206">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="df80d-207">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="df80d-207">**contentTypes**</span></span>  | <span data-ttu-id="df80d-208">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="df80d-208">Collection([contentType][])</span></span>      | <span data-ttu-id="df80d-209">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="df80d-209">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="df80d-210">**drive**</span><span class="sxs-lookup"><span data-stu-id="df80d-210">**drive**</span></span>         | <span data-ttu-id="df80d-211">[drive][]</span><span class="sxs-lookup"><span data-stu-id="df80d-211">[drive][]</span></span>                        | <span data-ttu-id="df80d-212">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="df80d-212">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="df80d-213">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="df80d-213">**drives**</span></span>        | <span data-ttu-id="df80d-214">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="df80d-214">Collection([drive][])</span></span>            | <span data-ttu-id="df80d-215">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="df80d-215">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="df80d-216">**项目**</span><span class="sxs-lookup"><span data-stu-id="df80d-216">**items**</span></span>         | <span data-ttu-id="df80d-217">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="df80d-217">Collection([baseItem][])</span></span>         | <span data-ttu-id="df80d-p110">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="df80d-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="df80d-220">**lists**</span><span class="sxs-lookup"><span data-stu-id="df80d-220">**lists**</span></span>         | <span data-ttu-id="df80d-221">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="df80d-221">Collection([list][])</span></span>             | <span data-ttu-id="df80d-222">此网站下的列表集合。</span><span class="sxs-lookup"><span data-stu-id="df80d-222">The collection of lists under this site.</span></span>
| <span data-ttu-id="df80d-223">**pages**</span><span class="sxs-lookup"><span data-stu-id="df80d-223">**pages**</span></span>         | <span data-ttu-id="df80d-224">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="df80d-224">Collection([sitePage][])</span></span>         | <span data-ttu-id="df80d-225">此网站的 SitePages 列表中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="df80d-225">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="df80d-226">**sites**</span><span class="sxs-lookup"><span data-stu-id="df80d-226">**sites**</span></span>         | <span data-ttu-id="df80d-227">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="df80d-227">Collection([site][])</span></span>             | <span data-ttu-id="df80d-228">网站下的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="df80d-228">The collection of the sub-sites under this site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="df80d-240">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df80d-240">JSON representation</span></span>

<span data-ttu-id="df80d-241">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df80d-241">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="df80d-242">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="df80d-242">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" }],
  "items": [ { "@odata.type": "microsoft.graph.baseItem" }],
  "lists": [ { "@odata.type": "microsoft.graph.list" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
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
