---
author: JeremyKelley
ms.author: JeremyKelley
title: site 资源
description: site 资源提供 Sharepoint 网站的元数据和关系。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f351ee2a9fe107ede3317a46789810ae2bf24b33
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161367"
---
# <a name="site-resource"></a><span data-ttu-id="9d623-103">site 资源</span><span class="sxs-lookup"><span data-stu-id="9d623-103">site resource</span></span>

<span data-ttu-id="9d623-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d623-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9d623-105">**site** 资源提供 SharePoint 网站的元数据和关系。</span><span class="sxs-lookup"><span data-stu-id="9d623-105">The **site** resource provides metadata and relationships for a SharePoint site.</span></span>

## <a name="methods"></a><span data-ttu-id="9d623-106">方法</span><span class="sxs-lookup"><span data-stu-id="9d623-106">Methods</span></span>

| <span data-ttu-id="9d623-107">方法</span><span class="sxs-lookup"><span data-stu-id="9d623-107">Method</span></span>                | <span data-ttu-id="9d623-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9d623-108">Return type</span></span> | <span data-ttu-id="9d623-109">说明</span><span class="sxs-lookup"><span data-stu-id="9d623-109">Description</span></span>
|:-------------------------|:-------------|:----------
| <span data-ttu-id="9d623-110">[获取根网站][]</span><span class="sxs-lookup"><span data-stu-id="9d623-110">[Get root site][]</span></span>        | <span data-ttu-id="9d623-111">网站</span><span class="sxs-lookup"><span data-stu-id="9d623-111">site</span></span> | <span data-ttu-id="9d623-112">访问租户内的根 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="9d623-112">Access the root SharePoint site within a tenant.</span></span>
| <span data-ttu-id="9d623-113">[获取网站][]</span><span class="sxs-lookup"><span data-stu-id="9d623-113">[Get site][]</span></span>             | <span data-ttu-id="9d623-114">网站</span><span class="sxs-lookup"><span data-stu-id="9d623-114">site</span></span> | <span data-ttu-id="9d623-115">使用 siteId 访问 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="9d623-115">Access a sharePoint site using the siteId.</span></span>
| <span data-ttu-id="9d623-116">[根据路径获取网站][]</span><span class="sxs-lookup"><span data-stu-id="9d623-116">[Get site by path][]</span></span>     | <span data-ttu-id="9d623-117">网站</span><span class="sxs-lookup"><span data-stu-id="9d623-117">site</span></span> | <span data-ttu-id="9d623-118">通过相对路径访问根 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="9d623-118">Access the root SharePoint site with a relative path.</span></span>
| <span data-ttu-id="9d623-119">[获取组的网站][]</span><span class="sxs-lookup"><span data-stu-id="9d623-119">[Get site for a group][]</span></span> | <span data-ttu-id="9d623-120">网站</span><span class="sxs-lookup"><span data-stu-id="9d623-120">site</span></span> | <span data-ttu-id="9d623-121">访问组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="9d623-121">Access the team site for a group.</span></span>
| <span data-ttu-id="9d623-122">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="9d623-122">[Get analytics][]</span></span>              | <span data-ttu-id="9d623-123">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="9d623-123">[itemAnalytics][]</span></span> | <span data-ttu-id="9d623-124">对此资源可获取分析。</span><span class="sxs-lookup"><span data-stu-id="9d623-124">Get analytics for this resource.</span></span> 
| <span data-ttu-id="9d623-125">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="9d623-125">[Get activities by interval][]</span></span> | <span data-ttu-id="9d623-126">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="9d623-126">[itemActivityStat][]</span></span> | <span data-ttu-id="9d623-127">在指定的时间间隔内获取 **itemActivityStats** 的集合。</span><span class="sxs-lookup"><span data-stu-id="9d623-127">Get a collection of **itemActivityStats** within the specified time interval.</span></span>
| <span data-ttu-id="9d623-128">[搜索网站][]</span><span class="sxs-lookup"><span data-stu-id="9d623-128">[Search for sites][]</span></span>     | <span data-ttu-id="9d623-129">网站集合</span><span class="sxs-lookup"><span data-stu-id="9d623-129">collection of site</span></span> | <span data-ttu-id="9d623-130">在 SharePoint 租户中搜索与所提供的关键字匹配的 网站。</span><span class="sxs-lookup"><span data-stu-id="9d623-130">Search across a SharePoint tenant for sites that match keywords provided.</span></span>
| <span data-ttu-id="9d623-131">[关注网站][]</span><span class="sxs-lookup"><span data-stu-id="9d623-131">[Follow site][]</span></span>          | <span data-ttu-id="9d623-132">网站集合</span><span class="sxs-lookup"><span data-stu-id="9d623-132">collection of site</span></span> | <span data-ttu-id="9d623-133">关注用户的网站或多个网站。</span><span class="sxs-lookup"><span data-stu-id="9d623-133">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="9d623-134">[取消关注网站][]</span><span class="sxs-lookup"><span data-stu-id="9d623-134">[Unfollow site][]</span></span>        | <span data-ttu-id="9d623-135">网站集合</span><span class="sxs-lookup"><span data-stu-id="9d623-135">collection of site</span></span> | <span data-ttu-id="9d623-136">关注用户的网站或多个网站。</span><span class="sxs-lookup"><span data-stu-id="9d623-136">Follow a user's site or multiple sites.</span></span>
| <span data-ttu-id="9d623-137">[关注网站列表][]</span><span class="sxs-lookup"><span data-stu-id="9d623-137">[List followed sites][]</span></span>  | <span data-ttu-id="9d623-138">网站集合</span><span class="sxs-lookup"><span data-stu-id="9d623-138">collection of site</span></span> | <span data-ttu-id="9d623-139">已登录用户的关注网站列表。</span><span class="sxs-lookup"><span data-stu-id="9d623-139">List the sites that have been followed by the signed in user.</span></span>
| <span data-ttu-id="9d623-140">[获取权限][]</span><span class="sxs-lookup"><span data-stu-id="9d623-140">[Get permission][]</span></span>             | <span data-ttu-id="9d623-141">GET /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="9d623-141">GET /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="9d623-142">[列出权限][]</span><span class="sxs-lookup"><span data-stu-id="9d623-142">[List permissions][]</span></span>           | <span data-ttu-id="9d623-143">GET /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="9d623-143">GET /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="9d623-144">[创建权限][]</span><span class="sxs-lookup"><span data-stu-id="9d623-144">[Create permissions][]</span></span>         | <span data-ttu-id="9d623-145">POST /sites/{site-id}/permissions</span><span class="sxs-lookup"><span data-stu-id="9d623-145">POST /sites/{site-id}/permissions</span></span>
| <span data-ttu-id="9d623-146">[删除权限][]</span><span class="sxs-lookup"><span data-stu-id="9d623-146">[Delete permission][]</span></span>         | <span data-ttu-id="9d623-147">DELETE /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="9d623-147">DELETE /sites/{site-id}/permissions/{permission-id}</span></span>
| <span data-ttu-id="9d623-148">[更新权限][]</span><span class="sxs-lookup"><span data-stu-id="9d623-148">[Update permission][]</span></span>         | <span data-ttu-id="9d623-149">PATCH /sites/{site-id}/permissions/{permission-id}</span><span class="sxs-lookup"><span data-stu-id="9d623-149">PATCH /sites/{site-id}/permissions/{permission-id}</span></span>

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

