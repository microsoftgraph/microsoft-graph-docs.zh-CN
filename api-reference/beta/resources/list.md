---
author: JeremyKelley
description: ”列表”资源代表网站中的列表。
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 30d26dfd3e140f302c6535cd6603a90568dbb567
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317096"
---
# <a name="list-resource"></a><span data-ttu-id="de07b-103">List 资源</span><span class="sxs-lookup"><span data-stu-id="de07b-103">List resource</span></span>

<span data-ttu-id="de07b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de07b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de07b-105">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="de07b-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="de07b-106">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="de07b-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="de07b-107">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="de07b-107">Tasks on a list</span></span>

<span data-ttu-id="de07b-108">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="de07b-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="de07b-109">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="de07b-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="de07b-110">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="de07b-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="de07b-111">下面的所有示例都相对于网站，例如， `https://graph.microsoft.com/beta/sites/{site-id}` 。</span><span class="sxs-lookup"><span data-stu-id="de07b-111">All examples below are relative to a site, for example, `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="de07b-112">常见任务</span><span class="sxs-lookup"><span data-stu-id="de07b-112">Common task</span></span>               | <span data-ttu-id="de07b-113">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="de07b-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="de07b-114">[获取网站中的列表][]</span><span class="sxs-lookup"><span data-stu-id="de07b-114">[Get lists in a site][]</span></span>   | <span data-ttu-id="de07b-115">GET /sites/{site-id}/lists</span><span class="sxs-lookup"><span data-stu-id="de07b-115">GET /sites/{site-id}/lists</span></span>
| <span data-ttu-id="de07b-116">[创建列表][]</span><span class="sxs-lookup"><span data-stu-id="de07b-116">[Create list][]</span></span>           | <span data-ttu-id="de07b-117">POST /列表</span><span class="sxs-lookup"><span data-stu-id="de07b-117">POST /lists</span></span>
| <span data-ttu-id="de07b-118">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="de07b-118">[Get list][]</span></span>              | <span data-ttu-id="de07b-119">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="de07b-119">GET /lists/{list-id}</span></span>
| <span data-ttu-id="de07b-120">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="de07b-120">[Enumerate list items][]</span></span>  | <span data-ttu-id="de07b-121">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="de07b-121">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="de07b-122">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="de07b-122">[Update list item][]</span></span>      | <span data-ttu-id="de07b-123">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="de07b-123">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="de07b-124">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="de07b-124">[Delete list item][]</span></span>      | <span data-ttu-id="de07b-125">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="de07b-125">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="de07b-126">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="de07b-126">[Create list item][]</span></span>      | <span data-ttu-id="de07b-127">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="de07b-127">POST /lists/{list-id}</span></span>
| <span data-ttu-id="de07b-128">[获取最近的活动][]</span><span class="sxs-lookup"><span data-stu-id="de07b-128">[Get recent activities][]</span></span> | <span data-ttu-id="de07b-129">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="de07b-129">GET /lists/{list-id}/activities</span></span>
| <span data-ttu-id="de07b-130">[获取 WebSocket 频道][]</span><span class="sxs-lookup"><span data-stu-id="de07b-130">[Get WebSocket channel][]</span></span> | <span data-ttu-id="de07b-131">GET /lists/{list-id}/subscriptions/socketIo</span><span class="sxs-lookup"><span data-stu-id="de07b-131">GET /lists/{list-id}/subscriptions/socketIo</span></span>
|<span data-ttu-id="de07b-132">[列表内容类型][]</span><span class="sxs-lookup"><span data-stu-id="de07b-132">[List content types][]</span></span>          | <span data-ttu-id="de07b-133">GET /lists/{list-id}/contentTypes</span><span class="sxs-lookup"><span data-stu-id="de07b-133">GET /lists/{list-id}/contentTypes</span></span>
|<span data-ttu-id="de07b-134">[从网站添加内容类型副本][]</span><span class="sxs-lookup"><span data-stu-id="de07b-134">[Add copy of content type from site][]</span></span> | <span data-ttu-id="de07b-135">POST /lists/{list-id}/contentTypes/addCopy</span><span class="sxs-lookup"><span data-stu-id="de07b-135">POST /lists/{list-id}/contentTypes/addCopy</span></span>
|<span data-ttu-id="de07b-136">[List columns][]</span><span class="sxs-lookup"><span data-stu-id="de07b-136">[List columns][]</span></span>               | <span data-ttu-id="de07b-137">GET /lists/{list-id}/columns</span><span class="sxs-lookup"><span data-stu-id="de07b-137">GET /lists/{list-id}/columns</span></span>
|<span data-ttu-id="de07b-138">[创建列][]</span><span class="sxs-lookup"><span data-stu-id="de07b-138">[Create column][]</span></span>              | <span data-ttu-id="de07b-139">POST /lists/{list-id}/columns</span><span class="sxs-lookup"><span data-stu-id="de07b-139">POST /lists/{list-id}/columns</span></span>

