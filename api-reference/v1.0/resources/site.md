---
author: JeremyKelley
ms.author: JeremyKelley
title: site 资源
description: site 资源提供 Sharepoint 网站的元数据和关系。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 1878b46f7738f440808960e43310b2d7606ee22f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533696"
---
# <a name="site-resource"></a><span data-ttu-id="899a7-103">site 资源</span><span class="sxs-lookup"><span data-stu-id="899a7-103">site resource</span></span>

<span data-ttu-id="899a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="899a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="899a7-105">**site** 资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="899a7-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="899a7-106">方法</span><span class="sxs-lookup"><span data-stu-id="899a7-106">Methods</span></span>

| <span data-ttu-id="899a7-107">方法</span><span class="sxs-lookup"><span data-stu-id="899a7-107">Method</span></span>                | <span data-ttu-id="899a7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="899a7-108">Return type</span></span> | <span data-ttu-id="899a7-109">说明</span><span class="sxs-lookup"><span data-stu-id="899a7-109">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="899a7-110">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="899a7-110">[Get root site][]</span></span>        | <span data-ttu-id="899a7-111">网站</span><span class="sxs-lookup"><span data-stu-id="899a7-111">site</span></span> | <span data-ttu-id="899a7-112">访问租户内的根 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="899a7-112">Access the root SharePoint site within a tenant.</span></span>
| <span data-ttu-id="899a7-113">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="899a7-113">[Get site][]</span></span>             | <span data-ttu-id="899a7-114">网站</span><span class="sxs-lookup"><span data-stu-id="899a7-114">site</span></span> | <span data-ttu-id="899a7-115">使用 siteId 访问 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="899a7-115">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="899a7-116">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="899a7-116">[Get site by path][]</span></span>     | <span data-ttu-id="899a7-117">网站</span><span class="sxs-lookup"><span data-stu-id="899a7-117">site</span></span> | <span data-ttu-id="899a7-118">通过相对路径访问根 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="899a7-118">Access the root SharePoint site with a relative path.</span></span>
| <span data-ttu-id="899a7-119">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="899a7-119">[Get site for a group][]</span></span> | <span data-ttu-id="899a7-120">网站</span><span class="sxs-lookup"><span data-stu-id="899a7-120">site</span></span> | <span data-ttu-id="899a7-121">访问组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="899a7-121">Access the team site for a group.</span></span>
| <span data-ttu-id="899a7-122">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="899a7-122">[Get analytics][]</span></span>              | <span data-ttu-id="899a7-123">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="899a7-123">[itemAnalytics][]</span></span> | <span data-ttu-id="899a7-124">对此资源可获取分析。</span><span class="sxs-lookup"><span data-stu-id="899a7-124">Get analytics for this resource.</span></span> 
| <span data-ttu-id="899a7-125">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="899a7-125">[Get activities by interval][]</span></span> | <span data-ttu-id="899a7-126">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="899a7-126">[itemActivityStat][]</span></span> | <span data-ttu-id="899a7-127">在指定的时间间隔内获取 **itemActivityStats** 的集合。</span><span class="sxs-lookup"><span data-stu-id="899a7-127">Get a collection of **itemActivityStats** within the specified time interval.</span></span>
| <span data-ttu-id="899a7-128">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="899a7-128">[Search for sites][]</span></span>     | <span data-ttu-id="899a7-129">网站集合</span><span class="sxs-lookup"><span data-stu-id="899a7-129">collection of site</span></span> | <span data-ttu-id="899a7-130">在 SharePoint 租户中搜索与所提供的关键字匹配的 网站。</span><span class="sxs-lookup"><span data-stu-id="899a7-130">Search across a SharePoint tenant for sites that match keywords provided.</span></span>

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

## <a name="properties"></a><span data-ttu-id="899a7-139">属性</span><span class="sxs-lookup"><span data-stu-id="899a7-139">Properties</span></span>

