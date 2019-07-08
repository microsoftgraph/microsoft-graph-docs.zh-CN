---
author: JeremyKelley
ms.author: JeremyKelley
title: site 资源
description: site 资源提供 Sharepoint 网站的元数据和关系。
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 40add99dfbeee28d82b3d02def833497c01385df
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33968847"
---
# <a name="site-resource"></a><span data-ttu-id="367f3-103">site 资源</span><span class="sxs-lookup"><span data-stu-id="367f3-103">Site resource</span></span>

<span data-ttu-id="367f3-104">**site** 资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="367f3-104">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="367f3-105">方法</span><span class="sxs-lookup"><span data-stu-id="367f3-105">Methods</span></span>

| <span data-ttu-id="367f3-106">方法</span><span class="sxs-lookup"><span data-stu-id="367f3-106">Method</span></span>                | <span data-ttu-id="367f3-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="367f3-107">Return type</span></span> | <span data-ttu-id="367f3-108">说明</span><span class="sxs-lookup"><span data-stu-id="367f3-108">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="367f3-109">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="367f3-109">[Get root site][]</span></span>        | <span data-ttu-id="367f3-110">网站</span><span class="sxs-lookup"><span data-stu-id="367f3-110">Site</span></span> | <span data-ttu-id="367f3-111">访问租户内的根 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="367f3-111">To access the root SharePoint site within a tenant:</span></span>
| <span data-ttu-id="367f3-112">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="367f3-112">[Get site][]</span></span>             | <span data-ttu-id="367f3-113">网站</span><span class="sxs-lookup"><span data-stu-id="367f3-113">Site</span></span> | <span data-ttu-id="367f3-114">使用 siteId 访问 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="367f3-114">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="367f3-115">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="367f3-115">[Get site by path][]</span></span>     | <span data-ttu-id="367f3-116">网站</span><span class="sxs-lookup"><span data-stu-id="367f3-116">Site</span></span> | <span data-ttu-id="367f3-117">通过相对路径访问根 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="367f3-117">To access the root SharePoint site with a relative path:</span></span>
| <span data-ttu-id="367f3-118">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="367f3-118">[Get site for a group][]</span></span> | <span data-ttu-id="367f3-119">网站</span><span class="sxs-lookup"><span data-stu-id="367f3-119">Site</span></span> | <span data-ttu-id="367f3-120">访问组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="367f3-120">To access the team site for a group:</span></span>
| <span data-ttu-id="367f3-121">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="367f3-121">[Get analytics][]</span></span>              | <span data-ttu-id="367f3-122">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="367f3-122">[itemAnalytics][]</span></span> | <span data-ttu-id="367f3-123">对此资源可获取分析。</span><span class="sxs-lookup"><span data-stu-id="367f3-123">Get analytics for this resource.</span></span> 
| <span data-ttu-id="367f3-124">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="367f3-124">[Get activities by interval][]</span></span> | <span data-ttu-id="367f3-125">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="367f3-125">[itemActivityStat][]</span></span> | <span data-ttu-id="367f3-126">在指定的时间间隔内获取 **itemActivityStats** 的集合。</span><span class="sxs-lookup"><span data-stu-id="367f3-126">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="367f3-127">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="367f3-127">[Search for sites][]</span></span>     | <span data-ttu-id="367f3-128">网站集合</span><span class="sxs-lookup"><span data-stu-id="367f3-128">collection of site</span></span> | <span data-ttu-id="367f3-129">在 SharePoint 租户中搜索与所提供的关键字匹配的 网站。</span><span class="sxs-lookup"><span data-stu-id="367f3-129">Search across a SharePoint tenant for sites that match provided keywords.</span></span>

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
[按间隔获取活动]: ../api/itemactivitystat-getactivitybyinterval.md
[Get activities by interval]: ../api/itemactivitystat-getactivitybyinterval.md
[搜索网站]: ../api/site-search.md
[Search for sites]: ../api/site-search.md
[itemActivityStat]: itemactivitystat.md

## <a name="properties"></a><span data-ttu-id="367f3-138">属性</span><span class="sxs-lookup"><span data-stu-id="367f3-138">Properties</span></span>