[获取网站中的列表]: ../api/list-list.md
[Get lists in a site]: ../api/list-list.md
[获取列表]: ../api/list-get.md
[Get list]: ../api/list-get.md
[创建列表]: ../api/list-create.md
[Create list]: ../api/list-create.md
[枚举列表项]: ../api/listitem-list.md
[Enumerate list items]: ../api/listitem-list.md
[更新列表项]: ../api/listitem-update.md
[Update list item]: ../api/listitem-update.md
[删除列表项]: ../api/listitem-delete.md
[Delete list item]: ../api/listitem-delete.md
[创建列表项]: ../api/listitem-create.md
[Create list item]: ../api/listitem-create.md
[获取最近的活动]: ../api/activities-list.md
[Get recent activities]: ../api/activities-list.md
[获取 WebSocket 频道]: ../api/subscriptions-socketio.md
[Get WebSocket channel]: ../api/subscriptions-socketio.md
[列表内容类型]: ../api/list-list-contenttypes.md
[List content types]: ../api/list-list-contenttypes.md
[从网站添加内容类型副本]: ../api/contenttype-addCopy.md
[Add copy of content type from site]: ../api/contenttype-addCopy.md
[List columns]: ../api/list-list-columns.md
[创建列]: ../api/list-post-columns.md
[Create column]: ../api/list-post-columns.md
## <a name="json-representation"></a><span data-ttu-id="de07b-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de07b-153">JSON representation</span></span>

<span data-ttu-id="de07b-154">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de07b-154">Here is a JSON representation of a **list** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

```json
{
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template&quot;: &quot;documentLibrary | genericList | survey | links | announcements | contacts ..."
  },
  "system": false,
  "subscriptions": [ {"@odata.type": "microsoft.graph.subscription"} ],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of list",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of list",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl&quot;: &quot;url to visit the list in a browser"
}
```

## <a name="properties"></a><span data-ttu-id="de07b-155">属性</span><span class="sxs-lookup"><span data-stu-id="de07b-155">Properties</span></span>

<span data-ttu-id="de07b-156">**list** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="de07b-156">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="de07b-157">属性名称</span><span class="sxs-lookup"><span data-stu-id="de07b-157">Property name</span></span>    | <span data-ttu-id="de07b-158">类型</span><span class="sxs-lookup"><span data-stu-id="de07b-158">Type</span></span>                             | <span data-ttu-id="de07b-159">说明</span><span class="sxs-lookup"><span data-stu-id="de07b-159">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="de07b-160">**columns**</span><span class="sxs-lookup"><span data-stu-id="de07b-160">**columns**</span></span>      | <span data-ttu-id="de07b-161">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="de07b-161">Collection([columnDefinition][])</span></span> | <span data-ttu-id="de07b-162">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="de07b-162">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="de07b-163">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="de07b-163">**contentTypes**</span></span> | <span data-ttu-id="de07b-164">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="de07b-164">Collection([contentType][])</span></span>      | <span data-ttu-id="de07b-165">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="de07b-165">The collection of content types present in this list.</span></span>
| <span data-ttu-id="de07b-166">**displayName**</span><span class="sxs-lookup"><span data-stu-id="de07b-166">**displayName**</span></span>  | <span data-ttu-id="de07b-167">string</span><span class="sxs-lookup"><span data-stu-id="de07b-167">string</span></span>                           | <span data-ttu-id="de07b-168">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="de07b-168">The displayable title of the list.</span></span>
| <span data-ttu-id="de07b-169">**list**</span><span class="sxs-lookup"><span data-stu-id="de07b-169">**list**</span></span>         | <span data-ttu-id="de07b-170">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="de07b-170">[listInfo][]</span></span>                     | <span data-ttu-id="de07b-171">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="de07b-171">Provides additional details about the list.</span></span>
| <span data-ttu-id="de07b-172">**system**</span><span class="sxs-lookup"><span data-stu-id="de07b-172">**system**</span></span>       | <span data-ttu-id="de07b-173">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="de07b-173">[systemFacet][]</span></span>                  | <span data-ttu-id="de07b-174">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="de07b-174">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="de07b-175">只读。</span><span class="sxs-lookup"><span data-stu-id="de07b-175">Read-only.</span></span>