| <span data-ttu-id="899a7-140">属性</span><span class="sxs-lookup"><span data-stu-id="899a7-140">Property</span></span>            | <span data-ttu-id="899a7-141">类型</span><span class="sxs-lookup"><span data-stu-id="899a7-141">Type</span></span>                                | <span data-ttu-id="899a7-142">说明</span><span class="sxs-lookup"><span data-stu-id="899a7-142">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="899a7-143">**id**</span><span class="sxs-lookup"><span data-stu-id="899a7-143">**id**</span></span>                   | <span data-ttu-id="899a7-144">string</span><span class="sxs-lookup"><span data-stu-id="899a7-144">string</span></span>                              | <span data-ttu-id="899a7-p101">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="899a7-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="899a7-147">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="899a7-147">**createdDateTime**</span></span>      | <span data-ttu-id="899a7-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="899a7-148">DateTimeOffset</span></span>                      | <span data-ttu-id="899a7-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="899a7-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="899a7-151">**说明**</span><span class="sxs-lookup"><span data-stu-id="899a7-151">**description**</span></span>          | <span data-ttu-id="899a7-152">string</span><span class="sxs-lookup"><span data-stu-id="899a7-152">string</span></span>                              | <span data-ttu-id="899a7-153">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="899a7-153">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="899a7-154">**displayName**</span><span class="sxs-lookup"><span data-stu-id="899a7-154">**displayName**</span></span>          | <span data-ttu-id="899a7-155">string</span><span class="sxs-lookup"><span data-stu-id="899a7-155">string</span></span>                              | <span data-ttu-id="899a7-p103">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="899a7-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="899a7-158">**eTag**</span><span class="sxs-lookup"><span data-stu-id="899a7-158">**eTag**</span></span>                 | <span data-ttu-id="899a7-159">string</span><span class="sxs-lookup"><span data-stu-id="899a7-159">string</span></span>                              | <span data-ttu-id="899a7-p104">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="899a7-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="899a7-162">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="899a7-162">**lastModifiedDateTime**</span></span> | <span data-ttu-id="899a7-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="899a7-163">DateTimeOffset</span></span>                      | <span data-ttu-id="899a7-p105">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="899a7-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="899a7-166">**name**</span><span class="sxs-lookup"><span data-stu-id="899a7-166">**name**</span></span>                 | <span data-ttu-id="899a7-167">string</span><span class="sxs-lookup"><span data-stu-id="899a7-167">string</span></span>                              | <span data-ttu-id="899a7-168">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="899a7-168">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="899a7-169">**根**</span><span class="sxs-lookup"><span data-stu-id="899a7-169">**root**</span></span>                 | [<span data-ttu-id="899a7-170">根</span><span class="sxs-lookup"><span data-stu-id="899a7-170">root</span></span>](root.md)                     | <span data-ttu-id="899a7-p106">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="899a7-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="899a7-173">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="899a7-173">**sharepointIds**</span></span>        | [<span data-ttu-id="899a7-174">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="899a7-174">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="899a7-p107">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="899a7-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="899a7-177">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="899a7-177">**siteCollection**</span></span>       | [<span data-ttu-id="899a7-178">siteCollection</span><span class="sxs-lookup"><span data-stu-id="899a7-178">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="899a7-p108">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="899a7-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="899a7-182">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="899a7-182">**webUrl**</span></span>               | <span data-ttu-id="899a7-183">string (url)</span><span class="sxs-lookup"><span data-stu-id="899a7-183">string (url)</span></span>                        | <span data-ttu-id="899a7-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="899a7-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="899a7-186">关系</span><span class="sxs-lookup"><span data-stu-id="899a7-186">Relationships</span></span>

| <span data-ttu-id="899a7-187">关系</span><span class="sxs-lookup"><span data-stu-id="899a7-187">Relationship</span></span>      | <span data-ttu-id="899a7-188">类型</span><span class="sxs-lookup"><span data-stu-id="899a7-188">Type</span></span>                             | <span data-ttu-id="899a7-189">说明</span><span class="sxs-lookup"><span data-stu-id="899a7-189">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="899a7-190">**analytics**</span><span class="sxs-lookup"><span data-stu-id="899a7-190">**analytics**</span></span>     | <span data-ttu-id="899a7-191">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="899a7-191">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="899a7-192">此网站上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="899a7-192">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="899a7-193">**columns**</span><span class="sxs-lookup"><span data-stu-id="899a7-193">**columns**</span></span>       | <span data-ttu-id="899a7-194">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="899a7-194">Collection([columnDefinition][])</span></span> | <span data-ttu-id="899a7-195">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="899a7-195">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="899a7-196">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="899a7-196">**contentTypes**</span></span>  | <span data-ttu-id="899a7-197">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="899a7-197">Collection([contentType][])</span></span>      | <span data-ttu-id="899a7-198">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="899a7-198">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="899a7-199">**drive**</span><span class="sxs-lookup"><span data-stu-id="899a7-199">**drive**</span></span>         | <span data-ttu-id="899a7-200">[drive][]</span><span class="sxs-lookup"><span data-stu-id="899a7-200">[drive][]</span></span>                        | <span data-ttu-id="899a7-201">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="899a7-201">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="899a7-202">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="899a7-202">**drives**</span></span>        | <span data-ttu-id="899a7-203">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="899a7-203">Collection([drive][])</span></span>            | <span data-ttu-id="899a7-204">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="899a7-204">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="899a7-205">**项目**</span><span class="sxs-lookup"><span data-stu-id="899a7-205">**items**</span></span>         | <span data-ttu-id="899a7-206">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="899a7-206">Collection([baseItem][])</span></span>         | <span data-ttu-id="899a7-p110">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="899a7-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="899a7-209">**lists**</span><span class="sxs-lookup"><span data-stu-id="899a7-209">**lists**</span></span>         | <span data-ttu-id="899a7-210">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="899a7-210">Collection([list][])</span></span>             | <span data-ttu-id="899a7-211">此网站下方的列表集合。</span><span class="sxs-lookup"><span data-stu-id="899a7-211">The collection of lists under this site.</span></span>
| <span data-ttu-id="899a7-212">**sites**</span><span class="sxs-lookup"><span data-stu-id="899a7-212">**sites**</span></span>         | <span data-ttu-id="899a7-213">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="899a7-213">Collection([site][])</span></span>             | <span data-ttu-id="899a7-214">网站下方的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="899a7-214">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="899a7-215">**onenote**</span><span class="sxs-lookup"><span data-stu-id="899a7-215">**onenote**</span></span>       | <span data-ttu-id="899a7-216">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="899a7-216">[onenote][]</span></span>                      | <span data-ttu-id="899a7-217">调用 OneNote 服务执行笔记本相关操作。</span><span class="sxs-lookup"><span data-stu-id="899a7-217">Calls the OneNote service for notebook related operations.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="899a7-226">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="899a7-226">JSON representation</span></span>

<span data-ttu-id="899a7-227">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="899a7-227">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="899a7-228">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="899a7-228">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
