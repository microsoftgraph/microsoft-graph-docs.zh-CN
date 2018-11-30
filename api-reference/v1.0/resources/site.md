---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Site
ms.openlocfilehash: db465f93f336a51d862daf6e05b1d6bc422247ea
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="site-resource"></a><span data-ttu-id="9423d-102">Site 资源</span><span class="sxs-lookup"><span data-stu-id="9423d-102">Site resource</span></span>

<span data-ttu-id="9423d-103">**网站**资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="9423d-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="9423d-104">任务</span><span class="sxs-lookup"><span data-stu-id="9423d-104">Tasks</span></span>

<span data-ttu-id="9423d-105">下面的所有示例都相对于 `https://graph.microsoft.com/v1.0`。</span><span class="sxs-lookup"><span data-stu-id="9423d-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="9423d-106">任务名称</span><span class="sxs-lookup"><span data-stu-id="9423d-106">Task name</span></span>                | <span data-ttu-id="9423d-107">示例请求</span><span class="sxs-lookup"><span data-stu-id="9423d-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="9423d-108">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="9423d-108">[Get root site][]</span></span>        | <span data-ttu-id="9423d-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="9423d-109">GET /sites/root</span></span>
| <span data-ttu-id="9423d-110">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="9423d-110">[Get site][]</span></span>             | <span data-ttu-id="9423d-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="9423d-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="9423d-112">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="9423d-112">[Get site by path][]</span></span>     | <span data-ttu-id="9423d-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="9423d-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="9423d-114">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="9423d-114">[Get site for a group][]</span></span> | <span data-ttu-id="9423d-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="9423d-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="9423d-116">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="9423d-116">[Search for sites][]</span></span>     | <span data-ttu-id="9423d-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="9423d-117">GET /sites?search={query}</span></span>

[获取网站]: ../api/site_get.md
[获取根网站]: ../api/site_get.md
[按路径获取网站]: ../api/site_getbypath.md
[获取组的网站]: ../api/site_get.md
[搜索网站]: ../api/site_search.md

## <a name="json-representation"></a><span data-ttu-id="9423d-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9423d-123">JSON representation</span></span>

<span data-ttu-id="9423d-124">下面是**网站**资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9423d-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="9423d-125">**driveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="9423d-125">The **driveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- { "blockType": "resource",
       "@odata.type": "microsoft.graph.site",
       "keyProperty": "id",
       "optionalProperties": [ "root", "sharepointIds", "siteCollection", "drive", "drives", "sites" ] } -->

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
  "onenote": [ { "@odata.type": "microsoft.graph.onenote"} ],

  /* inherited from baseItem */
  "name": "string",
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedDateTime": "datetime",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="9423d-126">属性</span><span class="sxs-lookup"><span data-stu-id="9423d-126">Properties</span></span>

| <span data-ttu-id="9423d-127">属性名称</span><span class="sxs-lookup"><span data-stu-id="9423d-127">Property name</span></span>            | <span data-ttu-id="9423d-128">类型</span><span class="sxs-lookup"><span data-stu-id="9423d-128">Type</span></span>                                | <span data-ttu-id="9423d-129">说明</span><span class="sxs-lookup"><span data-stu-id="9423d-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9423d-130">**id**</span><span class="sxs-lookup"><span data-stu-id="9423d-130">**id**</span></span>                   | <span data-ttu-id="9423d-131">string</span><span class="sxs-lookup"><span data-stu-id="9423d-131">string</span></span>                              | <span data-ttu-id="9423d-p101">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="9423d-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="9423d-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="9423d-134">**createdDateTime**</span></span>      | <span data-ttu-id="9423d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9423d-135">DateTimeOffset</span></span>                      | <span data-ttu-id="9423d-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="9423d-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="9423d-138">**说明**</span><span class="sxs-lookup"><span data-stu-id="9423d-138">**description**</span></span>          | <span data-ttu-id="9423d-139">string</span><span class="sxs-lookup"><span data-stu-id="9423d-139">string</span></span>                              | <span data-ttu-id="9423d-140">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="9423d-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="9423d-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="9423d-141">**displayName**</span></span>          | <span data-ttu-id="9423d-142">string</span><span class="sxs-lookup"><span data-stu-id="9423d-142">string</span></span>                              | <span data-ttu-id="9423d-p103">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="9423d-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="9423d-145">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="9423d-145">**lastModifiedDateTime**</span></span> | <span data-ttu-id="9423d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9423d-146">DateTimeOffset</span></span>                      | <span data-ttu-id="9423d-p104">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="9423d-p104">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="9423d-149">**name**</span><span class="sxs-lookup"><span data-stu-id="9423d-149">**name**</span></span>                 | <span data-ttu-id="9423d-150">string</span><span class="sxs-lookup"><span data-stu-id="9423d-150">string</span></span>                              | <span data-ttu-id="9423d-151">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="9423d-151">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="9423d-152">**根**</span><span class="sxs-lookup"><span data-stu-id="9423d-152">**root**</span></span>                 | [<span data-ttu-id="9423d-153">根</span><span class="sxs-lookup"><span data-stu-id="9423d-153">root</span></span>](root.md)                     | <span data-ttu-id="9423d-p105">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="9423d-p105">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="9423d-156">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="9423d-156">**sharepointIds**</span></span>        | [<span data-ttu-id="9423d-157">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="9423d-157">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="9423d-p106">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="9423d-p106">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="9423d-160">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="9423d-160">**siteCollection**</span></span>       | [<span data-ttu-id="9423d-161">siteCollection</span><span class="sxs-lookup"><span data-stu-id="9423d-161">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="9423d-p107">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="9423d-p107">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="9423d-165">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="9423d-165">**webUrl**</span></span>               | <span data-ttu-id="9423d-166">string (url)</span><span class="sxs-lookup"><span data-stu-id="9423d-166">string (url)</span></span>                        | <span data-ttu-id="9423d-p108">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="9423d-p108">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="9423d-169">关系</span><span class="sxs-lookup"><span data-stu-id="9423d-169">Relationships</span></span>

