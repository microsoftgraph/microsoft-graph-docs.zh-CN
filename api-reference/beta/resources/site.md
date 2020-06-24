---
author: JeremyKelley
description: 网站资源提供 SharePoint 网站的元数据和关系。
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: fc6a7472da2676d0266d964b7bdddee976d5ac8c
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864222"
---
# <a name="site-resource-type"></a><span data-ttu-id="5ca7c-103">site 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ca7c-103">site resource type</span></span>

<span data-ttu-id="5ca7c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ca7c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ca7c-105">**site** 资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="5ca7c-106">方法</span><span class="sxs-lookup"><span data-stu-id="5ca7c-106">Methods</span></span>

| <span data-ttu-id="5ca7c-107">方法</span><span class="sxs-lookup"><span data-stu-id="5ca7c-107">Method</span></span>                         | <span data-ttu-id="5ca7c-108">REST 路径</span><span class="sxs-lookup"><span data-stu-id="5ca7c-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="5ca7c-109">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-109">[Get root site][]</span></span>              | <span data-ttu-id="5ca7c-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="5ca7c-110">GET /sites/root</span></span>
| <span data-ttu-id="5ca7c-111">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-111">[Get site][]</span></span>                   | <span data-ttu-id="5ca7c-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="5ca7c-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="5ca7c-113">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-113">[Get site by path][]</span></span>           | <span data-ttu-id="5ca7c-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="5ca7c-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="5ca7c-115">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-115">[Get site for a group][]</span></span>       | <span data-ttu-id="5ca7c-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="5ca7c-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="5ca7c-117">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-117">[Get analytics][]</span></span>              | <span data-ttu-id="5ca7c-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="5ca7c-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="5ca7c-119">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-119">[Get activities by interval][]</span></span> | <span data-ttu-id="5ca7c-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="5ca7c-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="5ca7c-121">[列出页面][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-121">[List pages][]</span></span>                 | <span data-ttu-id="5ca7c-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="5ca7c-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="5ca7c-123">[列出根网站][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-123">[List root sites][]</span></span>            | <span data-ttu-id="5ca7c-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="5ca7c-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="5ca7c-125">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-125">[Search for sites][]</span></span>           | <span data-ttu-id="5ca7c-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="5ca7c-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="5ca7c-127">[关注网站][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-127">[Follow site][]</span></span>                | <span data-ttu-id="5ca7c-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="5ca7c-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="5ca7c-129">[取消关注网站][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-129">[Unfollow site][]</span></span>              | <span data-ttu-id="5ca7c-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="5ca7c-130">POST /users/{user-id}/followedSites/remove</span></span>
| <span data-ttu-id="5ca7c-131">[关注网站列表][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-131">[List followed sites][]</span></span>        | <span data-ttu-id="5ca7c-132">GET /me/followedSites</span><span class="sxs-lookup"><span data-stu-id="5ca7c-132">GET /me/followedSites</span></span>

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
[关注网站列表]: ../api/sites-list-followed.md
[List followed sites]: ../api/sites-list-followed.md


## <a name="properties"></a><span data-ttu-id="5ca7c-145">属性</span><span class="sxs-lookup"><span data-stu-id="5ca7c-145">Properties</span></span>

| <span data-ttu-id="5ca7c-146">属性名称</span><span class="sxs-lookup"><span data-stu-id="5ca7c-146">Property name</span></span>            | <span data-ttu-id="5ca7c-147">类型</span><span class="sxs-lookup"><span data-stu-id="5ca7c-147">Type</span></span>               | <span data-ttu-id="5ca7c-148">说明</span><span class="sxs-lookup"><span data-stu-id="5ca7c-148">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="5ca7c-149">**id**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-149">**id**</span></span>                   | <span data-ttu-id="5ca7c-150">string</span><span class="sxs-lookup"><span data-stu-id="5ca7c-150">string</span></span>             | <span data-ttu-id="5ca7c-151">项的[唯一标识符](#id-property)。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-151">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="5ca7c-152">只读。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-152">Read-only.</span></span>
| <span data-ttu-id="5ca7c-153">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-153">**createdDateTime**</span></span>      | <span data-ttu-id="5ca7c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ca7c-154">DateTimeOffset</span></span>     | <span data-ttu-id="5ca7c-155">The date and time the item was created.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-155">The date and time the item was created.</span></span> <span data-ttu-id="5ca7c-156">Read-only.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-156">Read-only.</span></span>
| <span data-ttu-id="5ca7c-157">**说明**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-157">**description**</span></span>          | <span data-ttu-id="5ca7c-158">string</span><span class="sxs-lookup"><span data-stu-id="5ca7c-158">string</span></span>             | <span data-ttu-id="5ca7c-159">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-159">The descriptive text for the site.</span></span>
| <span data-ttu-id="5ca7c-160">**eTag**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-160">**eTag**</span></span>                 | <span data-ttu-id="5ca7c-161">string</span><span class="sxs-lookup"><span data-stu-id="5ca7c-161">string</span></span>             | <span data-ttu-id="5ca7c-162">ETag for the item.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-162">ETag for the item.</span></span> <span data-ttu-id="5ca7c-163">Read-only.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-163">Read-only.</span></span>                                                                  |
| <span data-ttu-id="5ca7c-164">**displayName**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-164">**displayName**</span></span>          | <span data-ttu-id="5ca7c-165">string</span><span class="sxs-lookup"><span data-stu-id="5ca7c-165">string</span></span>             | <span data-ttu-id="5ca7c-166">The full title for the site.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-166">The full title for the site.</span></span> <span data-ttu-id="5ca7c-167">Read-only.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-167">Read-only.</span></span>
| <span data-ttu-id="5ca7c-168">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-168">**lastModifiedDateTime**</span></span> | <span data-ttu-id="5ca7c-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ca7c-169">DateTimeOffset</span></span>     | <span data-ttu-id="5ca7c-170">The date and time the item was last modified.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-170">The date and time the item was last modified.</span></span> <span data-ttu-id="5ca7c-171">Read-only.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-171">Read-only.</span></span>
| <span data-ttu-id="5ca7c-172">**name**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-172">**name**</span></span>                 | <span data-ttu-id="5ca7c-173">string</span><span class="sxs-lookup"><span data-stu-id="5ca7c-173">string</span></span>             | <span data-ttu-id="5ca7c-174">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-174">The name / title of the item.</span></span>
| <span data-ttu-id="5ca7c-175">**根**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-175">**root**</span></span>                 | <span data-ttu-id="5ca7c-176">[根][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-176">[root][]</span></span>           | <span data-ttu-id="5ca7c-177">If present, indicates that this is the root site in the site collection.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-177">If present, indicates that this is the root site in the site collection.</span></span> <span data-ttu-id="5ca7c-178">Read-only.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-178">Read-only.</span></span>
| <span data-ttu-id="5ca7c-179">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-179">**sharepointIds**</span></span>        | <span data-ttu-id="5ca7c-180">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-180">[sharepointIds][]</span></span>  | <span data-ttu-id="5ca7c-181">Returns identifiers useful for SharePoint REST compatibility.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-181">Returns identifiers useful for SharePoint REST compatibility.</span></span> <span data-ttu-id="5ca7c-182">Read-only.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-182">Read-only.</span></span>
| <span data-ttu-id="5ca7c-183">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-183">**siteCollection**</span></span>       | <span data-ttu-id="5ca7c-184">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-184">[siteCollection][]</span></span> | <span data-ttu-id="5ca7c-185">Provides details about the site's site collection.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-185">Provides details about the site's site collection.</span></span> <span data-ttu-id="5ca7c-186">Available only on the root site.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-186">Available only on the root site.</span></span> <span data-ttu-id="5ca7c-187">Read-only.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-187">Read-only.</span></span>
| <span data-ttu-id="5ca7c-188">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-188">**webUrl**</span></span>               | <span data-ttu-id="5ca7c-189">string (url)</span><span class="sxs-lookup"><span data-stu-id="5ca7c-189">string (url)</span></span>       | <span data-ttu-id="5ca7c-190">URL that displays the item in the browser.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-190">URL that displays the item in the browser.</span></span> <span data-ttu-id="5ca7c-191">Read-only.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-191">Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="5ca7c-192">id 属性</span><span class="sxs-lookup"><span data-stu-id="5ca7c-192">id property</span></span>
<span data-ttu-id="5ca7c-193">**site** 由一个唯一 ID 标识，此唯一 ID 由以下值组成：</span><span class="sxs-lookup"><span data-stu-id="5ca7c-193">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="5ca7c-194">网站集主机名称 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="5ca7c-194">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="5ca7c-195">网站集的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="5ca7c-195">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="5ca7c-196">网站的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="5ca7c-196">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="5ca7c-197">`root` 标识符经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="5ca7c-197">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="5ca7c-198">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-198">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="5ca7c-199">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-199">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="5ca7c-200">关系</span><span class="sxs-lookup"><span data-stu-id="5ca7c-200">Relationships</span></span>

| <span data-ttu-id="5ca7c-201">关系名称</span><span class="sxs-lookup"><span data-stu-id="5ca7c-201">Relationship name</span></span> | <span data-ttu-id="5ca7c-202">类型</span><span class="sxs-lookup"><span data-stu-id="5ca7c-202">Type</span></span>                             | <span data-ttu-id="5ca7c-203">说明</span><span class="sxs-lookup"><span data-stu-id="5ca7c-203">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="5ca7c-204">**analytics**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-204">**analytics**</span></span>     | <span data-ttu-id="5ca7c-205">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="5ca7c-205">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="5ca7c-206">此网站上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-206">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="5ca7c-207">**columns**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-207">**columns**</span></span>       | <span data-ttu-id="5ca7c-208">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="5ca7c-208">Collection([columnDefinition][])</span></span> | <span data-ttu-id="5ca7c-209">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-209">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="5ca7c-210">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-210">**contentTypes**</span></span>  | <span data-ttu-id="5ca7c-211">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="5ca7c-211">Collection([contentType][])</span></span>      | <span data-ttu-id="5ca7c-212">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-212">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="5ca7c-213">**drive**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-213">**drive**</span></span>         | <span data-ttu-id="5ca7c-214">[drive][]</span><span class="sxs-lookup"><span data-stu-id="5ca7c-214">[drive][]</span></span>                        | <span data-ttu-id="5ca7c-215">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-215">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="5ca7c-216">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-216">**drives**</span></span>        | <span data-ttu-id="5ca7c-217">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="5ca7c-217">Collection([drive][])</span></span>            | <span data-ttu-id="5ca7c-218">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-218">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="5ca7c-219">**项目**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-219">**items**</span></span>         | <span data-ttu-id="5ca7c-220">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="5ca7c-220">Collection([baseItem][])</span></span>         | <span data-ttu-id="5ca7c-221">Used to address any item contained in this site.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-221">Used to address any item contained in this site.</span></span> <span data-ttu-id="5ca7c-222">This collection cannot be enumerated.</span><span class="sxs-lookup"><span data-stu-id="5ca7c-222">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="5ca7c-223">**lists**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-223">**lists**</span></span>         | <span data-ttu-id="5ca7c-224">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="5ca7c-224">Collection([list][])</span></span>             | <span data-ttu-id="5ca7c-225">此网站下的列表集合。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-225">The collection of lists under this site.</span></span>
| <span data-ttu-id="5ca7c-226">**pages**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-226">**pages**</span></span>         | <span data-ttu-id="5ca7c-227">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="5ca7c-227">Collection([sitePage][])</span></span>         | <span data-ttu-id="5ca7c-228">此网站的 SitePages 列表中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-228">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="5ca7c-229">**sites**</span><span class="sxs-lookup"><span data-stu-id="5ca7c-229">**sites**</span></span>         | <span data-ttu-id="5ca7c-230">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="5ca7c-230">Collection([site][])</span></span>             | <span data-ttu-id="5ca7c-231">网站下的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-231">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="5ca7c-243">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ca7c-243">JSON representation</span></span>

<span data-ttu-id="5ca7c-244">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-244">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="5ca7c-245">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="5ca7c-245">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
