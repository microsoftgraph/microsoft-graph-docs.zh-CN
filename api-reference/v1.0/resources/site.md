---
author: JeremyKelley
ms.author: JeremyKelley
title: site 资源
description: site 资源提供 Sharepoint 网站的元数据和关系。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a4e67deb63850bdc938f72f5e517bc28a5a8df03
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934855"
---
# <a name="site-resource"></a><span data-ttu-id="736de-103">site 资源</span><span class="sxs-lookup"><span data-stu-id="736de-103">site resource</span></span>

<span data-ttu-id="736de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="736de-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="736de-105">**site** 资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="736de-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="736de-106">方法</span><span class="sxs-lookup"><span data-stu-id="736de-106">Methods</span></span>

| <span data-ttu-id="736de-107">方法</span><span class="sxs-lookup"><span data-stu-id="736de-107">Method</span></span>                | <span data-ttu-id="736de-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="736de-108">Return type</span></span> | <span data-ttu-id="736de-109">说明</span><span class="sxs-lookup"><span data-stu-id="736de-109">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="736de-110">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="736de-110">[Get root site][]</span></span>        | <span data-ttu-id="736de-111">网站</span><span class="sxs-lookup"><span data-stu-id="736de-111">site</span></span> | <span data-ttu-id="736de-112">访问租户内的根 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="736de-112">Access the root SharePoint site within a tenant.</span></span>
| <span data-ttu-id="736de-113">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="736de-113">[Get site][]</span></span>             | <span data-ttu-id="736de-114">网站</span><span class="sxs-lookup"><span data-stu-id="736de-114">site</span></span> | <span data-ttu-id="736de-115">使用 siteId 访问 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="736de-115">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="736de-116">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="736de-116">[Get site by path][]</span></span>     | <span data-ttu-id="736de-117">网站</span><span class="sxs-lookup"><span data-stu-id="736de-117">site</span></span> | <span data-ttu-id="736de-118">通过相对路径访问根 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="736de-118">Access the root SharePoint site with a relative path.</span></span>
| <span data-ttu-id="736de-119">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="736de-119">[Get site for a group][]</span></span> | <span data-ttu-id="736de-120">网站</span><span class="sxs-lookup"><span data-stu-id="736de-120">site</span></span> | <span data-ttu-id="736de-121">访问组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="736de-121">Access the team site for a group.</span></span>
| <span data-ttu-id="736de-122">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="736de-122">[Get analytics][]</span></span>              | <span data-ttu-id="736de-123">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="736de-123">[itemAnalytics][]</span></span> | <span data-ttu-id="736de-124">对此资源可获取分析。</span><span class="sxs-lookup"><span data-stu-id="736de-124">Get analytics for this resource.</span></span> 
| <span data-ttu-id="736de-125">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="736de-125">[Get activities by interval][]</span></span> | <span data-ttu-id="736de-126">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="736de-126">[itemActivityStat][]</span></span> | <span data-ttu-id="736de-127">在指定的时间间隔内获取 **itemActivityStats** 的集合。</span><span class="sxs-lookup"><span data-stu-id="736de-127">Get a collection of **itemActivityStats** within the specified time interval.</span></span>
| <span data-ttu-id="736de-128">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="736de-128">[Search for sites][]</span></span>     | <span data-ttu-id="736de-129">网站集合</span><span class="sxs-lookup"><span data-stu-id="736de-129">collection of site</span></span> | <span data-ttu-id="736de-130">在 SharePoint 租户中搜索与所提供的关键字匹配的 网站。</span><span class="sxs-lookup"><span data-stu-id="736de-130">Search across a SharePoint tenant for sites that match keywords provided.</span></span>
| <span data-ttu-id="736de-131">[关注网站][]</span><span class="sxs-lookup"><span data-stu-id="736de-131">[Follow site][]</span></span>          | <span data-ttu-id="736de-132">网站集合</span><span class="sxs-lookup"><span data-stu-id="736de-132">collection of site</span></span> | <span data-ttu-id="736de-133">关注用户的网站或多个网站。</span><span class="sxs-lookup"><span data-stu-id="736de-133">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="736de-134">[取消关注网站][]</span><span class="sxs-lookup"><span data-stu-id="736de-134">[Unfollow site][]</span></span>        | <span data-ttu-id="736de-135">网站集合</span><span class="sxs-lookup"><span data-stu-id="736de-135">collection of site</span></span> | <span data-ttu-id="736de-136">关注用户的网站或多个网站。</span><span class="sxs-lookup"><span data-stu-id="736de-136">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="736de-137">[关注网站列表][]</span><span class="sxs-lookup"><span data-stu-id="736de-137">[List followed sites][]</span></span>  | <span data-ttu-id="736de-138">网站集合</span><span class="sxs-lookup"><span data-stu-id="736de-138">collection of site</span></span> | <span data-ttu-id="736de-139">已登录用户的关注网站列表。</span><span class="sxs-lookup"><span data-stu-id="736de-139">List the sites that have been followed by the signed in user.</span></span>

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
[关注网站]: ../api/site-follow.md
[Follow site]: ../api/site-follow.md
[取消关注网站]: ../api/site-unfollow.md
[Unfollow site]: ../api/site-unfollow.md
[关注网站列表]: ../api/sites-list-followed.md
[List followed sites]: ../api/sites-list-followed.md