## <a name="properties"></a><span data-ttu-id="9d623-166">属性</span><span class="sxs-lookup"><span data-stu-id="9d623-166">Properties</span></span>

| <span data-ttu-id="9d623-167">属性</span><span class="sxs-lookup"><span data-stu-id="9d623-167">Property</span></span>            | <span data-ttu-id="9d623-168">类型</span><span class="sxs-lookup"><span data-stu-id="9d623-168">Type</span></span>                                | <span data-ttu-id="9d623-169">说明</span><span class="sxs-lookup"><span data-stu-id="9d623-169">Description</span></span>                                                                                    |
| :----------------------- | :---------------------------------- | :--------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9d623-170">**id**</span><span class="sxs-lookup"><span data-stu-id="9d623-170">**id**</span></span>                   | <span data-ttu-id="9d623-171">string</span><span class="sxs-lookup"><span data-stu-id="9d623-171">string</span></span>                              | <span data-ttu-id="9d623-p101">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="9d623-p101">The unique identifier of the item. Read-only.</span></span>                                                  |
| <span data-ttu-id="9d623-174">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="9d623-174">**createdDateTime**</span></span>      | <span data-ttu-id="9d623-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d623-175">DateTimeOffset</span></span>                      | <span data-ttu-id="9d623-p102">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="9d623-p102">The date and time the item was created. Read-only.</span></span>                                             |
| <span data-ttu-id="9d623-178">**说明**</span><span class="sxs-lookup"><span data-stu-id="9d623-178">**description**</span></span>          | <span data-ttu-id="9d623-179">string</span><span class="sxs-lookup"><span data-stu-id="9d623-179">string</span></span>                              | <span data-ttu-id="9d623-180">网站的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="9d623-180">The descriptive text for the site.</span></span>                                                             |
| <span data-ttu-id="9d623-181">**displayName**</span><span class="sxs-lookup"><span data-stu-id="9d623-181">**displayName**</span></span>          | <span data-ttu-id="9d623-182">string</span><span class="sxs-lookup"><span data-stu-id="9d623-182">string</span></span>                              | <span data-ttu-id="9d623-p103">网站的完整标题。只读。</span><span class="sxs-lookup"><span data-stu-id="9d623-p103">The full title for the site. Read-only.</span></span>                                                        |
| <span data-ttu-id="9d623-185">**eTag**</span><span class="sxs-lookup"><span data-stu-id="9d623-185">**eTag**</span></span>                 | <span data-ttu-id="9d623-186">string</span><span class="sxs-lookup"><span data-stu-id="9d623-186">string</span></span>                              | <span data-ttu-id="9d623-p104">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="9d623-p104">ETag for the item. Read-only.</span></span>                                                                  |
| <span data-ttu-id="9d623-189">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="9d623-189">**lastModifiedDateTime**</span></span> | <span data-ttu-id="9d623-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d623-190">DateTimeOffset</span></span>                      | <span data-ttu-id="9d623-p105">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="9d623-p105">The date and time the item was last modified. Read-only.</span></span>                                       |
| <span data-ttu-id="9d623-193">**name**</span><span class="sxs-lookup"><span data-stu-id="9d623-193">**name**</span></span>                 | <span data-ttu-id="9d623-194">string</span><span class="sxs-lookup"><span data-stu-id="9d623-194">string</span></span>                              | <span data-ttu-id="9d623-195">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="9d623-195">The name / title of the item.</span></span>                                                                  |
| <span data-ttu-id="9d623-196">**根**</span><span class="sxs-lookup"><span data-stu-id="9d623-196">**root**</span></span>                 | [<span data-ttu-id="9d623-197">根</span><span class="sxs-lookup"><span data-stu-id="9d623-197">root</span></span>](root.md)                     | <span data-ttu-id="9d623-p106">如果存在，则表示这是网站集中的根网站。只读。</span><span class="sxs-lookup"><span data-stu-id="9d623-p106">If present, indicates that this is the root site in the site collection. Read-only.</span></span>            |
| <span data-ttu-id="9d623-200">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="9d623-200">**sharepointIds**</span></span>        | [<span data-ttu-id="9d623-201">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="9d623-201">sharepointIds</span></span>](sharepointids.md)   | <span data-ttu-id="9d623-p107">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="9d623-p107">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>                       |
| <span data-ttu-id="9d623-204">**siteCollection**</span><span class="sxs-lookup"><span data-stu-id="9d623-204">**siteCollection**</span></span>       | [<span data-ttu-id="9d623-205">siteCollection</span><span class="sxs-lookup"><span data-stu-id="9d623-205">siteCollection</span></span>](sitecollection.md) | <span data-ttu-id="9d623-p108">提供有关该网站的网站集的详细信息。仅在根网站上可用。只读。</span><span class="sxs-lookup"><span data-stu-id="9d623-p108">Provides details about the site's site collection. Available only on the root site. Read-only.</span></span> |
| <span data-ttu-id="9d623-209">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="9d623-209">**webUrl**</span></span>               | <span data-ttu-id="9d623-210">string (url)</span><span class="sxs-lookup"><span data-stu-id="9d623-210">string (url)</span></span>                        | <span data-ttu-id="9d623-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="9d623-p109">URL that displays the item in the browser. Read-only.</span></span>                                          |

