---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: f2386228c3758cc15d9c270f0da32608e4f2b901
ms.sourcegitcommit: 895a03cb2706a9b3a2236b30d6a7e9f5cbc6a89e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34683501"
---
# <a name="site-resource-type"></a><span data-ttu-id="e22dc-102">site 资源类型</span><span class="sxs-lookup"><span data-stu-id="e22dc-102">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e22dc-103">**site** 资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="e22dc-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="e22dc-104">方法</span><span class="sxs-lookup"><span data-stu-id="e22dc-104">Methods</span></span>

| <span data-ttu-id="e22dc-105">方法</span><span class="sxs-lookup"><span data-stu-id="e22dc-105">Method</span></span>                         | <span data-ttu-id="e22dc-106">REST 路径</span><span class="sxs-lookup"><span data-stu-id="e22dc-106">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="e22dc-107">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-107">[Get root site][]</span></span>              | <span data-ttu-id="e22dc-108">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="e22dc-108">GET /sites/root</span></span>
| <span data-ttu-id="e22dc-109">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-109">[Get site][]</span></span>                   | <span data-ttu-id="e22dc-110">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="e22dc-110">GET /sites/{site-id}</span></span>
| <span data-ttu-id="e22dc-111">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-111">[Get site by path][]</span></span>           | <span data-ttu-id="e22dc-112">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="e22dc-112">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="e22dc-113">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-113">[Get site for a group][]</span></span>       | <span data-ttu-id="e22dc-114">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="e22dc-114">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="e22dc-115">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-115">[Get analytics][]</span></span>              | <span data-ttu-id="e22dc-116">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="e22dc-116">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="e22dc-117">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-117">[Get activities by interval][]</span></span> | <span data-ttu-id="e22dc-118">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="e22dc-118">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="e22dc-119">[列出页面][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-119">[List pages][]</span></span>                 | <span data-ttu-id="e22dc-120">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="e22dc-120">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="e22dc-121">[列出根网站][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-121">[List root sites][]</span></span>            | <span data-ttu-id="e22dc-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="e22dc-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="e22dc-123">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-123">[Search for sites][]</span></span>           | <span data-ttu-id="e22dc-124">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="e22dc-124">GET /sites?search={query}</span></span>
| <span data-ttu-id="e22dc-125">[关注网站][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-125">[Follow Site][]</span></span>                | <span data-ttu-id="e22dc-126">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="e22dc-126">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="e22dc-127">[取消关注网站][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-127">[Unfollow Site][]</span></span>              | <span data-ttu-id="e22dc-128">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="e22dc-128">POST /users/{user-id}/followedSites/remove</span></span>

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


## <a name="properties"></a><span data-ttu-id="e22dc-140">属性</span><span class="sxs-lookup"><span data-stu-id="e22dc-140">Properties</span></span>

| <span data-ttu-id="e22dc-141">属性名称</span><span class="sxs-lookup"><span data-stu-id="e22dc-141">Property name</span></span>            | <span data-ttu-id="e22dc-142">类型</span><span class="sxs-lookup"><span data-stu-id="e22dc-142">Type</span></span>               | <span data-ttu-id="e22dc-143">说明</span><span class="sxs-lookup"><span data-stu-id="e22dc-143">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="e22dc-144">**id**</span><span class="sxs-lookup"><span data-stu-id="e22dc-144">**id**</span></span>                   | <span data-ttu-id="e22dc-145">string</span><span class="sxs-lookup"><span data-stu-id="e22dc-145">string</span></span>             | <span data-ttu-id="e22dc-146">项的[唯一标识符](#id-property)。</span><span class="sxs-lookup"><span data-stu-id="e22dc-146">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="e22dc-147">只读。</span><span class="sxs-lookup"><span data-stu-id="e22dc-147">Read-only.</span></span>
| <span data-ttu-id="e22dc-148">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="e22dc-148">**createdDateTime**</span></span>      | <span data-ttu-id="e22dc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e22dc-149">DateTimeOffset</span></span>     | <span data-ttu-id="e22dc-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="e22dc-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="e22dc-152">**说明**</span><span class="sxs-lookup"><span data-stu-id="e22dc-152">**description**</span></span>          | <span data-ttu-id="e22dc-153">string</span><span class="sxs-lookup"><span data-stu-id="e22dc-153">string</span></span>             | <span data-ttu-id="e22dc-154">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="e22dc-154">The descriptive text for the site.</span></span>
| <span data-ttu-id="e22dc-155">**eTag**</span><span class="sxs-lookup"><span data-stu-id="e22dc-155">**eTag**</span></span>                 | <span data-ttu-id="e22dc-156">string</span><span class="sxs-lookup"><span data-stu-id="e22dc-156">string</span></span>             | <span data-ttu-id="e22dc-p103">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="e22dc-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="e22dc-159">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e22dc-159">**displayName**</span></span>          | <span data-ttu-id="e22dc-160">string</span><span class="sxs-lookup"><span data-stu-id="e22dc-160">string</span></span>             | <span data-ttu-id="e22dc-p104">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="e22dc-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="e22dc-163">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e22dc-163">**lastModifiedDateTime**</span></span> | <span data-ttu-id="e22dc-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e22dc-164">DateTimeOffset</span></span>     | <span data-ttu-id="e22dc-p105">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="e22dc-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="e22dc-167">**name**</span><span class="sxs-lookup"><span data-stu-id="e22dc-167">**name**</span></span>                 | <span data-ttu-id="e22dc-168">string</span><span class="sxs-lookup"><span data-stu-id="e22dc-168">string</span></span>             | <span data-ttu-id="e22dc-169">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="e22dc-169">The name / title of the item.</span></span>
| <span data-ttu-id="e22dc-170">**根**</span><span class="sxs-lookup"><span data-stu-id="e22dc-170">**root**</span></span>                 | <span data-ttu-id="e22dc-171">[根][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-171">[root][]</span></span>           | <span data-ttu-id="e22dc-p106">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="e22dc-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="e22dc-174">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="e22dc-174">**sharepointIds**</span></span>        | <span data-ttu-id="e22dc-175">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-175">[sharepointIds][]</span></span>  | <span data-ttu-id="e22dc-p107">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="e22dc-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="e22dc-178">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="e22dc-178">**siteCollection**</span></span>       | <span data-ttu-id="e22dc-179">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-179">[siteCollection][]</span></span> | <span data-ttu-id="e22dc-p108">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="e22dc-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="e22dc-183">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="e22dc-183">**webUrl**</span></span>               | <span data-ttu-id="e22dc-184">string (url)</span><span class="sxs-lookup"><span data-stu-id="e22dc-184">string (url)</span></span>       | <span data-ttu-id="e22dc-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="e22dc-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="e22dc-187">id 属性</span><span class="sxs-lookup"><span data-stu-id="e22dc-187">id property</span></span>
<span data-ttu-id="e22dc-188">**site** 由一个唯一 ID 标识，此唯一 ID 由以下值组成：</span><span class="sxs-lookup"><span data-stu-id="e22dc-188">A **site** is addressed by a unique identifier which is a composite ID of the following values:</span></span>
* <span data-ttu-id="e22dc-189">网站集主机名称 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="e22dc-189">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="e22dc-190">网站集的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="e22dc-190">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="e22dc-191">网站的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="e22dc-191">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="e22dc-192">`root` 标识符经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="e22dc-192">There is also a reserved site identifier, `root`, which always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="e22dc-193">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="e22dc-193">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="e22dc-194">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="e22dc-194">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="e22dc-195">关系</span><span class="sxs-lookup"><span data-stu-id="e22dc-195">Relationships</span></span>

| <span data-ttu-id="e22dc-196">关系名称</span><span class="sxs-lookup"><span data-stu-id="e22dc-196">Relationship name</span></span> | <span data-ttu-id="e22dc-197">类型</span><span class="sxs-lookup"><span data-stu-id="e22dc-197">Type</span></span>                             | <span data-ttu-id="e22dc-198">说明</span><span class="sxs-lookup"><span data-stu-id="e22dc-198">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="e22dc-199">**analytics**</span><span class="sxs-lookup"><span data-stu-id="e22dc-199">**analytics**</span></span>     | <span data-ttu-id="e22dc-200">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="e22dc-200">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="e22dc-201">此网站上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="e22dc-201">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="e22dc-202">**columns**</span><span class="sxs-lookup"><span data-stu-id="e22dc-202">**columns**</span></span>       | <span data-ttu-id="e22dc-203">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="e22dc-203">Collection([columnDefinition][])</span></span> | <span data-ttu-id="e22dc-204">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="e22dc-204">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="e22dc-205">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="e22dc-205">**contentTypes**</span></span>  | <span data-ttu-id="e22dc-206">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="e22dc-206">Collection([contentType][])</span></span>      | <span data-ttu-id="e22dc-207">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="e22dc-207">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="e22dc-208">**drive**</span><span class="sxs-lookup"><span data-stu-id="e22dc-208">**drive**</span></span>         | <span data-ttu-id="e22dc-209">[drive][]</span><span class="sxs-lookup"><span data-stu-id="e22dc-209">[drive][]</span></span>                        | <span data-ttu-id="e22dc-210">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="e22dc-210">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="e22dc-211">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="e22dc-211">**drives**</span></span>        | <span data-ttu-id="e22dc-212">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="e22dc-212">Collection([drive][])</span></span>            | <span data-ttu-id="e22dc-213">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="e22dc-213">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="e22dc-214">**项目**</span><span class="sxs-lookup"><span data-stu-id="e22dc-214">**items**</span></span>         | <span data-ttu-id="e22dc-215">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="e22dc-215">Collection([baseItem][])</span></span>         | <span data-ttu-id="e22dc-p110">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="e22dc-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="e22dc-218">**lists**</span><span class="sxs-lookup"><span data-stu-id="e22dc-218">**lists**</span></span>         | <span data-ttu-id="e22dc-219">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="e22dc-219">Collection([list][])</span></span>             | <span data-ttu-id="e22dc-220">此网站下的列表集合。</span><span class="sxs-lookup"><span data-stu-id="e22dc-220">The collection of lists under this site.</span></span>
| <span data-ttu-id="e22dc-221">**pages**</span><span class="sxs-lookup"><span data-stu-id="e22dc-221">**pages**</span></span>         | <span data-ttu-id="e22dc-222">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="e22dc-222">Collection([sitePage][])</span></span>         | <span data-ttu-id="e22dc-223">此网站的 SitePages 列表中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="e22dc-223">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="e22dc-224">**sites**</span><span class="sxs-lookup"><span data-stu-id="e22dc-224">**sites**</span></span>         | <span data-ttu-id="e22dc-225">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="e22dc-225">Collection([site][])</span></span>             | <span data-ttu-id="e22dc-226">网站下的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="e22dc-226">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="e22dc-238">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e22dc-238">JSON representation</span></span>

<span data-ttu-id="e22dc-239">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e22dc-239">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="e22dc-240">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="e22dc-240">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
