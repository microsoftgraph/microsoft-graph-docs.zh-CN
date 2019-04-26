---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 63d4232c2af37541f2a96359f9d2a209d065bc98
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343047"
---
# <a name="site-resource-type"></a><span data-ttu-id="83951-102">site 资源类型</span><span class="sxs-lookup"><span data-stu-id="83951-102">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83951-103">**site** 资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="83951-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="83951-104">方法</span><span class="sxs-lookup"><span data-stu-id="83951-104">Methods</span></span>

| <span data-ttu-id="83951-105">方法</span><span class="sxs-lookup"><span data-stu-id="83951-105">Method</span></span>                         | <span data-ttu-id="83951-106">REST 路径</span><span class="sxs-lookup"><span data-stu-id="83951-106">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="83951-107">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="83951-107">[Get root site][]</span></span>              | <span data-ttu-id="83951-108">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="83951-108">GET /sites/root</span></span>
| <span data-ttu-id="83951-109">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="83951-109">[Get site][]</span></span>                   | <span data-ttu-id="83951-110">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="83951-110">GET /sites/{site-id}</span></span>
| <span data-ttu-id="83951-111">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="83951-111">[Get site by path][]</span></span>           | <span data-ttu-id="83951-112">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="83951-112">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="83951-113">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="83951-113">[Get site for a group][]</span></span>       | <span data-ttu-id="83951-114">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="83951-114">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="83951-115">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="83951-115">[Get analytics][]</span></span>              | <span data-ttu-id="83951-116">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="83951-116">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="83951-117">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="83951-117">[Get activities by interval][]</span></span> | <span data-ttu-id="83951-118">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="83951-118">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="83951-119">[列出页面][]</span><span class="sxs-lookup"><span data-stu-id="83951-119">[List pages][]</span></span>                 | <span data-ttu-id="83951-120">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="83951-120">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="83951-121">[列出根网站][]</span><span class="sxs-lookup"><span data-stu-id="83951-121">[List root sites][]</span></span>            | <span data-ttu-id="83951-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="83951-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="83951-123">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="83951-123">[Search for sites][]</span></span>           | <span data-ttu-id="83951-124">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="83951-124">GET /sites?search={query}</span></span>

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


## <a name="properties"></a><span data-ttu-id="83951-134">属性</span><span class="sxs-lookup"><span data-stu-id="83951-134">Properties</span></span>

| <span data-ttu-id="83951-135">属性名称</span><span class="sxs-lookup"><span data-stu-id="83951-135">Property name</span></span>            | <span data-ttu-id="83951-136">类型</span><span class="sxs-lookup"><span data-stu-id="83951-136">Type</span></span>               | <span data-ttu-id="83951-137">说明</span><span class="sxs-lookup"><span data-stu-id="83951-137">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="83951-138">**id**</span><span class="sxs-lookup"><span data-stu-id="83951-138">**id**</span></span>                   | <span data-ttu-id="83951-139">string</span><span class="sxs-lookup"><span data-stu-id="83951-139">string</span></span>             | <span data-ttu-id="83951-p101">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="83951-p101">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="83951-142">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="83951-142">**createdDateTime**</span></span>      | <span data-ttu-id="83951-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83951-143">DateTimeOffset</span></span>     | <span data-ttu-id="83951-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="83951-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="83951-146">**说明**</span><span class="sxs-lookup"><span data-stu-id="83951-146">**description**</span></span>          | <span data-ttu-id="83951-147">string</span><span class="sxs-lookup"><span data-stu-id="83951-147">string</span></span>             | <span data-ttu-id="83951-148">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="83951-148">The descriptive text for the site.</span></span>
| <span data-ttu-id="83951-149">**eTag**</span><span class="sxs-lookup"><span data-stu-id="83951-149">**eTag**</span></span>                 | <span data-ttu-id="83951-150">string</span><span class="sxs-lookup"><span data-stu-id="83951-150">string</span></span>             | <span data-ttu-id="83951-p103">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="83951-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="83951-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="83951-153">**displayName**</span></span>          | <span data-ttu-id="83951-154">string</span><span class="sxs-lookup"><span data-stu-id="83951-154">string</span></span>             | <span data-ttu-id="83951-p104">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="83951-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="83951-157">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="83951-157">**lastModifiedDateTime**</span></span> | <span data-ttu-id="83951-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83951-158">DateTimeOffset</span></span>     | <span data-ttu-id="83951-p105">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="83951-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="83951-161">**name**</span><span class="sxs-lookup"><span data-stu-id="83951-161">**name**</span></span>                 | <span data-ttu-id="83951-162">string</span><span class="sxs-lookup"><span data-stu-id="83951-162">string</span></span>             | <span data-ttu-id="83951-163">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="83951-163">The name / title of the item.</span></span>
| <span data-ttu-id="83951-164">**根**</span><span class="sxs-lookup"><span data-stu-id="83951-164">**root**</span></span>                 | <span data-ttu-id="83951-165">[根][]</span><span class="sxs-lookup"><span data-stu-id="83951-165">[root][]</span></span>           | <span data-ttu-id="83951-p106">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="83951-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="83951-168">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="83951-168">**sharepointIds**</span></span>        | <span data-ttu-id="83951-169">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="83951-169">[sharepointIds][]</span></span>  | <span data-ttu-id="83951-p107">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="83951-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="83951-172">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="83951-172">**siteCollection**</span></span>       | <span data-ttu-id="83951-173">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="83951-173">[siteCollection][]</span></span> | <span data-ttu-id="83951-p108">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="83951-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="83951-177">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="83951-177">**webUrl**</span></span>               | <span data-ttu-id="83951-178">string (url)</span><span class="sxs-lookup"><span data-stu-id="83951-178">string (url)</span></span>       | <span data-ttu-id="83951-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="83951-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="83951-181">关系</span><span class="sxs-lookup"><span data-stu-id="83951-181">Relationships</span></span>