### <a name="id-property"></a><span data-ttu-id="9d623-213">id 属性</span><span class="sxs-lookup"><span data-stu-id="9d623-213">id property</span></span>
<span data-ttu-id="9d623-214">**site** 由一个唯一 ID 标识，此唯一 ID 由以下值组成：</span><span class="sxs-lookup"><span data-stu-id="9d623-214">A **site** is identified by a unique ID that is a composite of the following values:</span></span>
* <span data-ttu-id="9d623-215">网站集主机名称 (contoso.sharepoint.com)</span><span class="sxs-lookup"><span data-stu-id="9d623-215">Site collection hostname (contoso.sharepoint.com)</span></span>
* <span data-ttu-id="9d623-216">网站集的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="9d623-216">Site collection unique ID (GUID)</span></span>
* <span data-ttu-id="9d623-217">网站的唯一 ID (GUID)</span><span class="sxs-lookup"><span data-stu-id="9d623-217">Site unique ID (GUID)</span></span>
  
<span data-ttu-id="9d623-218">`root` 标识符经常用于引用给定目标的根网站，如下所示：</span><span class="sxs-lookup"><span data-stu-id="9d623-218">The `root` identifier always references the root site for a given target, as follows:</span></span>

* <span data-ttu-id="9d623-219">`/sites/root`：租户根网站。</span><span class="sxs-lookup"><span data-stu-id="9d623-219">`/sites/root`: The tenant root site.</span></span>
* <span data-ttu-id="9d623-220">`/groups/{group-id}/sites/root`：该组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="9d623-220">`/groups/{group-id}/sites/root`: The group's team site.</span></span>
  