| <span data-ttu-id="367f3-139">属性</span><span class="sxs-lookup"><span data-stu-id="367f3-139">Property</span></span>            | <span data-ttu-id="367f3-140">类型</span><span class="sxs-lookup"><span data-stu-id="367f3-140">Type</span></span>                                | <span data-ttu-id="367f3-141">说明</span><span class="sxs-lookup"><span data-stu-id="367f3-141">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="367f3-142">**id**</span><span class="sxs-lookup"><span data-stu-id="367f3-142">**id**</span></span>                   | <span data-ttu-id="367f3-143">string</span><span class="sxs-lookup"><span data-stu-id="367f3-143">string</span></span>                              | <span data-ttu-id="367f3-p101">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="367f3-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="367f3-146">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="367f3-146">**createdDateTime**</span></span>      | <span data-ttu-id="367f3-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="367f3-147">DateTimeOffset</span></span>                      | <span data-ttu-id="367f3-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="367f3-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="367f3-150">**说明**</span><span class="sxs-lookup"><span data-stu-id="367f3-150">**description**</span></span>          | <span data-ttu-id="367f3-151">string</span><span class="sxs-lookup"><span data-stu-id="367f3-151">string</span></span>                              | <span data-ttu-id="367f3-152">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="367f3-152">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="367f3-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="367f3-153">**displayName**</span></span>          | <span data-ttu-id="367f3-154">string</span><span class="sxs-lookup"><span data-stu-id="367f3-154">string</span></span>                              | <span data-ttu-id="367f3-p103">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="367f3-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="367f3-157">**eTag**</span><span class="sxs-lookup"><span data-stu-id="367f3-157">**eTag**</span></span>                 | <span data-ttu-id="367f3-158">string</span><span class="sxs-lookup"><span data-stu-id="367f3-158">string</span></span>                              | <span data-ttu-id="367f3-p104">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="367f3-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="367f3-161">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="367f3-161">**lastModifiedDateTime**</span></span> | <span data-ttu-id="367f3-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="367f3-162">DateTimeOffset</span></span>                      | <span data-ttu-id="367f3-p105">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="367f3-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="367f3-165">**name**</span><span class="sxs-lookup"><span data-stu-id="367f3-165">**name**</span></span>                 | <span data-ttu-id="367f3-166">string</span><span class="sxs-lookup"><span data-stu-id="367f3-166">string</span></span>                              | <span data-ttu-id="367f3-167">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="367f3-167">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="367f3-168">**根**</span><span class="sxs-lookup"><span data-stu-id="367f3-168">**root**</span></span>                 | [<span data-ttu-id="367f3-169">根</span><span class="sxs-lookup"><span data-stu-id="367f3-169">root</span></span>](root.md)                     | <span data-ttu-id="367f3-p106">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="367f3-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="367f3-172">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="367f3-172">**sharepointIds**</span></span>        | [<span data-ttu-id="367f3-173">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="367f3-173">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="367f3-p107">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="367f3-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="367f3-176">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="367f3-176">**siteCollection**</span></span>       | [<span data-ttu-id="367f3-177">siteCollection</span><span class="sxs-lookup"><span data-stu-id="367f3-177">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="367f3-p108">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="367f3-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="367f3-181">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="367f3-181">**webUrl**</span></span>               | <span data-ttu-id="367f3-182">string (url)</span><span class="sxs-lookup"><span data-stu-id="367f3-182">string (url)</span></span>                        | <span data-ttu-id="367f3-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="367f3-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="367f3-185">关系</span><span class="sxs-lookup"><span data-stu-id="367f3-185">Relationships</span></span>

| <span data-ttu-id="367f3-186">关系</span><span class="sxs-lookup"><span data-stu-id="367f3-186">Relationship</span></span>      | <span data-ttu-id="367f3-187">类型</span><span class="sxs-lookup"><span data-stu-id="367f3-187">Type</span></span>                             | <span data-ttu-id="367f3-188">说明</span><span class="sxs-lookup"><span data-stu-id="367f3-188">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="367f3-189">**analytics**</span><span class="sxs-lookup"><span data-stu-id="367f3-189">**analytics**</span></span>     | <span data-ttu-id="367f3-190">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="367f3-190">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="367f3-191">此网站上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="367f3-191">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="367f3-192">**columns**</span><span class="sxs-lookup"><span data-stu-id="367f3-192">**columns**</span></span>       | <span data-ttu-id="367f3-193">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="367f3-193">Collection([columnDefinition][])</span></span> | <span data-ttu-id="367f3-194">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="367f3-194">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="367f3-195">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="367f3-195">**contentTypes**</span></span>  | <span data-ttu-id="367f3-196">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="367f3-196">Collection([contentType][])</span></span>      | <span data-ttu-id="367f3-197">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="367f3-197">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="367f3-198">**drive**</span><span class="sxs-lookup"><span data-stu-id="367f3-198">**drive**</span></span>         | <span data-ttu-id="367f3-199">[drive][]</span><span class="sxs-lookup"><span data-stu-id="367f3-199">[drive][]</span></span>                        | <span data-ttu-id="367f3-200">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="367f3-200">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="367f3-201">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="367f3-201">**drives**</span></span>        | <span data-ttu-id="367f3-202">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="367f3-202">Collection([drive][])</span></span>            | <span data-ttu-id="367f3-203">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="367f3-203">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="367f3-204">**项目**</span><span class="sxs-lookup"><span data-stu-id="367f3-204">**items**</span></span>         | <span data-ttu-id="367f3-205">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="367f3-205">Collection([baseItem][])</span></span>         | <span data-ttu-id="367f3-p110">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="367f3-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="367f3-208">**lists**</span><span class="sxs-lookup"><span data-stu-id="367f3-208">**lists**</span></span>         | <span data-ttu-id="367f3-209">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="367f3-209">Collection([list][])</span></span>             | <span data-ttu-id="367f3-210">此网站下方的列表集合。</span><span class="sxs-lookup"><span data-stu-id="367f3-210">The collection of lists under this site.</span></span>
| <span data-ttu-id="367f3-211">**sites**</span><span class="sxs-lookup"><span data-stu-id="367f3-211">**sites**</span></span>         | <span data-ttu-id="367f3-212">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="367f3-212">Collection([site][])</span></span>             | <span data-ttu-id="367f3-213">网站下方的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="367f3-213">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="367f3-214">**onenote**</span><span class="sxs-lookup"><span data-stu-id="367f3-214">**onenote**</span></span>       | <span data-ttu-id="367f3-215">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="367f3-215">[onenote][]</span></span>                      | <span data-ttu-id="367f3-216">调用 OneNote 服务执行笔记本相关操作。</span><span class="sxs-lookup"><span data-stu-id="367f3-216">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[网站]: site.md
[site]: site.md
[onenote]: onenote.md

## <a name="json-representation"></a><span data-ttu-id="367f3-225">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="367f3-225">JSON representation</span></span>

<span data-ttu-id="367f3-226">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="367f3-226">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="367f3-227">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="367f3-227">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