| <span data-ttu-id="83951-182">关系名称</span><span class="sxs-lookup"><span data-stu-id="83951-182">Relationship name</span></span> | <span data-ttu-id="83951-183">类型</span><span class="sxs-lookup"><span data-stu-id="83951-183">Type</span></span>                             | <span data-ttu-id="83951-184">说明</span><span class="sxs-lookup"><span data-stu-id="83951-184">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="83951-185">**analytics**</span><span class="sxs-lookup"><span data-stu-id="83951-185">**analytics**</span></span>     | <span data-ttu-id="83951-186">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="83951-186">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="83951-187">此网站上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="83951-187">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="83951-188">**columns**</span><span class="sxs-lookup"><span data-stu-id="83951-188">**columns**</span></span>       | <span data-ttu-id="83951-189">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="83951-189">Collection([columnDefinition][])</span></span> | <span data-ttu-id="83951-190">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="83951-190">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="83951-191">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="83951-191">**contentTypes**</span></span>  | <span data-ttu-id="83951-192">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="83951-192">Collection([contentType][])</span></span>      | <span data-ttu-id="83951-193">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="83951-193">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="83951-194">**drive**</span><span class="sxs-lookup"><span data-stu-id="83951-194">**drive**</span></span>         | <span data-ttu-id="83951-195">[drive][]</span><span class="sxs-lookup"><span data-stu-id="83951-195">[drive][]</span></span>                        | <span data-ttu-id="83951-196">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="83951-196">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="83951-197">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="83951-197">**drives**</span></span>        | <span data-ttu-id="83951-198">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="83951-198">Collection([drive][])</span></span>            | <span data-ttu-id="83951-199">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="83951-199">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="83951-200">**项目**</span><span class="sxs-lookup"><span data-stu-id="83951-200">**items**</span></span>         | <span data-ttu-id="83951-201">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="83951-201">Collection([baseItem][])</span></span>         | <span data-ttu-id="83951-p110">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="83951-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="83951-204">**lists**</span><span class="sxs-lookup"><span data-stu-id="83951-204">**lists**</span></span>         | <span data-ttu-id="83951-205">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="83951-205">Collection([list][])</span></span>             | <span data-ttu-id="83951-206">此网站下的列表集合。</span><span class="sxs-lookup"><span data-stu-id="83951-206">The collection of lists under this site.</span></span>
| <span data-ttu-id="83951-207">**pages**</span><span class="sxs-lookup"><span data-stu-id="83951-207">**pages**</span></span>         | <span data-ttu-id="83951-208">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="83951-208">Collection([sitePage][])</span></span>         | <span data-ttu-id="83951-209">此网站的 SitePages 列表中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="83951-209">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="83951-210">**sites**</span><span class="sxs-lookup"><span data-stu-id="83951-210">**sites**</span></span>         | <span data-ttu-id="83951-211">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="83951-211">Collection([site][])</span></span>             | <span data-ttu-id="83951-212">网站下的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="83951-212">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="83951-224">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83951-224">JSON representation</span></span>

<span data-ttu-id="83951-225">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83951-225">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="83951-226">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="83951-226">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
