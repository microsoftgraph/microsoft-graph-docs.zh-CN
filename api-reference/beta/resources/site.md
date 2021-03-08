---
author: JeremyKelley
description: 网站资源提供 SharePoint 网站的元数据和关系。
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 587014aa0c9dbe4c05c0e3b946c3f6e44b7cb821
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442787"
---
# <a name="site-resource-type"></a><span data-ttu-id="246b7-103">site 资源类型</span><span class="sxs-lookup"><span data-stu-id="246b7-103">site resource type</span></span>

<span data-ttu-id="246b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="246b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="246b7-105">**site** 资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="246b7-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="246b7-106">方法</span><span class="sxs-lookup"><span data-stu-id="246b7-106">Methods</span></span>

| <span data-ttu-id="246b7-107">方法</span><span class="sxs-lookup"><span data-stu-id="246b7-107">Method</span></span>                         | <span data-ttu-id="246b7-108">REST 路径</span><span class="sxs-lookup"><span data-stu-id="246b7-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="246b7-109">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="246b7-109">[Get root site][]</span></span>              | <span data-ttu-id="246b7-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="246b7-110">GET /sites/root</span></span>
| <span data-ttu-id="246b7-111">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="246b7-111">[Get site][]</span></span>                   | <span data-ttu-id="246b7-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="246b7-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="246b7-113">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="246b7-113">[Get site by path][]</span></span>           | <span data-ttu-id="246b7-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="246b7-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="246b7-115">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="246b7-115">[Get site for a group][]</span></span>       | <span data-ttu-id="246b7-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="246b7-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="246b7-117">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="246b7-117">[Get analytics][]</span></span>              | <span data-ttu-id="246b7-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="246b7-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="246b7-119">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="246b7-119">[Get activities by interval][]</span></span> | <span data-ttu-id="246b7-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="246b7-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="246b7-121">[列出页面][]</span><span class="sxs-lookup"><span data-stu-id="246b7-121">[List pages][]</span></span>                 | <span data-ttu-id="246b7-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="246b7-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="246b7-123">[列出根网站][]</span><span class="sxs-lookup"><span data-stu-id="246b7-123">[List root sites][]</span></span>            | <span data-ttu-id="246b7-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="246b7-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="246b7-125">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="246b7-125">[Search for sites][]</span></span>           | <span data-ttu-id="246b7-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="246b7-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="246b7-127">[关注网站][]</span><span class="sxs-lookup"><span data-stu-id="246b7-127">[Follow site][]</span></span>                | <span data-ttu-id="246b7-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="246b7-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="246b7-129">[取消关注网站][]</span><span class="sxs-lookup"><span data-stu-id="246b7-129">[Unfollow site][]</span></span>              | <span data-ttu-id="246b7-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="246b7-130">POST /users/{user-id}/followedSites/remove</span></span>
| <span data-ttu-id="246b7-131">[关注网站列表][]</span><span class="sxs-lookup"><span data-stu-id="246b7-131">[List followed sites][]</span></span>        | <span data-ttu-id="246b7-132">GET /me/followedSites</span><span class="sxs-lookup"><span data-stu-id="246b7-132">GET /me/followedSites</span></span>
| <span data-ttu-id="246b7-133">[获取权限][]</span><span class="sxs-lookup"><span data-stu-id="246b7-133">[Get permission][]</span></span>             | <span data-ttu-id="246b7-134">GET /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="246b7-134">GET /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="246b7-135">[列出权限][]</span><span class="sxs-lookup"><span data-stu-id="246b7-135">[List permissions][]</span></span>           | <span data-ttu-id="246b7-136">GET /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="246b7-136">GET /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="246b7-137">[创建权限][]</span><span class="sxs-lookup"><span data-stu-id="246b7-137">[Create permissions][]</span></span>         | <span data-ttu-id="246b7-138">POST /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="246b7-138">POST /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="246b7-139">[删除权限][]</span><span class="sxs-lookup"><span data-stu-id="246b7-139">[Delete permission][]</span></span>         | <span data-ttu-id="246b7-140">DELETE /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="246b7-140">DELETE /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="246b7-141">[更新权限][]</span><span class="sxs-lookup"><span data-stu-id="246b7-141">[Update permission][]</span></span>         | <span data-ttu-id="246b7-142">PATCH /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="246b7-142">PATCH /sites/{site-id}/permissions/{permission-id}</span></span>

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
[获取权限]: ../api/site-get-permission.md
[Get permission]: ../api/site-get-permission.md
[列出权限]: ../api/site-list-permissions.md
[List permissions]: ../api/site-list-permissions.md
[创建权限]: ../api/site-post-permissions.md
[Create permissions]: ../api/site-post-permissions.md
[删除权限]: ../api/site-delete-permission.md
[Delete permission]: ../api/site-delete-permission.md
[更新权限]: ../api/site-update-permission.md
[Update permission]: ../api/site-update-permission.md


