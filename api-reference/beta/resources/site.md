---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 17b9b8731a2b4e4ce39fa2ee10535bcb302f1be3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514801"
---
# <a name="site-resource-type"></a><span data-ttu-id="8593c-102">site 资源类型</span><span class="sxs-lookup"><span data-stu-id="8593c-102">site resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8593c-103">**site** 资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="8593c-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="8593c-104">方法</span><span class="sxs-lookup"><span data-stu-id="8593c-104">Methods</span></span>

| <span data-ttu-id="8593c-105">方法</span><span class="sxs-lookup"><span data-stu-id="8593c-105">Method</span></span>                         | <span data-ttu-id="8593c-106">REST 路径</span><span class="sxs-lookup"><span data-stu-id="8593c-106">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="8593c-107">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="8593c-107">[Get root site][]</span></span>              | <span data-ttu-id="8593c-108">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="8593c-108">GET /sites/root</span></span>
| <span data-ttu-id="8593c-109">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="8593c-109">[Get site][]</span></span>                   | <span data-ttu-id="8593c-110">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="8593c-110">GET /sites/{site-id}</span></span>
| <span data-ttu-id="8593c-111">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="8593c-111">[Get site by path][]</span></span>           | <span data-ttu-id="8593c-112">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="8593c-112">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="8593c-113">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="8593c-113">[Get site for a group][]</span></span>       | <span data-ttu-id="8593c-114">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="8593c-114">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="8593c-115">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="8593c-115">[Get analytics][]</span></span>              | <span data-ttu-id="8593c-116">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="8593c-116">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="8593c-117">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="8593c-117">[Get activities by interval][]</span></span> | <span data-ttu-id="8593c-118">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="8593c-118">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="8593c-119">[列出页面][]</span><span class="sxs-lookup"><span data-stu-id="8593c-119">[List pages][]</span></span>                 | <span data-ttu-id="8593c-120">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="8593c-120">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="8593c-121">[列出根网站][]</span><span class="sxs-lookup"><span data-stu-id="8593c-121">[List root sites][]</span></span>            | <span data-ttu-id="8593c-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="8593c-122">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="8593c-123">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="8593c-123">[Search for sites][]</span></span>           | <span data-ttu-id="8593c-124">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="8593c-124">GET /sites?search={query}</span></span>

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


## <a name="properties"></a><span data-ttu-id="8593c-134">属性</span><span class="sxs-lookup"><span data-stu-id="8593c-134">Properties</span></span>

| <span data-ttu-id="8593c-135">属性名称</span><span class="sxs-lookup"><span data-stu-id="8593c-135">Property name</span></span>            | <span data-ttu-id="8593c-136">类型</span><span class="sxs-lookup"><span data-stu-id="8593c-136">Type</span></span>               | <span data-ttu-id="8593c-137">说明</span><span class="sxs-lookup"><span data-stu-id="8593c-137">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="8593c-138">**id**</span><span class="sxs-lookup"><span data-stu-id="8593c-138">**id**</span></span>                   | <span data-ttu-id="8593c-139">string</span><span class="sxs-lookup"><span data-stu-id="8593c-139">string</span></span>             | <span data-ttu-id="8593c-p101">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="8593c-p101">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="8593c-142">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="8593c-142">**createdDateTime**</span></span>      | <span data-ttu-id="8593c-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8593c-143">DateTimeOffset</span></span>     | <span data-ttu-id="8593c-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="8593c-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="8593c-146">**说明**</span><span class="sxs-lookup"><span data-stu-id="8593c-146">**description**</span></span>          | <span data-ttu-id="8593c-147">string</span><span class="sxs-lookup"><span data-stu-id="8593c-147">string</span></span>             | <span data-ttu-id="8593c-148">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="8593c-148">The descriptive text for the site.</span></span>
| <span data-ttu-id="8593c-149">**eTag**</span><span class="sxs-lookup"><span data-stu-id="8593c-149">**eTag**</span></span>                 | <span data-ttu-id="8593c-150">string</span><span class="sxs-lookup"><span data-stu-id="8593c-150">string</span></span>             | <span data-ttu-id="8593c-p103">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="8593c-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="8593c-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="8593c-153">**displayName**</span></span>          | <span data-ttu-id="8593c-154">string</span><span class="sxs-lookup"><span data-stu-id="8593c-154">string</span></span>             | <span data-ttu-id="8593c-p104">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="8593c-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="8593c-157">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="8593c-157">**lastModifiedDateTime**</span></span> | <span data-ttu-id="8593c-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8593c-158">DateTimeOffset</span></span>     | <span data-ttu-id="8593c-p105">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="8593c-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="8593c-161">**name**</span><span class="sxs-lookup"><span data-stu-id="8593c-161">**name**</span></span>                 | <span data-ttu-id="8593c-162">string</span><span class="sxs-lookup"><span data-stu-id="8593c-162">string</span></span>             | <span data-ttu-id="8593c-163">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="8593c-163">The name / title of the item.</span></span>
| <span data-ttu-id="8593c-164">**根**</span><span class="sxs-lookup"><span data-stu-id="8593c-164">**root**</span></span>                 | <span data-ttu-id="8593c-165">[根][]</span><span class="sxs-lookup"><span data-stu-id="8593c-165">[root][]</span></span>           | <span data-ttu-id="8593c-p106">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="8593c-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="8593c-168">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="8593c-168">**sharepointIds**</span></span>        | <span data-ttu-id="8593c-169">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="8593c-169">[sharepointIds][]</span></span>  | <span data-ttu-id="8593c-p107">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="8593c-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="8593c-172">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="8593c-172">**siteCollection**</span></span>       | <span data-ttu-id="8593c-173">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="8593c-173">[siteCollection][]</span></span> | <span data-ttu-id="8593c-p108">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="8593c-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="8593c-177">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="8593c-177">**webUrl**</span></span>               | <span data-ttu-id="8593c-178">string (url)</span><span class="sxs-lookup"><span data-stu-id="8593c-178">string (url)</span></span>       | <span data-ttu-id="8593c-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="8593c-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="8593c-181">关系</span><span class="sxs-lookup"><span data-stu-id="8593c-181">Relationships</span></span>

