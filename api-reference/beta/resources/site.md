---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.openlocfilehash: fb91e9bada227f1a22cf862726ea0b6f658fe469
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871020"
---
# <a name="site-resource-type"></a><span data-ttu-id="ed802-102">网站资源类型</span><span class="sxs-lookup"><span data-stu-id="ed802-102">site resource type</span></span>

> <span data-ttu-id="ed802-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ed802-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed802-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ed802-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed802-105">**网站**资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="ed802-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="ed802-106">方法</span><span class="sxs-lookup"><span data-stu-id="ed802-106">Methods</span></span>

| <span data-ttu-id="ed802-107">方法</span><span class="sxs-lookup"><span data-stu-id="ed802-107">Method</span></span>                         | <span data-ttu-id="ed802-108">REST 路径</span><span class="sxs-lookup"><span data-stu-id="ed802-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="ed802-109">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="ed802-109">[Get root site][]</span></span>              | <span data-ttu-id="ed802-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="ed802-110">GET /sites/root</span></span>
| <span data-ttu-id="ed802-111">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="ed802-111">[Get site][]</span></span>                   | <span data-ttu-id="ed802-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="ed802-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="ed802-113">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="ed802-113">[Get site by path][]</span></span>           | <span data-ttu-id="ed802-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="ed802-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="ed802-115">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="ed802-115">[Get site for a group][]</span></span>       | <span data-ttu-id="ed802-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="ed802-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="ed802-117">[获取分析][]</span><span class="sxs-lookup"><span data-stu-id="ed802-117">[Get analytics][]</span></span>              | <span data-ttu-id="ed802-118">GET /sites/ {网站-id} / 分析</span><span class="sxs-lookup"><span data-stu-id="ed802-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="ed802-119">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="ed802-119">[Get activities by interval][]</span></span> | <span data-ttu-id="ed802-120">GET /sites/ {网站-id} / getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="ed802-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="ed802-121">[List pages][]</span><span class="sxs-lookup"><span data-stu-id="ed802-121">[List pages][]</span></span>                 | <span data-ttu-id="ed802-122">GET /sites/ {网站-id} / 页面</span><span class="sxs-lookup"><span data-stu-id="ed802-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="ed802-123">[列出根网站][]</span><span class="sxs-lookup"><span data-stu-id="ed802-123">[List root sites][]</span></span>            | <span data-ttu-id="ed802-124">GET /sites？ 筛选器 = 根 ne null = 选择 = sitecollection 和 Site，webUrl</span><span class="sxs-lookup"><span data-stu-id="ed802-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="ed802-125">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="ed802-125">[Search for sites][]</span></span>           | <span data-ttu-id="ed802-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="ed802-126">GET /sites?search={query}</span></span>

[获取网站]: ../api/site-get.md
[Get site]: ../api/site-get.md
[获取根网站]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[根据路径获取网站]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[获取组的网站]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[获取分析]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[List pages]: ../api/sitepage-list.md
[列出根网站]: ../api/site-list.md
[List root sites]: ../api/site-list.md
[搜索网站]: ../api/site-search.md
[Search for sites]: ../api/site-search.md


## <a name="properties"></a><span data-ttu-id="ed802-136">属性</span><span class="sxs-lookup"><span data-stu-id="ed802-136">Properties</span></span>

| <span data-ttu-id="ed802-137">属性名称</span><span class="sxs-lookup"><span data-stu-id="ed802-137">Property name</span></span>            | <span data-ttu-id="ed802-138">类型</span><span class="sxs-lookup"><span data-stu-id="ed802-138">Type</span></span>               | <span data-ttu-id="ed802-139">说明</span><span class="sxs-lookup"><span data-stu-id="ed802-139">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="ed802-140">**id**</span><span class="sxs-lookup"><span data-stu-id="ed802-140">**id**</span></span>                   | <span data-ttu-id="ed802-141">string</span><span class="sxs-lookup"><span data-stu-id="ed802-141">string</span></span>             | <span data-ttu-id="ed802-p102">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="ed802-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="ed802-144">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="ed802-144">**createdDateTime**</span></span>      | <span data-ttu-id="ed802-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed802-145">DateTimeOffset</span></span>     | <span data-ttu-id="ed802-p103">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="ed802-p103">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="ed802-148">**说明**</span><span class="sxs-lookup"><span data-stu-id="ed802-148">**description**</span></span>          | <span data-ttu-id="ed802-149">string</span><span class="sxs-lookup"><span data-stu-id="ed802-149">string</span></span>             | <span data-ttu-id="ed802-150">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="ed802-150">The descriptive text for the site.</span></span>
| <span data-ttu-id="ed802-151">**eTag**</span><span class="sxs-lookup"><span data-stu-id="ed802-151">**eTag**</span></span>                 | <span data-ttu-id="ed802-152">string</span><span class="sxs-lookup"><span data-stu-id="ed802-152">string</span></span>             | <span data-ttu-id="ed802-p104">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="ed802-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="ed802-155">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ed802-155">**displayName**</span></span>          | <span data-ttu-id="ed802-156">string</span><span class="sxs-lookup"><span data-stu-id="ed802-156">string</span></span>             | <span data-ttu-id="ed802-p105">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="ed802-p105">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="ed802-159">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ed802-159">**lastModifiedDateTime**</span></span> | <span data-ttu-id="ed802-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ed802-160">DateTimeOffset</span></span>     | <span data-ttu-id="ed802-p106">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="ed802-p106">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ed802-163">**name**</span><span class="sxs-lookup"><span data-stu-id="ed802-163">**name**</span></span>                 | <span data-ttu-id="ed802-164">string</span><span class="sxs-lookup"><span data-stu-id="ed802-164">string</span></span>             | <span data-ttu-id="ed802-165">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="ed802-165">The name / title of the item.</span></span>
| <span data-ttu-id="ed802-166">**根**</span><span class="sxs-lookup"><span data-stu-id="ed802-166">**root**</span></span>                 | <span data-ttu-id="ed802-167">[根][]</span><span class="sxs-lookup"><span data-stu-id="ed802-167">[root][]</span></span>           | <span data-ttu-id="ed802-p107">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="ed802-p107">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="ed802-170">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="ed802-170">**sharepointIds**</span></span>        | <span data-ttu-id="ed802-171">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ed802-171">[sharepointIds][]</span></span>  | <span data-ttu-id="ed802-p108">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="ed802-p108">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="ed802-174">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="ed802-174">**siteCollection**</span></span>       | <span data-ttu-id="ed802-175">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="ed802-175">[siteCollection][]</span></span> | <span data-ttu-id="ed802-p109">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="ed802-p109">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="ed802-179">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="ed802-179">**webUrl**</span></span>               | <span data-ttu-id="ed802-180">string (url)</span><span class="sxs-lookup"><span data-stu-id="ed802-180">string (url)</span></span>       | <span data-ttu-id="ed802-p110">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="ed802-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="ed802-183">关系</span><span class="sxs-lookup"><span data-stu-id="ed802-183">Relationships</span></span>

