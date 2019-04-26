---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: d4dfb3f340a2b2b7ff5ad5a3c9279cb2a03c63be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549599"
---
# <a name="site-resource"></a><span data-ttu-id="cf3a2-102">Site 资源</span><span class="sxs-lookup"><span data-stu-id="cf3a2-102">Site resource</span></span>

<span data-ttu-id="cf3a2-103">**网站**资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-103">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="tasks"></a><span data-ttu-id="cf3a2-104">任务</span><span class="sxs-lookup"><span data-stu-id="cf3a2-104">Tasks</span></span>

<span data-ttu-id="cf3a2-105">下面的所有示例都相对于 `https://graph.microsoft.com/v1.0`。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-105">All examples below are relative to `https://graph.microsoft.com/v1.0`.</span></span>

| <span data-ttu-id="cf3a2-106">任务名称</span><span class="sxs-lookup"><span data-stu-id="cf3a2-106">Task name</span></span>                | <span data-ttu-id="cf3a2-107">示例请求</span><span class="sxs-lookup"><span data-stu-id="cf3a2-107">Example Request</span></span>
|:-------------------------|:--------------------------------------------------
| <span data-ttu-id="cf3a2-108">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="cf3a2-108">[Get root site][]</span></span>        | <span data-ttu-id="cf3a2-109">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="cf3a2-109">GET /sites/root</span></span>
| <span data-ttu-id="cf3a2-110">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="cf3a2-110">[Get site][]</span></span>             | <span data-ttu-id="cf3a2-111">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="cf3a2-111">GET /sites/{site-id}</span></span>
| <span data-ttu-id="cf3a2-112">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="cf3a2-112">[Get site by path][]</span></span>     | <span data-ttu-id="cf3a2-113">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="cf3a2-113">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="cf3a2-114">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="cf3a2-114">[Get site for a group][]</span></span> | <span data-ttu-id="cf3a2-115">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="cf3a2-115">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="cf3a2-116">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="cf3a2-116">[Search for sites][]</span></span>     | <span data-ttu-id="cf3a2-117">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="cf3a2-117">GET /sites?search={query}</span></span>

[获取网站]: ../api/site-get.md
[Get site]: ../api/site-get.md
[获取根网站]: ../api/site-get.md
[Get root site]: ../api/site-get.md
[根据路径获取网站]: ../api/site-getbypath.md
[Get site by path]: ../api/site-getbypath.md
[获取组的网站]: ../api/site-get.md
[Get site for a group]: ../api/site-get.md
[搜索网站]: ../api/site-search.md
[Search for sites]: ../api/site-search.md

## <a name="json-representation"></a><span data-ttu-id="cf3a2-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf3a2-123">JSON representation</span></span>

<span data-ttu-id="cf3a2-124">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-124">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="cf3a2-125">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-125">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="cf3a2-126">属性</span><span class="sxs-lookup"><span data-stu-id="cf3a2-126">Properties</span></span>