| <span data-ttu-id="9423d-170">关系名称</span><span class="sxs-lookup"><span data-stu-id="9423d-170">Relationship name</span></span> | <span data-ttu-id="9423d-171">类型</span><span class="sxs-lookup"><span data-stu-id="9423d-171">Type</span></span>                             | <span data-ttu-id="9423d-172">说明</span><span class="sxs-lookup"><span data-stu-id="9423d-172">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="9423d-173">**columns**</span><span class="sxs-lookup"><span data-stu-id="9423d-173">**columns**</span></span>       | <span data-ttu-id="9423d-174">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="9423d-174">Collection([columnDefinition][])</span></span> | <span data-ttu-id="9423d-175">可以在此网站下方的列表中重复使用列定义的集合。</span><span class="sxs-lookup"><span data-stu-id="9423d-175">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="9423d-176">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="9423d-176"><ContentTypes></span></span>  | <span data-ttu-id="9423d-177">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="9423d-177">Collection([contentType][])</span></span>      | <span data-ttu-id="9423d-178">为此网站定义的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="9423d-178">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="9423d-179">**drive**</span><span class="sxs-lookup"><span data-stu-id="9423d-179">**drive**</span></span>         | <span data-ttu-id="9423d-180">[驱动器][]</span><span class="sxs-lookup"><span data-stu-id="9423d-180">[drive][]</span></span>                        | <span data-ttu-id="9423d-181">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="9423d-181">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="9423d-182">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="9423d-182">**drives**</span></span>        | <span data-ttu-id="9423d-183">集合（[驱动器][]）</span><span class="sxs-lookup"><span data-stu-id="9423d-183">Collection([drive][])</span></span>            | <span data-ttu-id="9423d-184">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="9423d-184">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="9423d-185">**项目**</span><span class="sxs-lookup"><span data-stu-id="9423d-185">**items**</span></span>         | <span data-ttu-id="9423d-186">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="9423d-186">Collection([baseItem][])</span></span>         | <span data-ttu-id="9423d-p109">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="9423d-p109">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="9423d-189">**lists**</span><span class="sxs-lookup"><span data-stu-id="9423d-189">**Lists**</span></span>         | <span data-ttu-id="9423d-190">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="9423d-190">Collection([list][])</span></span>             | <span data-ttu-id="9423d-191">此网站下方的列表的集合。</span><span class="sxs-lookup"><span data-stu-id="9423d-191">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="9423d-192">**sites**</span><span class="sxs-lookup"><span data-stu-id="9423d-192">**sites**</span></span>         | <span data-ttu-id="9423d-193">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="9423d-193">Collection([site][])</span></span>             | <span data-ttu-id="9423d-194">网站下方的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="9423d-194">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="9423d-195">**onenote**</span><span class="sxs-lookup"><span data-stu-id="9423d-195">**onenote**</span></span>       | <span data-ttu-id="9423d-196">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="9423d-196">[onenote][]</span></span>                      | <span data-ttu-id="9423d-197">调用 OneNote 服务执行笔记本相关操作。</span><span class="sxs-lookup"><span data-stu-id="9423d-197">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contentType.md
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
