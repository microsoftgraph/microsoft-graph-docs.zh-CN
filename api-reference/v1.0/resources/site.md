---
author: JeremyKelley
ms.author: JeremyKelley
title: site 资源
description: site 资源提供 Sharepoint 网站的元数据和关系。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 43e321ef3b04124095257a6bf6b9d218ac080a3d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086443"
---
# <a name="site-resource"></a><span data-ttu-id="3a948-103">site 资源</span><span class="sxs-lookup"><span data-stu-id="3a948-103">site resource</span></span>

<span data-ttu-id="3a948-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a948-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a948-105">**site** 资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="3a948-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="3a948-106">方法</span><span class="sxs-lookup"><span data-stu-id="3a948-106">Methods</span></span>

| <span data-ttu-id="3a948-107">方法</span><span class="sxs-lookup"><span data-stu-id="3a948-107">Method</span></span>                | <span data-ttu-id="3a948-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3a948-108">Return type</span></span> | <span data-ttu-id="3a948-109">说明</span><span class="sxs-lookup"><span data-stu-id="3a948-109">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="3a948-110">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="3a948-110">[Get root site][]</span></span>        | <span data-ttu-id="3a948-111">网站</span><span class="sxs-lookup"><span data-stu-id="3a948-111">site</span></span> | <span data-ttu-id="3a948-112">访问租户内的根 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="3a948-112">Access the root SharePoint site within a tenant.</span></span>
| <span data-ttu-id="3a948-113">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="3a948-113">[Get site][]</span></span>             | <span data-ttu-id="3a948-114">网站</span><span class="sxs-lookup"><span data-stu-id="3a948-114">site</span></span> | <span data-ttu-id="3a948-115">使用 siteId 访问 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="3a948-115">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="3a948-116">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="3a948-116">[Get site by path][]</span></span>     | <span data-ttu-id="3a948-117">网站</span><span class="sxs-lookup"><span data-stu-id="3a948-117">site</span></span> | <span data-ttu-id="3a948-118">通过相对路径访问根 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="3a948-118">Access the root SharePoint site with a relative path.</span></span>
| <span data-ttu-id="3a948-119">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="3a948-119">[Get site for a group][]</span></span> | <span data-ttu-id="3a948-120">网站</span><span class="sxs-lookup"><span data-stu-id="3a948-120">site</span></span> | <span data-ttu-id="3a948-121">访问组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="3a948-121">Access the team site for a group.</span></span>
| <span data-ttu-id="3a948-122">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="3a948-122">[Get analytics][]</span></span>              | <span data-ttu-id="3a948-123">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="3a948-123">[itemAnalytics][]</span></span> | <span data-ttu-id="3a948-124">对此资源可获取分析。</span><span class="sxs-lookup"><span data-stu-id="3a948-124">Get analytics for this resource.</span></span> 
| <span data-ttu-id="3a948-125">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="3a948-125">[Get activities by interval][]</span></span> | <span data-ttu-id="3a948-126">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="3a948-126">[itemActivityStat][]</span></span> | <span data-ttu-id="3a948-127">在指定的时间间隔内获取 **itemActivityStats** 的集合。</span><span class="sxs-lookup"><span data-stu-id="3a948-127">Get a collection of **itemActivityStats** within the specified time interval.</span></span>
| <span data-ttu-id="3a948-128">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="3a948-128">[Search for sites][]</span></span>     | <span data-ttu-id="3a948-129">网站集合</span><span class="sxs-lookup"><span data-stu-id="3a948-129">collection of site</span></span> | <span data-ttu-id="3a948-130">在 SharePoint 租户中搜索与所提供的关键字匹配的 网站。</span><span class="sxs-lookup"><span data-stu-id="3a948-130">Search across a SharePoint tenant for sites that match keywords provided.</span></span>
| <span data-ttu-id="3a948-131">[关注网站][]</span><span class="sxs-lookup"><span data-stu-id="3a948-131">[Follow site][]</span></span>          | <span data-ttu-id="3a948-132">网站集合</span><span class="sxs-lookup"><span data-stu-id="3a948-132">collection of site</span></span> | <span data-ttu-id="3a948-133">关注用户的网站或多个网站。</span><span class="sxs-lookup"><span data-stu-id="3a948-133">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="3a948-134">[取消关注网站][]</span><span class="sxs-lookup"><span data-stu-id="3a948-134">[Unfollow site][]</span></span>        | <span data-ttu-id="3a948-135">网站集合</span><span class="sxs-lookup"><span data-stu-id="3a948-135">collection of site</span></span> | <span data-ttu-id="3a948-136">关注用户的网站或多个网站。</span><span class="sxs-lookup"><span data-stu-id="3a948-136">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="3a948-137">[关注网站列表][]</span><span class="sxs-lookup"><span data-stu-id="3a948-137">[List followed sites][]</span></span>  | <span data-ttu-id="3a948-138">网站集合</span><span class="sxs-lookup"><span data-stu-id="3a948-138">collection of site</span></span> | <span data-ttu-id="3a948-139">已登录用户的关注网站列表。</span><span class="sxs-lookup"><span data-stu-id="3a948-139">List the sites that have been followed by the signed in user.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3a948-151">属性</span><span class="sxs-lookup"><span data-stu-id="3a948-151">Properties</span></span>