| <span data-ttu-id="cf3a2-127">属性名称</span><span class="sxs-lookup"><span data-stu-id="cf3a2-127">Property name</span></span>            | <span data-ttu-id="cf3a2-128">类型</span><span class="sxs-lookup"><span data-stu-id="cf3a2-128">Type</span></span>                                | <span data-ttu-id="cf3a2-129">说明</span><span class="sxs-lookup"><span data-stu-id="cf3a2-129">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="cf3a2-130">**id**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-130">**id**</span></span>                   | <span data-ttu-id="cf3a2-131">string</span><span class="sxs-lookup"><span data-stu-id="cf3a2-131">string</span></span>                              | <span data-ttu-id="cf3a2-p101">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="cf3a2-134">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-134">**createdDateTime**</span></span>      | <span data-ttu-id="cf3a2-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf3a2-135">DateTimeOffset</span></span>                      | <span data-ttu-id="cf3a2-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="cf3a2-138">**说明**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-138">**description**</span></span>          | <span data-ttu-id="cf3a2-139">string</span><span class="sxs-lookup"><span data-stu-id="cf3a2-139">string</span></span>                              | <span data-ttu-id="cf3a2-140">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-140">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="cf3a2-141">**displayName**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-141">**displayName**</span></span>          | <span data-ttu-id="cf3a2-142">string</span><span class="sxs-lookup"><span data-stu-id="cf3a2-142">string</span></span>                              | <span data-ttu-id="cf3a2-p103">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="cf3a2-145">**eTag**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-145">**eTag**</span></span>                 | <span data-ttu-id="cf3a2-146">string</span><span class="sxs-lookup"><span data-stu-id="cf3a2-146">string</span></span>                              | <span data-ttu-id="cf3a2-p104">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="cf3a2-149">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-149">**lastModifiedDateTime**</span></span> | <span data-ttu-id="cf3a2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf3a2-150">DateTimeOffset</span></span>                      | <span data-ttu-id="cf3a2-p105">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="cf3a2-153">**name**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-153">**name**</span></span>                 | <span data-ttu-id="cf3a2-154">string</span><span class="sxs-lookup"><span data-stu-id="cf3a2-154">string</span></span>                              | <span data-ttu-id="cf3a2-155">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-155">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="cf3a2-156">**根**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-156">**root**</span></span>                 | [<span data-ttu-id="cf3a2-157">根</span><span class="sxs-lookup"><span data-stu-id="cf3a2-157">root</span></span>](root.md)                     | <span data-ttu-id="cf3a2-p106">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="cf3a2-160">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-160">**sharepointIds**</span></span>        | [<span data-ttu-id="cf3a2-161">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="cf3a2-161">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="cf3a2-p107">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="cf3a2-164">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-164">**siteCollection**</span></span>       | [<span data-ttu-id="cf3a2-165">siteCollection</span><span class="sxs-lookup"><span data-stu-id="cf3a2-165">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="cf3a2-p108">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="cf3a2-169">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-169">**webUrl**</span></span>               | <span data-ttu-id="cf3a2-170">string (url)</span><span class="sxs-lookup"><span data-stu-id="cf3a2-170">string (url)</span></span>                        | <span data-ttu-id="cf3a2-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

## <a name="relationships"></a><span data-ttu-id="cf3a2-173">关系</span><span class="sxs-lookup"><span data-stu-id="cf3a2-173">Relationships</span></span>

| <span data-ttu-id="cf3a2-174">关系名称</span><span class="sxs-lookup"><span data-stu-id="cf3a2-174">Relationship name</span></span> | <span data-ttu-id="cf3a2-175">类型</span><span class="sxs-lookup"><span data-stu-id="cf3a2-175">Type</span></span>                             | <span data-ttu-id="cf3a2-176">说明</span><span class="sxs-lookup"><span data-stu-id="cf3a2-176">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="cf3a2-177">**columns**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-177">**columns**</span></span>       | <span data-ttu-id="cf3a2-178">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="cf3a2-178">Collection([columnDefinition][])</span></span> | <span data-ttu-id="cf3a2-179">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-179">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="cf3a2-180">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-180">**contentTypes**</span></span>  | <span data-ttu-id="cf3a2-181">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="cf3a2-181">Collection([contentType][])</span></span>      | <span data-ttu-id="cf3a2-182">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-182">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="cf3a2-183">**drive**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-183">**drive**</span></span>         | <span data-ttu-id="cf3a2-184">[drive][]</span><span class="sxs-lookup"><span data-stu-id="cf3a2-184">[drive][]</span></span>                        | <span data-ttu-id="cf3a2-185">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-185">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="cf3a2-186">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-186">**drives**</span></span>        | <span data-ttu-id="cf3a2-187">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="cf3a2-187">Collection([drive][])</span></span>            | <span data-ttu-id="cf3a2-188">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-188">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="cf3a2-189">**项目**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-189">**items**</span></span>         | <span data-ttu-id="cf3a2-190">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="cf3a2-190">Collection([baseItem][])</span></span>         | <span data-ttu-id="cf3a2-p110">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="cf3a2-193">**lists**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-193">**lists**</span></span>         | <span data-ttu-id="cf3a2-194">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="cf3a2-194">Collection([list][])</span></span>             | <span data-ttu-id="cf3a2-195">此网站下方的列表集合。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-195">The collection of lists under this site.</span></span>
| <span data-ttu-id="cf3a2-196">**sites**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-196">**sites**</span></span>         | <span data-ttu-id="cf3a2-197">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="cf3a2-197">Collection([site][])</span></span>             | <span data-ttu-id="cf3a2-198">网站下方的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-198">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="cf3a2-199">**onenote**</span><span class="sxs-lookup"><span data-stu-id="cf3a2-199">**onenote**</span></span>       | <span data-ttu-id="cf3a2-200">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="cf3a2-200">[onenote][]</span></span>                      | <span data-ttu-id="cf3a2-201">调用 OneNote 服务执行笔记本相关操作。</span><span class="sxs-lookup"><span data-stu-id="cf3a2-201">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[list]: list.md
[网站]: site.md
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