## <a name="properties"></a><span data-ttu-id="736de-151">属性</span><span class="sxs-lookup"><span data-stu-id="736de-151">Properties</span></span>

| <span data-ttu-id="736de-152">属性</span><span class="sxs-lookup"><span data-stu-id="736de-152">Property</span></span>            | <span data-ttu-id="736de-153">类型</span><span class="sxs-lookup"><span data-stu-id="736de-153">Type</span></span>                                | <span data-ttu-id="736de-154">说明</span><span class="sxs-lookup"><span data-stu-id="736de-154">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="736de-155">**id**</span><span class="sxs-lookup"><span data-stu-id="736de-155">**id**</span></span>                   | <span data-ttu-id="736de-156">string</span><span class="sxs-lookup"><span data-stu-id="736de-156">string</span></span>                              | <span data-ttu-id="736de-p101">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="736de-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="736de-159">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="736de-159">**createdDateTime**</span></span>      | <span data-ttu-id="736de-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="736de-160">DateTimeOffset</span></span>                      | <span data-ttu-id="736de-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="736de-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="736de-163">**说明**</span><span class="sxs-lookup"><span data-stu-id="736de-163">**description**</span></span>          | <span data-ttu-id="736de-164">string</span><span class="sxs-lookup"><span data-stu-id="736de-164">string</span></span>                              | <span data-ttu-id="736de-165">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="736de-165">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="736de-166">**displayName**</span><span class="sxs-lookup"><span data-stu-id="736de-166">**displayName**</span></span>          | <span data-ttu-id="736de-167">string</span><span class="sxs-lookup"><span data-stu-id="736de-167">string</span></span>                              | <span data-ttu-id="736de-p103">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="736de-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="736de-170">**eTag**</span><span class="sxs-lookup"><span data-stu-id="736de-170">**eTag**</span></span>                 | <span data-ttu-id="736de-171">string</span><span class="sxs-lookup"><span data-stu-id="736de-171">string</span></span>                              | <span data-ttu-id="736de-p104">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="736de-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="736de-174">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="736de-174">**lastModifiedDateTime**</span></span> | <span data-ttu-id="736de-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="736de-175">DateTimeOffset</span></span>                      | <span data-ttu-id="736de-p105">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="736de-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="736de-178">**name**</span><span class="sxs-lookup"><span data-stu-id="736de-178">**name**</span></span>                 | <span data-ttu-id="736de-179">string</span><span class="sxs-lookup"><span data-stu-id="736de-179">string</span></span>                              | <span data-ttu-id="736de-180">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="736de-180">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="736de-181">**根**</span><span class="sxs-lookup"><span data-stu-id="736de-181">**root**</span></span>                 | [<span data-ttu-id="736de-182">根</span><span class="sxs-lookup"><span data-stu-id="736de-182">root</span></span>](root.md)                     | <span data-ttu-id="736de-p106">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="736de-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="736de-185">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="736de-185">**sharepointIds**</span></span>        | [<span data-ttu-id="736de-186">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="736de-186">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="736de-p107">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="736de-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="736de-189">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="736de-189">**siteCollection**</span></span>       | [<span data-ttu-id="736de-190">siteCollection</span><span class="sxs-lookup"><span data-stu-id="736de-190">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="736de-p108">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="736de-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="736de-194">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="736de-194">**webUrl**</span></span>               | <span data-ttu-id="736de-195">string (url)</span><span class="sxs-lookup"><span data-stu-id="736de-195">string (url)</span></span>                        | <span data-ttu-id="736de-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="736de-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

### <a name="id-property"></a><span data-ttu-id="736de-198">id 属性</span><span class="sxs-lookup"><span data-stu-id="736de-198">id property</span></span>
<span data-ttu-id="736de-199">**site** 由一个唯一 ID 标识，此唯一 ID 由以下值组成：</span><span class="sxs-lookup"><span data-stu-id="736de-199">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="736de-200">网站集主机名称 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="736de-200">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="736de-201">网站集的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="736de-201">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="736de-202">网站的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="736de-202">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="736de-203">`root` 标识符经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="736de-203">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="736de-204">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="736de-204">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="736de-205">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="736de-205">`/groups/{group-id}/sites/root`: The group's team site.</span></span>
  
## <a name="relationships"></a><span data-ttu-id="736de-206">关系</span><span class="sxs-lookup"><span data-stu-id="736de-206">Relationships</span></span>

| <span data-ttu-id="736de-207">关系</span><span class="sxs-lookup"><span data-stu-id="736de-207">Relationship</span></span>      | <span data-ttu-id="736de-208">类型</span><span class="sxs-lookup"><span data-stu-id="736de-208">Type</span></span>                             | <span data-ttu-id="736de-209">说明</span><span class="sxs-lookup"><span data-stu-id="736de-209">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="736de-210">**analytics**</span><span class="sxs-lookup"><span data-stu-id="736de-210">**analytics**</span></span>     | <span data-ttu-id="736de-211">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="736de-211">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="736de-212">此网站上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="736de-212">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="736de-213">**columns**</span><span class="sxs-lookup"><span data-stu-id="736de-213">**columns**</span></span>       | <span data-ttu-id="736de-214">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="736de-214">Collection([columnDefinition][])</span></span> | <span data-ttu-id="736de-215">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="736de-215">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="736de-216">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="736de-216">**contentTypes**</span></span>  | <span data-ttu-id="736de-217">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="736de-217">Collection([contentType][])</span></span>      | <span data-ttu-id="736de-218">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="736de-218">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="736de-219">**drive**</span><span class="sxs-lookup"><span data-stu-id="736de-219">**drive**</span></span>         | <span data-ttu-id="736de-220">[drive][]</span><span class="sxs-lookup"><span data-stu-id="736de-220">[drive][]</span></span>                        | <span data-ttu-id="736de-221">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="736de-221">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="736de-222">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="736de-222">**drives**</span></span>        | <span data-ttu-id="736de-223">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="736de-223">Collection([drive][])</span></span>            | <span data-ttu-id="736de-224">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="736de-224">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="736de-225">**项目**</span><span class="sxs-lookup"><span data-stu-id="736de-225">**items**</span></span>         | <span data-ttu-id="736de-226">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="736de-226">Collection([baseItem][])</span></span>         | <span data-ttu-id="736de-p110">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="736de-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="736de-229">**lists**</span><span class="sxs-lookup"><span data-stu-id="736de-229">**lists**</span></span>         | <span data-ttu-id="736de-230">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="736de-230">Collection([list][])</span></span>             | <span data-ttu-id="736de-231">此网站下方的列表集合。</span><span class="sxs-lookup"><span data-stu-id="736de-231">The collection of lists under this site.</span></span>
| <span data-ttu-id="736de-232">**sites**</span><span class="sxs-lookup"><span data-stu-id="736de-232">**sites**</span></span>         | <span data-ttu-id="736de-233">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="736de-233">Collection([site][])</span></span>             | <span data-ttu-id="736de-234">网站下方的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="736de-234">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="736de-235">**onenote**</span><span class="sxs-lookup"><span data-stu-id="736de-235">**onenote**</span></span>       | <span data-ttu-id="736de-236">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="736de-236">[onenote][]</span></span>                      | <span data-ttu-id="736de-237">调用 OneNote 服务执行笔记本相关操作。</span><span class="sxs-lookup"><span data-stu-id="736de-237">Calls the OneNote service for notebook related operations.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="736de-246">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="736de-246">JSON representation</span></span>

<span data-ttu-id="736de-247">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="736de-247">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="736de-248">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="736de-248">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
