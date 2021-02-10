---
author: JeremyKelley
description: 网站资源提供 SharePoint 网站的元数据和关系。
ms.date: 09/10/2017
title: Site
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 152100311e85dc905e14ca6f434a9a9fbe1d87fe
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155837"
---
# <a name="site-resource-type"></a><span data-ttu-id="623df-103">site 资源类型</span><span class="sxs-lookup"><span data-stu-id="623df-103">site resource type</span></span>

<span data-ttu-id="623df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="623df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="623df-105">**site** 资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="623df-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="623df-106">方法</span><span class="sxs-lookup"><span data-stu-id="623df-106">Methods</span></span>

| <span data-ttu-id="623df-107">方法</span><span class="sxs-lookup"><span data-stu-id="623df-107">Method</span></span>                         | <span data-ttu-id="623df-108">REST 路径</span><span class="sxs-lookup"><span data-stu-id="623df-108">REST Path</span></span>
|:-------------------------------|:--------------------------------------------
| <span data-ttu-id="623df-109">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="623df-109">[Get root site][]</span></span>              | <span data-ttu-id="623df-110">GET /sites/root</span><span class="sxs-lookup"><span data-stu-id="623df-110">GET /sites/root</span></span>
| <span data-ttu-id="623df-111">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="623df-111">[Get site][]</span></span>                   | <span data-ttu-id="623df-112">GET /sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="623df-112">GET /sites/{site-id}</span></span>
| <span data-ttu-id="623df-113">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="623df-113">[Get site by path][]</span></span>           | <span data-ttu-id="623df-114">GET /sites/{hostname}:/{site-path}</span><span class="sxs-lookup"><span data-stu-id="623df-114">GET /sites/{hostname}:/{site-path}</span></span>
| <span data-ttu-id="623df-115">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="623df-115">[Get site for a group][]</span></span>       | <span data-ttu-id="623df-116">GET /groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="623df-116">GET /groups/{group-id}/sites/root</span></span>
| <span data-ttu-id="623df-117">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="623df-117">[Get analytics][]</span></span>              | <span data-ttu-id="623df-118">GET /sites/{site-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="623df-118">GET /sites/{site-id}/analytics</span></span>
| <span data-ttu-id="623df-119">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="623df-119">[Get activities by interval][]</span></span> | <span data-ttu-id="623df-120">GET /sites/{site-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="623df-120">GET /sites/{site-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="623df-121">[列出页面][]</span><span class="sxs-lookup"><span data-stu-id="623df-121">[List pages][]</span></span>                 | <span data-ttu-id="623df-122">GET /sites/{site-id}/pages</span><span class="sxs-lookup"><span data-stu-id="623df-122">GET /sites/{site-id}/pages</span></span>
| <span data-ttu-id="623df-123">[列出根网站][]</span><span class="sxs-lookup"><span data-stu-id="623df-123">[List root sites][]</span></span>            | <span data-ttu-id="623df-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span><span class="sxs-lookup"><span data-stu-id="623df-124">GET /sites?filter=root ne null&select=siteCollection,webUrl</span></span>
| <span data-ttu-id="623df-125">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="623df-125">[Search for sites][]</span></span>           | <span data-ttu-id="623df-126">GET /sites?search={query}</span><span class="sxs-lookup"><span data-stu-id="623df-126">GET /sites?search={query}</span></span>
| <span data-ttu-id="623df-127">[关注网站][]</span><span class="sxs-lookup"><span data-stu-id="623df-127">[Follow site][]</span></span>                | <span data-ttu-id="623df-128">POST /users/{user-id}/followedSites/add</span><span class="sxs-lookup"><span data-stu-id="623df-128">POST /users/{user-id}/followedSites/add</span></span>
| <span data-ttu-id="623df-129">[取消关注网站][]</span><span class="sxs-lookup"><span data-stu-id="623df-129">[Unfollow site][]</span></span>              | <span data-ttu-id="623df-130">POST /users/{user-id}/followedSites/remove</span><span class="sxs-lookup"><span data-stu-id="623df-130">POST /users/{user-id}/followedSites/remove</span></span>
| <span data-ttu-id="623df-131">[关注网站列表][]</span><span class="sxs-lookup"><span data-stu-id="623df-131">[List followed sites][]</span></span>        | <span data-ttu-id="623df-132">GET /me/followedSites</span><span class="sxs-lookup"><span data-stu-id="623df-132">GET /me/followedSites</span></span>
| <span data-ttu-id="623df-133">[获取权限][]</span><span class="sxs-lookup"><span data-stu-id="623df-133">[Get permission][]</span></span>             | <span data-ttu-id="623df-134">GET /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="623df-134">GET /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="623df-135">[列出权限][]</span><span class="sxs-lookup"><span data-stu-id="623df-135">[List permissions][]</span></span>           | <span data-ttu-id="623df-136">GET /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="623df-136">GET /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="623df-137">[创建权限][]</span><span class="sxs-lookup"><span data-stu-id="623df-137">[Create permissions][]</span></span>         | <span data-ttu-id="623df-138">POST /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="623df-138">POST /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="623df-139">[删除权限][]</span><span class="sxs-lookup"><span data-stu-id="623df-139">[Delete permission][]</span></span>         | <span data-ttu-id="623df-140">DELETE /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="623df-140">DELETE /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="623df-141">[更新权限][]</span><span class="sxs-lookup"><span data-stu-id="623df-141">[Update permission][]</span></span>         | <span data-ttu-id="623df-142">PATCH /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="623df-142">PATCH /sites/{site-id}/permissions/{permission-id}</span></span>

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


## <a name="properties"></a><span data-ttu-id="623df-160">属性</span><span class="sxs-lookup"><span data-stu-id="623df-160">Properties</span></span>

| <span data-ttu-id="623df-161">属性名称</span><span class="sxs-lookup"><span data-stu-id="623df-161">Property name</span></span>            | <span data-ttu-id="623df-162">类型</span><span class="sxs-lookup"><span data-stu-id="623df-162">Type</span></span>               | <span data-ttu-id="623df-163">说明</span><span class="sxs-lookup"><span data-stu-id="623df-163">Description</span></span>
|:-------------------------|:-------------------|:-----------------------------
| <span data-ttu-id="623df-164">**id**</span><span class="sxs-lookup"><span data-stu-id="623df-164">**id**</span></span>                   | <span data-ttu-id="623df-165">string</span><span class="sxs-lookup"><span data-stu-id="623df-165">string</span></span>             | <span data-ttu-id="623df-166">项的[唯一标识符](#id-property)。</span><span class="sxs-lookup"><span data-stu-id="623df-166">The [unique identifier](#id-property) of the item.</span></span> <span data-ttu-id="623df-167">只读。</span><span class="sxs-lookup"><span data-stu-id="623df-167">Read-only.</span></span>
| <span data-ttu-id="623df-168">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="623df-168">**createdDateTime**</span></span>      | <span data-ttu-id="623df-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="623df-169">DateTimeOffset</span></span>     | <span data-ttu-id="623df-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="623df-p102">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="623df-172">**说明**</span><span class="sxs-lookup"><span data-stu-id="623df-172">**description**</span></span>          | <span data-ttu-id="623df-173">string</span><span class="sxs-lookup"><span data-stu-id="623df-173">string</span></span>             | <span data-ttu-id="623df-174">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="623df-174">The descriptive text for the site.</span></span>
| <span data-ttu-id="623df-175">**eTag**</span><span class="sxs-lookup"><span data-stu-id="623df-175">**eTag**</span></span>                 | <span data-ttu-id="623df-176">string</span><span class="sxs-lookup"><span data-stu-id="623df-176">string</span></span>             | <span data-ttu-id="623df-p103">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="623df-p103">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="623df-179">**displayName**</span><span class="sxs-lookup"><span data-stu-id="623df-179">**displayName**</span></span>          | <span data-ttu-id="623df-180">string</span><span class="sxs-lookup"><span data-stu-id="623df-180">string</span></span>             | <span data-ttu-id="623df-p104">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="623df-p104">The full title for the site. Read-only.</span></span>
| <span data-ttu-id="623df-183">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="623df-183">**lastModifiedDateTime**</span></span> | <span data-ttu-id="623df-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="623df-184">DateTimeOffset</span></span>     | <span data-ttu-id="623df-p105">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="623df-p105">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="623df-187">**name**</span><span class="sxs-lookup"><span data-stu-id="623df-187">**name**</span></span>                 | <span data-ttu-id="623df-188">string</span><span class="sxs-lookup"><span data-stu-id="623df-188">string</span></span>             | <span data-ttu-id="623df-189">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="623df-189">The name / title of the item.</span></span>
| <span data-ttu-id="623df-190">**根**</span><span class="sxs-lookup"><span data-stu-id="623df-190">**root**</span></span>                 | <span data-ttu-id="623df-191">[根][]</span><span class="sxs-lookup"><span data-stu-id="623df-191">[root][]</span></span>           | <span data-ttu-id="623df-p106">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="623df-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>
| <span data-ttu-id="623df-194">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="623df-194">**sharepointIds**</span></span>        | <span data-ttu-id="623df-195">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="623df-195">[sharepointIds][]</span></span>  | <span data-ttu-id="623df-p107">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="623df-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="623df-198">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="623df-198">**siteCollection**</span></span>       | <span data-ttu-id="623df-199">[siteCollection][]</span><span class="sxs-lookup"><span data-stu-id="623df-199">[siteCollection][]</span></span> | <span data-ttu-id="623df-p108">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="623df-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span>
| <span data-ttu-id="623df-203">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="623df-203">**webUrl**</span></span>               | <span data-ttu-id="623df-204">string (url)</span><span class="sxs-lookup"><span data-stu-id="623df-204">string (url)</span></span>       | <span data-ttu-id="623df-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="623df-p109">URL that displays the item in the browser. Read-only.</span></span>

### <a name="id-property"></a><span data-ttu-id="623df-207">id 属性</span><span class="sxs-lookup"><span data-stu-id="623df-207">id property</span></span>
<span data-ttu-id="623df-208">**site** 由一个唯一 ID 标识，此唯一 ID 由以下值组成：</span><span class="sxs-lookup"><span data-stu-id="623df-208">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="623df-209">网站集主机名称 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="623df-209">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="623df-210">网站集的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="623df-210">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="623df-211">网站的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="623df-211">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="623df-212">`root` 标识符经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="623df-212">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="623df-213">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="623df-213">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="623df-214">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="623df-214">`/groups/{group-id}/sites/root`: The group's team site.</span></span>

## <a name="relationships"></a><span data-ttu-id="623df-215">关系</span><span class="sxs-lookup"><span data-stu-id="623df-215">Relationships</span></span>

| <span data-ttu-id="623df-216">关系名称</span><span class="sxs-lookup"><span data-stu-id="623df-216">Relationship name</span></span> | <span data-ttu-id="623df-217">类型</span><span class="sxs-lookup"><span data-stu-id="623df-217">Type</span></span>                             | <span data-ttu-id="623df-218">说明</span><span class="sxs-lookup"><span data-stu-id="623df-218">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="623df-219">**analytics**</span><span class="sxs-lookup"><span data-stu-id="623df-219">**analytics**</span></span>     | <span data-ttu-id="623df-220">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="623df-220">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="623df-221">此网站上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="623df-221">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="623df-222">**columns**</span><span class="sxs-lookup"><span data-stu-id="623df-222">**columns**</span></span>       | <span data-ttu-id="623df-223">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="623df-223">Collection([columnDefinition][])</span></span> | <span data-ttu-id="623df-224">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="623df-224">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="623df-225">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="623df-225">**contentTypes**</span></span>  | <span data-ttu-id="623df-226">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="623df-226">Collection([contentType][])</span></span>      | <span data-ttu-id="623df-227">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="623df-227">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="623df-228">**drive**</span><span class="sxs-lookup"><span data-stu-id="623df-228">**drive**</span></span>         | <span data-ttu-id="623df-229">[drive][]</span><span class="sxs-lookup"><span data-stu-id="623df-229">[drive][]</span></span>                        | <span data-ttu-id="623df-230">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="623df-230">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="623df-231">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="623df-231">**drives**</span></span>        | <span data-ttu-id="623df-232">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="623df-232">Collection([drive][])</span></span>            | <span data-ttu-id="623df-233">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="623df-233">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="623df-234">**项目**</span><span class="sxs-lookup"><span data-stu-id="623df-234">**items**</span></span>         | <span data-ttu-id="623df-235">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="623df-235">Collection([baseItem][])</span></span>         | <span data-ttu-id="623df-p110">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="623df-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="623df-238">**lists**</span><span class="sxs-lookup"><span data-stu-id="623df-238">**lists**</span></span>         | <span data-ttu-id="623df-239">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="623df-239">Collection([list][])</span></span>             | <span data-ttu-id="623df-240">此网站下的列表集合。</span><span class="sxs-lookup"><span data-stu-id="623df-240">The collection of lists under this site.</span></span>
| <span data-ttu-id="623df-241">**pages**</span><span class="sxs-lookup"><span data-stu-id="623df-241">**pages**</span></span>         | <span data-ttu-id="623df-242">Collection([sitePage][])</span><span class="sxs-lookup"><span data-stu-id="623df-242">Collection([sitePage][])</span></span>         | <span data-ttu-id="623df-243">此网站的 SitePages 列表中的页面集合。</span><span class="sxs-lookup"><span data-stu-id="623df-243">The collection of pages in the SitePages list in this site.</span></span>
| <span data-ttu-id="623df-244">**权限**</span><span class="sxs-lookup"><span data-stu-id="623df-244">**permissions**</span></span>   | <span data-ttu-id="623df-245">集合([权限][])</span><span class="sxs-lookup"><span data-stu-id="623df-245">Collection([permission][])</span></span>         | <span data-ttu-id="623df-246">与网站关联的权限。</span><span class="sxs-lookup"><span data-stu-id="623df-246">The permissions associated with the site.</span></span> <span data-ttu-id="623df-247">可为空。</span><span class="sxs-lookup"><span data-stu-id="623df-247">Nullable.</span></span>
| <span data-ttu-id="623df-248">**sites**</span><span class="sxs-lookup"><span data-stu-id="623df-248">**sites**</span></span>         | <span data-ttu-id="623df-249">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="623df-249">Collection([site][])</span></span>             | <span data-ttu-id="623df-250">网站下的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="623df-250">The collection of the sub-sites under this site.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="623df-263">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="623df-263">JSON representation</span></span>

<span data-ttu-id="623df-264">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="623df-264">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="623df-265">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="623df-265">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