## <a name="relationships"></a><span data-ttu-id="9d623-221">关系</span><span class="sxs-lookup"><span data-stu-id="9d623-221">Relationships</span></span>

| <span data-ttu-id="9d623-222">关系</span><span class="sxs-lookup"><span data-stu-id="9d623-222">Relationship</span></span>      | <span data-ttu-id="9d623-223">类型</span><span class="sxs-lookup"><span data-stu-id="9d623-223">Type</span></span>                             | <span data-ttu-id="9d623-224">说明</span><span class="sxs-lookup"><span data-stu-id="9d623-224">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="9d623-225">**analytics**</span><span class="sxs-lookup"><span data-stu-id="9d623-225">**analytics**</span></span>     | <span data-ttu-id="9d623-226">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="9d623-226">[itemAnalytics][] resource</span></span>       | <span data-ttu-id="9d623-227">此网站上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="9d623-227">Analytics about the view activities that took place in this site.</span></span>
| <span data-ttu-id="9d623-228">**columns**</span><span class="sxs-lookup"><span data-stu-id="9d623-228">**columns**</span></span>       | <span data-ttu-id="9d623-229">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="9d623-229">Collection([columnDefinition][])</span></span> | <span data-ttu-id="9d623-230">可以在此网站下方的列表中重复使用的列定义集合。</span><span class="sxs-lookup"><span data-stu-id="9d623-230">The collection of column definitions reusable across lists under this site.</span></span>
| <span data-ttu-id="9d623-231">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="9d623-231">**contentTypes**</span></span>  | <span data-ttu-id="9d623-232">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="9d623-232">Collection([contentType][])</span></span>      | <span data-ttu-id="9d623-233">为此网站定义的内容类型集合。</span><span class="sxs-lookup"><span data-stu-id="9d623-233">The collection of content types defined for this site.</span></span>
| <span data-ttu-id="9d623-234">**drive**</span><span class="sxs-lookup"><span data-stu-id="9d623-234">**drive**</span></span>         | <span data-ttu-id="9d623-235">[drive][]</span><span class="sxs-lookup"><span data-stu-id="9d623-235">[drive][]</span></span>                        | <span data-ttu-id="9d623-236">此网站的默认驱动器（文档库）。</span><span class="sxs-lookup"><span data-stu-id="9d623-236">The default drive (document library) for this site.</span></span>
| <span data-ttu-id="9d623-237">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="9d623-237">**drives**</span></span>        | <span data-ttu-id="9d623-238">集合（[drive][]）</span><span class="sxs-lookup"><span data-stu-id="9d623-238">Collection([drive][])</span></span>            | <span data-ttu-id="9d623-239">网站下方的驱动器集合（文档库）。</span><span class="sxs-lookup"><span data-stu-id="9d623-239">The collection of drives (document libraries) under this site.</span></span>
| <span data-ttu-id="9d623-240">**项目**</span><span class="sxs-lookup"><span data-stu-id="9d623-240">**items**</span></span>         | <span data-ttu-id="9d623-241">集合 ([baseItem][])</span><span class="sxs-lookup"><span data-stu-id="9d623-241">Collection([baseItem][])</span></span>         | <span data-ttu-id="9d623-p110">用于处理包含在此网站中的任何项目。不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="9d623-p110">Used to address any item contained in this site. This collection cannot be enumerated.</span></span>
| <span data-ttu-id="9d623-244">**lists**</span><span class="sxs-lookup"><span data-stu-id="9d623-244">**lists**</span></span>         | <span data-ttu-id="9d623-245">Collection([list][])</span><span class="sxs-lookup"><span data-stu-id="9d623-245">Collection([list][])</span></span>             | <span data-ttu-id="9d623-246">此网站下方的列表集合。</span><span class="sxs-lookup"><span data-stu-id="9d623-246">The collection of lists under this site.</span></span>
| <span data-ttu-id="9d623-247">**权限**</span><span class="sxs-lookup"><span data-stu-id="9d623-247">**permissions**</span></span>   | <span data-ttu-id="9d623-248">集合([权限][])</span><span class="sxs-lookup"><span data-stu-id="9d623-248">Collection([permission][])</span></span>         | <span data-ttu-id="9d623-249">与网站关联的权限。</span><span class="sxs-lookup"><span data-stu-id="9d623-249">The permissions associated with the site.</span></span> <span data-ttu-id="9d623-250">可为空。</span><span class="sxs-lookup"><span data-stu-id="9d623-250">Nullable.</span></span>
| <span data-ttu-id="9d623-251">**sites**</span><span class="sxs-lookup"><span data-stu-id="9d623-251">**sites**</span></span>         | <span data-ttu-id="9d623-252">集合（[网站][]）</span><span class="sxs-lookup"><span data-stu-id="9d623-252">Collection([site][])</span></span>             | <span data-ttu-id="9d623-253">网站下方的子网站的集合。</span><span class="sxs-lookup"><span data-stu-id="9d623-253">The collection of the sub-sites under this site.</span></span>
| <span data-ttu-id="9d623-254">**onenote**</span><span class="sxs-lookup"><span data-stu-id="9d623-254">**onenote**</span></span>       | <span data-ttu-id="9d623-255">[onenote][]</span><span class="sxs-lookup"><span data-stu-id="9d623-255">[onenote][]</span></span>                      | <span data-ttu-id="9d623-256">调用 OneNote 服务执行笔记本相关操作。</span><span class="sxs-lookup"><span data-stu-id="9d623-256">Calls the OneNote service for notebook related operations.</span></span>

[columnDefinition]: columndefinition.md
[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[identitySet]: identityset.md
[itemAnalytics]: itemanalytics.md
[list]: list.md
[权限]: permission.md
[permission]: permission.md
[网站]: site.md
[site]: site.md
[onenote]: onenote.md

## <a name="json-representation"></a><span data-ttu-id="9d623-266">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d623-266">JSON representation</span></span>

<span data-ttu-id="9d623-267">下面是 **site** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d623-267">Here is a JSON representation of a **site** resource.</span></span>

<span data-ttu-id="9d623-268">**site** 资源派生自 [**baseItem**](baseitem.md)，并继承此资源的属性。</span><span class="sxs-lookup"><span data-stu-id="9d623-268">The **site** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