| <span data-ttu-id="8593c-182">关系名称</span><span class="sxs-lookup"><span data-stu-id="8593c-182">Relationship name</span></span> | <span data-ttu-id="8593c-183">类型</span><span class="sxs-lookup"><span data-stu-id="8593c-183">Type</span></span>                             | <span data-ttu-id="8593c-184">说明</span><span class="sxs-lookup"><span data-stu-id="8593c-184">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="8593c-185">**analytics**</span><span class="sxs-lookup"><span data-stu-id="8593c-185">**analytics**</span></span>     | <span data-ttu-id="8593c-186">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="8593c-186">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="8593c-187">此网站上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="8593c-187">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="8593c-188">**columns**</span><span class="sxs-lookup"><span data-stu-id="8593c-188">**columns**</span></span>       | <span data-ttu-id="8593c-189">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="8593c-189">Collection([columnDefinition][])</span></span> | <span data-ttu-id="8593c-190">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="8593c-190">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="8593c-191">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="8593c-191">**contentTypes**</span></span>  | <span data-ttu-id="8593c-192">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="8593c-192">Collection([contentType][])</span></span>      | <span data-ttu-id="8593c-193">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="8593c-193">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="8593c-194">**drive**</span><span class="sxs-lookup"><span data-stu-id="8593c-194">**drive**</span></span>         | <span data-ttu-id="8593c-195">[drive][]</span><span class="sxs-lookup"><span data-stu-id="8593c-195">[drive][]</span></span>                        | <span data-ttu-id="8593c-196">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="8593c-196">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="8593c-197">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="8593c-197">**drives**</span></span>        | <span data-ttu-id="8593c-198">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="8593c-198">Collection([drive][])</span></span>            | <span data-ttu-id="8593c-199">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="8593c-199">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="8593c-200">**项目**</span><span class="sxs-lookup"><span data-stu-id="8593c-200">**items**</span></span>         | <span data-ttu-id="8593c-201">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="8593c-201">Collection([baseItem][])</span></span>         | <span data-ttu-id="8593c-p110">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="8593c-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="8593c-204">**lists**</span><span class="sxs-lookup"><span data-stu-id="8593c-204">**lists**</span></span>         | <span data-ttu-id="8593c-205">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="8593c-205">Collection([list][])</span></span>             | <span data-ttu-id="8593c-206">此网站下的列表集合。</span><span class="sxs-lookup"><span data-stu-id="8593c-206">The collection of lists under this site.</span></span>
| <span data-ttu-id="8593c-207">**pages**</span><span class="sxs-lookup"><span data-stu-id="8593c-207">**pages**</span></span>         | <span data-ttu-id="8593c-208">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="8593c-208">Collection([sitePage][])</span></span>         | <span data-ttu-id="8593c-209">此网站的 SitePages 列表中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="8593c-209">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="8593c-210">**sites**</span><span class="sxs-lookup"><span data-stu-id="8593c-210">**sites**</span></span>         | <span data-ttu-id="8593c-211">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="8593c-211">Collection([site][])</span></span>             | <span data-ttu-id="8593c-212">网站下的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="8593c-212">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="8593c-224">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8593c-224">JSON representation</span></span>

<span data-ttu-id="8593c-225">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8593c-225">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="8593c-226">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="8593c-226">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/site.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