| <span data-ttu-id="ed802-184">关系名称</span><span class="sxs-lookup"><span data-stu-id="ed802-184">Relationship name</span></span> | <span data-ttu-id="ed802-185">类型</span><span class="sxs-lookup"><span data-stu-id="ed802-185">Type</span></span>                             | <span data-ttu-id="ed802-186">Description</span><span class="sxs-lookup"><span data-stu-id="ed802-186">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="ed802-187">**分析**</span><span class="sxs-lookup"><span data-stu-id="ed802-187">**analytics**</span></span>     | <span data-ttu-id="ed802-188">[itemAnalytics][]资源</span><span class="sxs-lookup"><span data-stu-id="ed802-188">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="ed802-189">有关发生此网站中查看活动的分析。</span><span class="sxs-lookup"><span data-stu-id="ed802-189">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="ed802-190">**columns**</span><span class="sxs-lookup"><span data-stu-id="ed802-190">**columns**</span></span>       | <span data-ttu-id="ed802-191">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="ed802-191">Collection([columnDefinition][])</span></span> | <span data-ttu-id="ed802-192">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="ed802-192">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="ed802-193">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="ed802-193">**contentTypes**</span></span>  | <span data-ttu-id="ed802-194">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="ed802-194">Collection([contentType][])</span></span>      | <span data-ttu-id="ed802-195">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="ed802-195">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="ed802-196">**drive**</span><span class="sxs-lookup"><span data-stu-id="ed802-196">**drive**</span></span>         | <span data-ttu-id="ed802-197">[驱动器][]</span><span class="sxs-lookup"><span data-stu-id="ed802-197">[drive][]</span></span>                        | <span data-ttu-id="ed802-198">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="ed802-198">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="ed802-199">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="ed802-199">**drives**</span></span>        | <span data-ttu-id="ed802-200">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="ed802-200">Collection([drive][])</span></span>            | <span data-ttu-id="ed802-201">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="ed802-201">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="ed802-202">**项目**</span><span class="sxs-lookup"><span data-stu-id="ed802-202">**items**</span></span>         | <span data-ttu-id="ed802-203">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="ed802-203">Collection([baseItem][])</span></span>         | <span data-ttu-id="ed802-p111">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="ed802-p111">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="ed802-206">**lists**</span><span class="sxs-lookup"><span data-stu-id="ed802-206">**lists**</span></span>         | <span data-ttu-id="ed802-207">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="ed802-207">Collection([list][])</span></span>             | <span data-ttu-id="ed802-208">此网站下方的列表集合。</span><span class="sxs-lookup"><span data-stu-id="ed802-208">The collection of lists under this site.</span></span>
| <span data-ttu-id="ed802-209">**页面**</span><span class="sxs-lookup"><span data-stu-id="ed802-209">**pages**</span></span>         | <span data-ttu-id="ed802-210">集合 ([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="ed802-210">Collection([sitePage][])</span></span>         | <span data-ttu-id="ed802-211">在此站点的 SitePages 列表中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="ed802-211">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="ed802-212">**sites**</span><span class="sxs-lookup"><span data-stu-id="ed802-212">**sites**</span></span>         | <span data-ttu-id="ed802-213">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="ed802-213">Collection([site][])</span></span>             | <span data-ttu-id="ed802-214">网站下方的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="ed802-214">The collection of the sub-sites under this site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[列表]: list.md
[list]: list.md
[sitePage]: sitepage.md
[根]: root.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="ed802-226">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed802-226">JSON representation</span></span>

<span data-ttu-id="ed802-227">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed802-227">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="ed802-228">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="ed802-228">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites",
  "tocBookmarks": { "Resources/Site": "#" }
} -->