| <span data-ttu-id="3a948-152">属性</span><span class="sxs-lookup"><span data-stu-id="3a948-152">Property</span></span>            | <span data-ttu-id="3a948-153">类型</span><span class="sxs-lookup"><span data-stu-id="3a948-153">Type</span></span>                                | <span data-ttu-id="3a948-154">说明</span><span class="sxs-lookup"><span data-stu-id="3a948-154">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3a948-155">**id**</span><span class="sxs-lookup"><span data-stu-id="3a948-155">**id**</span></span>                   | <span data-ttu-id="3a948-156">string</span><span class="sxs-lookup"><span data-stu-id="3a948-156">string</span></span>                              | <span data-ttu-id="3a948-p101">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="3a948-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="3a948-159">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="3a948-159">**createdDateTime**</span></span>      | <span data-ttu-id="3a948-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a948-160">DateTimeOffset</span></span>                      | <span data-ttu-id="3a948-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="3a948-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="3a948-163">**说明**</span><span class="sxs-lookup"><span data-stu-id="3a948-163">**description**</span></span>          | <span data-ttu-id="3a948-164">string</span><span class="sxs-lookup"><span data-stu-id="3a948-164">string</span></span>                              | <span data-ttu-id="3a948-165">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="3a948-165">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="3a948-166">**displayName**</span><span class="sxs-lookup"><span data-stu-id="3a948-166">**displayName**</span></span>          | <span data-ttu-id="3a948-167">string</span><span class="sxs-lookup"><span data-stu-id="3a948-167">string</span></span>                              | <span data-ttu-id="3a948-p103">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="3a948-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="3a948-170">**eTag**</span><span class="sxs-lookup"><span data-stu-id="3a948-170">**eTag**</span></span>                 | <span data-ttu-id="3a948-171">string</span><span class="sxs-lookup"><span data-stu-id="3a948-171">string</span></span>                              | <span data-ttu-id="3a948-p104">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="3a948-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="3a948-174">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="3a948-174">**lastModifiedDateTime**</span></span> | <span data-ttu-id="3a948-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a948-175">DateTimeOffset</span></span>                      | <span data-ttu-id="3a948-p105">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="3a948-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="3a948-178">**name**</span><span class="sxs-lookup"><span data-stu-id="3a948-178">**name**</span></span>                 | <span data-ttu-id="3a948-179">string</span><span class="sxs-lookup"><span data-stu-id="3a948-179">string</span></span>                              | <span data-ttu-id="3a948-180">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="3a948-180">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="3a948-181">**根**</span><span class="sxs-lookup"><span data-stu-id="3a948-181">**root**</span></span>                 | [<span data-ttu-id="3a948-182">根</span><span class="sxs-lookup"><span data-stu-id="3a948-182">root</span></span>](root.md)                     | <span data-ttu-id="3a948-p106">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="3a948-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="3a948-185">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="3a948-185">**sharepointIds**</span></span>        | [<span data-ttu-id="3a948-186">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="3a948-186">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="3a948-p107">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="3a948-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="3a948-189">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="3a948-189">**siteCollection**</span></span>       | [<span data-ttu-id="3a948-190">siteCollection</span><span class="sxs-lookup"><span data-stu-id="3a948-190">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="3a948-p108">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="3a948-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="3a948-194">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="3a948-194">**webUrl**</span></span>               | <span data-ttu-id="3a948-195">string (url)</span><span class="sxs-lookup"><span data-stu-id="3a948-195">string (url)</span></span>                        | <span data-ttu-id="3a948-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="3a948-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

### <a name="id-property"></a><span data-ttu-id="3a948-198">id 属性</span><span class="sxs-lookup"><span data-stu-id="3a948-198">id property</span></span>
<span data-ttu-id="3a948-199">**site** 由一个唯一 ID 标识，此唯一 ID 由以下值组成：</span><span class="sxs-lookup"><span data-stu-id="3a948-199">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="3a948-200">网站集主机名称 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="3a948-200">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="3a948-201">网站集的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="3a948-201">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="3a948-202">网站的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="3a948-202">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="3a948-203">`root` 标识符经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="3a948-203">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="3a948-204">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="3a948-204">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="3a948-205">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="3a948-205">`/groups/{group-id}/sites/root`: The group's team site.</span></span>
  
## <a name="relationships"></a><span data-ttu-id="3a948-206">关系</span><span class="sxs-lookup"><span data-stu-id="3a948-206">Relationships</span></span>

| <span data-ttu-id="3a948-207">关系</span><span class="sxs-lookup"><span data-stu-id="3a948-207">Relationship</span></span>      | <span data-ttu-id="3a948-208">类型</span><span class="sxs-lookup"><span data-stu-id="3a948-208">Type</span></span>                             | <span data-ttu-id="3a948-209">说明</span><span class="sxs-lookup"><span data-stu-id="3a948-209">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="3a948-210">**analytics**</span><span class="sxs-lookup"><span data-stu-id="3a948-210">**analytics**</span></span>     | <span data-ttu-id="3a948-211">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="3a948-211">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="3a948-212">此网站上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="3a948-212">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="3a948-213">**columns**</span><span class="sxs-lookup"><span data-stu-id="3a948-213">**columns**</span></span>       | <span data-ttu-id="3a948-214">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="3a948-214">Collection([columnDefinition][])</span></span> | <span data-ttu-id="3a948-215">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="3a948-215">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="3a948-216">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="3a948-216">**contentTypes**</span></span>  | <span data-ttu-id="3a948-217">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="3a948-217">Collection([contentType][])</span></span>      | <span data-ttu-id="3a948-218">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="3a948-218">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="3a948-219">**drive**</span><span class="sxs-lookup"><span data-stu-id="3a948-219">**drive**</span></span>         | <span data-ttu-id="3a948-220">[drive][]</span><span class="sxs-lookup"><span data-stu-id="3a948-220">[drive][]</span></span>                        | <span data-ttu-id="3a948-221">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="3a948-221">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="3a948-222">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="3a948-222">**drives**</span></span>        | <span data-ttu-id="3a948-223">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="3a948-223">Collection([drive][])</span></span>            | <span data-ttu-id="3a948-224">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="3a948-224">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="3a948-225">**项目**</span><span class="sxs-lookup"><span data-stu-id="3a948-225">**items**</span></span>         | <span data-ttu-id="3a948-226">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="3a948-226">Collection([baseItem][])</span></span>         | <span data-ttu-id="3a948-p110">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="3a948-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="3a948-229">**lists**</span><span class="sxs-lookup"><span data-stu-id="3a948-229">**lists**</span></span>         | <span data-ttu-id="3a948-230">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="3a948-230">Collection([list][])</span></span>             | <span data-ttu-id="3a948-231">此网站下方的列表集合。</span><span class="sxs-lookup"><span data-stu-id="3a948-231">The collection of lists under this site.</span></span>
| <span data-ttu-id="3a948-232">**sites**</span><span class="sxs-lookup"><span data-stu-id="3a948-232">**sites**</span></span>         | <span data-ttu-id="3a948-233">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="3a948-233">Collection([site][])</span></span>             | <span data-ttu-id="3a948-234">网站下方的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="3a948-234">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="3a948-235">**onenote**</span><span class="sxs-lookup"><span data-stu-id="3a948-235">**onenote**</span></span>       | <span data-ttu-id="3a948-236">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="3a948-236">[onenote][]</span></span>                      | <span data-ttu-id="3a948-237">调用 OneNote 服务执行笔记本相关操作。</span><span class="sxs-lookup"><span data-stu-id="3a948-237">Calls the OneNote service for notebook related operations.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="3a948-246">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a948-246">JSON representation</span></span>

<span data-ttu-id="3a948-247">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a948-247">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="3a948-248">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="3a948-248">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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