## <a name="properties"></a><span data-ttu-id="246b7-160">属性</span><span class="sxs-lookup"><span data-stu-id="246b7-160">Properties</span></span>

| <span data-ttu-id="246b7-161">属性名称</span><span class="sxs-lookup"><span data-stu-id="246b7-161">Property name</span></span>            | <span data-ttu-id="246b7-162">类型</span><span class="sxs-lookup"><span data-stu-id="246b7-162">Type</span></span>               | <span data-ttu-id="246b7-163">说明</span><span class="sxs-lookup"><span data-stu-id="246b7-163">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="246b7-164">**id**</span><span class="sxs-lookup"><span data-stu-id="246b7-164">**id**</span></span>                   | <span data-ttu-id="246b7-165">string</span><span class="sxs-lookup"><span data-stu-id="246b7-165">string</span></span>             | <span data-ttu-id="246b7-166">项的[唯一标识符](#id-property)。</span><span class="sxs-lookup"><span data-stu-id="246b7-166">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="246b7-167">只读。</span><span class="sxs-lookup"><span data-stu-id="246b7-167">Read-only.</span></span>
| <span data-ttu-id="246b7-168">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="246b7-168">**createdDateTime**</span></span>      | <span data-ttu-id="246b7-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="246b7-169">DateTimeOffset</span></span>     | <span data-ttu-id="246b7-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="246b7-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="246b7-172">**说明**</span><span class="sxs-lookup"><span data-stu-id="246b7-172">**description**</span></span>          | <span data-ttu-id="246b7-173">string</span><span class="sxs-lookup"><span data-stu-id="246b7-173">string</span></span>             | <span data-ttu-id="246b7-174">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="246b7-174">The descriptive text for the site.</span></span>
| <span data-ttu-id="246b7-175">**eTag**</span><span class="sxs-lookup"><span data-stu-id="246b7-175">**eTag**</span></span>                 | <span data-ttu-id="246b7-176">string</span><span class="sxs-lookup"><span data-stu-id="246b7-176">string</span></span>             | <span data-ttu-id="246b7-p103">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="246b7-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="246b7-179">**displayName**</span><span class="sxs-lookup"><span data-stu-id="246b7-179">**displayName**</span></span>          | <span data-ttu-id="246b7-180">string</span><span class="sxs-lookup"><span data-stu-id="246b7-180">string</span></span>             | <span data-ttu-id="246b7-p104">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="246b7-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="246b7-183">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="246b7-183">**lastModifiedDateTime**</span></span> | <span data-ttu-id="246b7-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="246b7-184">DateTimeOffset</span></span>     | <span data-ttu-id="246b7-p105">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="246b7-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="246b7-187">**name**</span><span class="sxs-lookup"><span data-stu-id="246b7-187">**name**</span></span>                 | <span data-ttu-id="246b7-188">string</span><span class="sxs-lookup"><span data-stu-id="246b7-188">string</span></span>             | <span data-ttu-id="246b7-189">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="246b7-189">The name / title of the item.</span></span>
| <span data-ttu-id="246b7-190">**根**</span><span class="sxs-lookup"><span data-stu-id="246b7-190">**root**</span></span>                 | <span data-ttu-id="246b7-191">[根][]</span><span class="sxs-lookup"><span data-stu-id="246b7-191">[root][]</span></span>           | <span data-ttu-id="246b7-p106">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="246b7-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="246b7-194">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="246b7-194">**sharepointIds**</span></span>        | <span data-ttu-id="246b7-195">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="246b7-195">[sharepointIds][]</span></span>  | <span data-ttu-id="246b7-p107">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="246b7-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="246b7-198">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="246b7-198">**siteCollection**</span></span>       | <span data-ttu-id="246b7-199">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="246b7-199">[siteCollection][]</span></span> | <span data-ttu-id="246b7-p108">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="246b7-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="246b7-203">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="246b7-203">**webUrl**</span></span>               | <span data-ttu-id="246b7-204">string (url)</span><span class="sxs-lookup"><span data-stu-id="246b7-204">string (url)</span></span>       | <span data-ttu-id="246b7-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="246b7-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="246b7-207">id 属性</span><span class="sxs-lookup"><span data-stu-id="246b7-207">id property</span></span>
<span data-ttu-id="246b7-208">**site** 由一个唯一 ID 标识，此唯一 ID 由以下值组成：</span><span class="sxs-lookup"><span data-stu-id="246b7-208">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="246b7-209">网站集主机名称 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="246b7-209">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="246b7-210">网站集的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="246b7-210">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="246b7-211">网站的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="246b7-211">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="246b7-212">`root` 标识符经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="246b7-212">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="246b7-213">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="246b7-213">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="246b7-214">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="246b7-214">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="246b7-215">关系</span><span class="sxs-lookup"><span data-stu-id="246b7-215">Relationships</span></span>

| <span data-ttu-id="246b7-216">关系名称</span><span class="sxs-lookup"><span data-stu-id="246b7-216">Relationship name</span></span> | <span data-ttu-id="246b7-217">类型</span><span class="sxs-lookup"><span data-stu-id="246b7-217">Type</span></span>                             | <span data-ttu-id="246b7-218">说明</span><span class="sxs-lookup"><span data-stu-id="246b7-218">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="246b7-219">**analytics**</span><span class="sxs-lookup"><span data-stu-id="246b7-219">**analytics**</span></span>     | <span data-ttu-id="246b7-220">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="246b7-220">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="246b7-221">此网站上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="246b7-221">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="246b7-222">**columns**</span><span class="sxs-lookup"><span data-stu-id="246b7-222">**columns**</span></span>       | <span data-ttu-id="246b7-223">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="246b7-223">Collection([columnDefinition][])</span></span> | <span data-ttu-id="246b7-224">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="246b7-224">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="246b7-225">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="246b7-225">**contentTypes**</span></span>  | <span data-ttu-id="246b7-226">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="246b7-226">Collection([contentType][])</span></span>      | <span data-ttu-id="246b7-227">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="246b7-227">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="246b7-228">**drive**</span><span class="sxs-lookup"><span data-stu-id="246b7-228">**drive**</span></span>         | <span data-ttu-id="246b7-229">[drive][]</span><span class="sxs-lookup"><span data-stu-id="246b7-229">[drive][]</span></span>                        | <span data-ttu-id="246b7-230">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="246b7-230">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="246b7-231">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="246b7-231">**drives**</span></span>        | <span data-ttu-id="246b7-232">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="246b7-232">Collection([drive][])</span></span>            | <span data-ttu-id="246b7-233">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="246b7-233">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="246b7-234">**项目**</span><span class="sxs-lookup"><span data-stu-id="246b7-234">**items**</span></span>         | <span data-ttu-id="246b7-235">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="246b7-235">Collection([baseItem][])</span></span>         | <span data-ttu-id="246b7-p110">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="246b7-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="246b7-238">**lists**</span><span class="sxs-lookup"><span data-stu-id="246b7-238">**lists**</span></span>         | <span data-ttu-id="246b7-239">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="246b7-239">Collection([list][])</span></span>             | <span data-ttu-id="246b7-240">此网站下的列表集合。</span><span class="sxs-lookup"><span data-stu-id="246b7-240">The collection of lists under this site.</span></span>
| <span data-ttu-id="246b7-241">**pages**</span><span class="sxs-lookup"><span data-stu-id="246b7-241">**pages**</span></span>         | <span data-ttu-id="246b7-242">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="246b7-242">Collection([sitePage][])</span></span>         | <span data-ttu-id="246b7-243">此网站的 SitePages 列表中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="246b7-243">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="246b7-244">**权限**</span><span class="sxs-lookup"><span data-stu-id="246b7-244">**permissions**</span></span>   | <span data-ttu-id="246b7-245">集合([权限][])</span><span class="sxs-lookup"><span data-stu-id="246b7-245">Collection([permission][])</span></span>         | <span data-ttu-id="246b7-246">与网站关联的权限。</span><span class="sxs-lookup"><span data-stu-id="246b7-246">The permissions associated with the site.</span></span> <span data-ttu-id="246b7-247">可为空。</span><span class="sxs-lookup"><span data-stu-id="246b7-247">Nullable.</span></span>
| <span data-ttu-id="246b7-248">**sites**</span><span class="sxs-lookup"><span data-stu-id="246b7-248">**sites**</span></span>         | <span data-ttu-id="246b7-249">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="246b7-249">Collection([site][])</span></span>             | <span data-ttu-id="246b7-250">网站下方的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="246b7-250">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="246b7-251">**externalColumns**</span><span class="sxs-lookup"><span data-stu-id="246b7-251">**externalColumns**</span></span>     | <span data-ttu-id="246b7-252">集合（[columnDefinition][]）</span><span class="sxs-lookup"><span data-stu-id="246b7-252">Collection([columnDefinition][])</span></span>  | <span data-ttu-id="246b7-253">网站中可用列定义的集合，从当前网站的父层次结构中的网站引用。</span><span class="sxs-lookup"><span data-stu-id="246b7-253">The collection of column definitions available in the site that are referenced from the sites in the parent hierarchy of the current site.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[permission]: permission.md
[sitePage]: sitepage.md
[root]: root.md
[site]: site.md
[sharepointIds]: sharepointids.md
[siteCollection]: sitecollection.md

## <a name="json-representation"></a><span data-ttu-id="246b7-266">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="246b7-266">JSON representation</span></span>

<span data-ttu-id="246b7-267">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="246b7-267">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="246b7-268">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="246b7-268">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "root",
    "sharepointIds",
    "siteCollection",
    "drive",
    "drives",
    "permissions",
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
  "permissions": [ { "@odata.type": "microsoft.graph.permission" }],
  "sites": [ { "@odata.type": "microsoft.graph.site"} ],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "externalColumns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
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