<span data-ttu-id="de07b-176">以下属性继承自 **[baseItem][]**。</span><span class="sxs-lookup"><span data-stu-id="de07b-176">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="de07b-177">属性名称</span><span class="sxs-lookup"><span data-stu-id="de07b-177">Property name</span></span>            | <span data-ttu-id="de07b-178">类型</span><span class="sxs-lookup"><span data-stu-id="de07b-178">Type</span></span>             | <span data-ttu-id="de07b-179">说明</span><span class="sxs-lookup"><span data-stu-id="de07b-179">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="de07b-180">**id**</span><span class="sxs-lookup"><span data-stu-id="de07b-180">**id**</span></span>                   | <span data-ttu-id="de07b-181">string</span><span class="sxs-lookup"><span data-stu-id="de07b-181">string</span></span>           | <span data-ttu-id="de07b-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="de07b-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="de07b-184">**名称**</span><span class="sxs-lookup"><span data-stu-id="de07b-184">**name**</span></span>                 | <span data-ttu-id="de07b-185">string</span><span class="sxs-lookup"><span data-stu-id="de07b-185">string</span></span>           | <span data-ttu-id="de07b-186">项目名称。</span><span class="sxs-lookup"><span data-stu-id="de07b-186">The name of the item.</span></span>
| <span data-ttu-id="de07b-187">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="de07b-187">**createdBy**</span></span>            | <span data-ttu-id="de07b-188">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="de07b-188">[identitySet][]</span></span>  | <span data-ttu-id="de07b-189">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="de07b-189">Identity of the creator of this item.</span></span> <span data-ttu-id="de07b-190">只读。</span><span class="sxs-lookup"><span data-stu-id="de07b-190">Read-only.</span></span>
| <span data-ttu-id="de07b-191">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="de07b-191">**createdDateTime**</span></span>      | <span data-ttu-id="de07b-192">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de07b-192">DateTimeOffset</span></span>   | <span data-ttu-id="de07b-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="de07b-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="de07b-195">**说明**</span><span class="sxs-lookup"><span data-stu-id="de07b-195">**description**</span></span>          | <span data-ttu-id="de07b-196">string</span><span class="sxs-lookup"><span data-stu-id="de07b-196">string</span></span>           | <span data-ttu-id="de07b-197">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="de07b-197">The descriptive text for the item.</span></span>
| <span data-ttu-id="de07b-198">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="de07b-198">**lastModifiedBy**</span></span>       | <span data-ttu-id="de07b-199">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="de07b-199">[identitySet][]</span></span>  | <span data-ttu-id="de07b-200">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="de07b-200">Identity of the last modifier of this item.</span></span> <span data-ttu-id="de07b-201">只读。</span><span class="sxs-lookup"><span data-stu-id="de07b-201">Read-only.</span></span>
| <span data-ttu-id="de07b-202">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="de07b-202">**lastModifiedDateTime**</span></span> | <span data-ttu-id="de07b-203">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de07b-203">DateTimeOffset</span></span>   | <span data-ttu-id="de07b-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="de07b-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="de07b-206">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="de07b-206">**webUrl**</span></span>               | <span data-ttu-id="de07b-207">string (url)</span><span class="sxs-lookup"><span data-stu-id="de07b-207">string (url)</span></span>     | <span data-ttu-id="de07b-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="de07b-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="de07b-210">关系</span><span class="sxs-lookup"><span data-stu-id="de07b-210">Relationships</span></span>

<span data-ttu-id="de07b-211">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="de07b-211">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="de07b-212">关系名称</span><span class="sxs-lookup"><span data-stu-id="de07b-212">Relationship name</span></span> | <span data-ttu-id="de07b-213">类型</span><span class="sxs-lookup"><span data-stu-id="de07b-213">Type</span></span>                        | <span data-ttu-id="de07b-214">说明</span><span class="sxs-lookup"><span data-stu-id="de07b-214">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="de07b-215">**activities**</span><span class="sxs-lookup"><span data-stu-id="de07b-215">**activities**</span></span>    | <span data-ttu-id="de07b-216">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="de07b-216">[itemActivity][] collection</span></span> | <span data-ttu-id="de07b-217">最近发生在此列表内的活动。</span><span class="sxs-lookup"><span data-stu-id="de07b-217">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="de07b-218">**drive**</span><span class="sxs-lookup"><span data-stu-id="de07b-218">**drive**</span></span>         | <span data-ttu-id="de07b-219">[drive][]</span><span class="sxs-lookup"><span data-stu-id="de07b-219">[drive][]</span></span>                   | <span data-ttu-id="de07b-220">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="de07b-220">Only present on document libraries.</span></span> <span data-ttu-id="de07b-221">允许使用 [driveItems][driveItem] 作为 [drive][] 资源访问列表。</span><span class="sxs-lookup"><span data-stu-id="de07b-221">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="de07b-222">**项目**</span><span class="sxs-lookup"><span data-stu-id="de07b-222">**items**</span></span>         | <span data-ttu-id="de07b-223">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="de07b-223">Collection([listItem][])</span></span>    | <span data-ttu-id="de07b-224">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="de07b-224">All items contained in the list.</span></span>
| <span data-ttu-id="de07b-225">订阅</span><span class="sxs-lookup"><span data-stu-id="de07b-225">subscriptions</span></span>      | <span data-ttu-id="de07b-226">[订阅][]集合</span><span class="sxs-lookup"><span data-stu-id="de07b-226">[subscription][] collection</span></span> | <span data-ttu-id="de07b-227">列表上的订阅集。</span><span class="sxs-lookup"><span data-stu-id="de07b-227">The set of subscriptions on the list.</span></span>

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[site]: site.md
[systemFacet]: systemfacet.md
[订阅]: subscription.md
[subscription]: subscription.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists&quot;: &quot;#"
  },
  "suppressions": []
}
-->


