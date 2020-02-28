---
author: JeremyKelley
description: ”列表”资源代表网站中的列表。
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 634ac31e5fa5de3700c238b4a931e5b43455e801
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331239"
---
# <a name="list-resource"></a><span data-ttu-id="55702-103">List 资源</span><span class="sxs-lookup"><span data-stu-id="55702-103">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55702-104">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="55702-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="55702-105">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="55702-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="55702-106">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="55702-106">Tasks on a list</span></span>

<span data-ttu-id="55702-107">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="55702-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="55702-108">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="55702-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="55702-109">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="55702-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="55702-110">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="55702-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="55702-111">常见任务</span><span class="sxs-lookup"><span data-stu-id="55702-111">Common task</span></span>               | <span data-ttu-id="55702-112">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="55702-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="55702-113">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="55702-113">[Get list][]</span></span>              | <span data-ttu-id="55702-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="55702-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="55702-115">[创建列表][]</span><span class="sxs-lookup"><span data-stu-id="55702-115">[Create list][]</span></span>           | <span data-ttu-id="55702-116">POST /列表</span><span class="sxs-lookup"><span data-stu-id="55702-116">POST /lists</span></span>
| <span data-ttu-id="55702-117">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="55702-117">[Enumerate list items][]</span></span>  | <span data-ttu-id="55702-118">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="55702-118">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="55702-119">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="55702-119">[Update list item][]</span></span>      | <span data-ttu-id="55702-120">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="55702-120">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="55702-121">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="55702-121">[Delete list item][]</span></span>      | <span data-ttu-id="55702-122">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="55702-122">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="55702-123">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="55702-123">[Create list item][]</span></span>      | <span data-ttu-id="55702-124">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="55702-124">POST /lists/{list-id}</span></span>
| <span data-ttu-id="55702-125">[获取最近的活动][]</span><span class="sxs-lookup"><span data-stu-id="55702-125">[Get recent activities][]</span></span> | <span data-ttu-id="55702-126">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="55702-126">GET /lists/{list-id}/activities</span></span>
| <span data-ttu-id="55702-127">[获取 WebSocket 频道][]</span><span class="sxs-lookup"><span data-stu-id="55702-127">[Get WebSocket channel][]</span></span> | <span data-ttu-id="55702-128">获取/lists/{list-id}/subscriptions/socketIo</span><span class="sxs-lookup"><span data-stu-id="55702-128">GET /lists/{list-id}/subscriptions/socketIo</span></span>

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
[获取 WebSocket 频道]: ../api/driveitem-subscriptions-socketio.md
[Get WebSocket channel]: ../api/driveitem-subscriptions-socketio.md

## <a name="json-representation"></a><span data-ttu-id="55702-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="55702-137">JSON representation</span></span>

<span data-ttu-id="55702-138">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55702-138">Here is a JSON representation of a **list** resource.</span></span>

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
    "template": "documentLibrary | genericList | survey | links | announcements | contacts ..."
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
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a><span data-ttu-id="55702-139">属性</span><span class="sxs-lookup"><span data-stu-id="55702-139">Properties</span></span>

<span data-ttu-id="55702-140">\*\*list \*\*资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="55702-140">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="55702-141">属性名称</span><span class="sxs-lookup"><span data-stu-id="55702-141">Property name</span></span>    | <span data-ttu-id="55702-142">类型</span><span class="sxs-lookup"><span data-stu-id="55702-142">Type</span></span>                             | <span data-ttu-id="55702-143">说明</span><span class="sxs-lookup"><span data-stu-id="55702-143">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="55702-144">**columns**</span><span class="sxs-lookup"><span data-stu-id="55702-144">**columns**</span></span>      | <span data-ttu-id="55702-145">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="55702-145">Collection([columnDefinition][])</span></span> | <span data-ttu-id="55702-146">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="55702-146">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="55702-147">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="55702-147">**contentTypes**</span></span> | <span data-ttu-id="55702-148">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="55702-148">Collection([contentType][])</span></span>      | <span data-ttu-id="55702-149">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="55702-149">The collection of content types present in this list.</span></span>
| <span data-ttu-id="55702-150">**displayName**</span><span class="sxs-lookup"><span data-stu-id="55702-150">**displayName**</span></span>  | <span data-ttu-id="55702-151">string</span><span class="sxs-lookup"><span data-stu-id="55702-151">string</span></span>                           | <span data-ttu-id="55702-152">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="55702-152">The displayable title of the list.</span></span>
| <span data-ttu-id="55702-153">**list**</span><span class="sxs-lookup"><span data-stu-id="55702-153">**list**</span></span>         | <span data-ttu-id="55702-154">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="55702-154">[listInfo][]</span></span>                     | <span data-ttu-id="55702-155">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="55702-155">Provides additional details about the list.</span></span>
| <span data-ttu-id="55702-156">**system**</span><span class="sxs-lookup"><span data-stu-id="55702-156">**system**</span></span>       | <span data-ttu-id="55702-157">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="55702-157">[systemFacet][]</span></span>                  | <span data-ttu-id="55702-158">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="55702-158">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="55702-159">只读。</span><span class="sxs-lookup"><span data-stu-id="55702-159">Read-only.</span></span>

<span data-ttu-id="55702-160">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="55702-160">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="55702-161">属性名称</span><span class="sxs-lookup"><span data-stu-id="55702-161">Property name</span></span>            | <span data-ttu-id="55702-162">类型</span><span class="sxs-lookup"><span data-stu-id="55702-162">Type</span></span>             | <span data-ttu-id="55702-163">说明</span><span class="sxs-lookup"><span data-stu-id="55702-163">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="55702-164">**id**</span><span class="sxs-lookup"><span data-stu-id="55702-164">**id**</span></span>                   | <span data-ttu-id="55702-165">string</span><span class="sxs-lookup"><span data-stu-id="55702-165">string</span></span>           | <span data-ttu-id="55702-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="55702-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="55702-168">**名称**</span><span class="sxs-lookup"><span data-stu-id="55702-168">**name**</span></span>                 | <span data-ttu-id="55702-169">string</span><span class="sxs-lookup"><span data-stu-id="55702-169">string</span></span>           | <span data-ttu-id="55702-170">项目名称。</span><span class="sxs-lookup"><span data-stu-id="55702-170">The name of the item.</span></span>
| <span data-ttu-id="55702-171">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="55702-171">**createdBy**</span></span>            | <span data-ttu-id="55702-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="55702-172">[identitySet][]</span></span>  | <span data-ttu-id="55702-173">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="55702-173">Identity of the creator of this item.</span></span> <span data-ttu-id="55702-174">只读。</span><span class="sxs-lookup"><span data-stu-id="55702-174">Read-only.</span></span>
| <span data-ttu-id="55702-175">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="55702-175">**createdDateTime**</span></span>      | <span data-ttu-id="55702-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55702-176">DateTimeOffset</span></span>   | <span data-ttu-id="55702-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="55702-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="55702-179">**说明**</span><span class="sxs-lookup"><span data-stu-id="55702-179">**description**</span></span>          | <span data-ttu-id="55702-180">string</span><span class="sxs-lookup"><span data-stu-id="55702-180">string</span></span>           | <span data-ttu-id="55702-181">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="55702-181">The descriptive text for the item.</span></span>
| <span data-ttu-id="55702-182">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="55702-182">**lastModifiedBy**</span></span>       | <span data-ttu-id="55702-183">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="55702-183">[identitySet][]</span></span>  | <span data-ttu-id="55702-184">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="55702-184">Identity of the last modifier of this item.</span></span> <span data-ttu-id="55702-185">只读。</span><span class="sxs-lookup"><span data-stu-id="55702-185">Read-only.</span></span>
| <span data-ttu-id="55702-186">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="55702-186">**lastModifiedDateTime**</span></span> | <span data-ttu-id="55702-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55702-187">DateTimeOffset</span></span>   | <span data-ttu-id="55702-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="55702-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="55702-190">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="55702-190">**webUrl**</span></span>               | <span data-ttu-id="55702-191">string (url)</span><span class="sxs-lookup"><span data-stu-id="55702-191">string (url)</span></span>     | <span data-ttu-id="55702-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="55702-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="55702-194">关系</span><span class="sxs-lookup"><span data-stu-id="55702-194">Relationships</span></span>

<span data-ttu-id="55702-195">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="55702-195">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="55702-196">关系名称</span><span class="sxs-lookup"><span data-stu-id="55702-196">Relationship name</span></span> | <span data-ttu-id="55702-197">类型</span><span class="sxs-lookup"><span data-stu-id="55702-197">Type</span></span>                        | <span data-ttu-id="55702-198">说明</span><span class="sxs-lookup"><span data-stu-id="55702-198">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="55702-199">**activities**</span><span class="sxs-lookup"><span data-stu-id="55702-199">**activities**</span></span>    | <span data-ttu-id="55702-200">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="55702-200">[itemActivity][] collection</span></span> | <span data-ttu-id="55702-201">最近发生在此列表内的活动。</span><span class="sxs-lookup"><span data-stu-id="55702-201">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="55702-202">**drive**</span><span class="sxs-lookup"><span data-stu-id="55702-202">**drive**</span></span>         | <span data-ttu-id="55702-203">[drive][]</span><span class="sxs-lookup"><span data-stu-id="55702-203">[drive][]</span></span>                   | <span data-ttu-id="55702-204">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="55702-204">Only present on document libraries.</span></span> <span data-ttu-id="55702-205">允许使用 [driveItems][driveItem] 作为 [drive][] 资源访问列表。</span><span class="sxs-lookup"><span data-stu-id="55702-205">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="55702-206">**项目**</span><span class="sxs-lookup"><span data-stu-id="55702-206">**items**</span></span>         | <span data-ttu-id="55702-207">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="55702-207">Collection([listItem][])</span></span>    | <span data-ttu-id="55702-208">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="55702-208">All items contained in the list.</span></span>
| <span data-ttu-id="55702-209">订阅</span><span class="sxs-lookup"><span data-stu-id="55702-209">subscriptions</span></span>      | <span data-ttu-id="55702-210">[订阅][]集合</span><span class="sxs-lookup"><span data-stu-id="55702-210">[subscription][] collection</span></span> | <span data-ttu-id="55702-211">列表上的一组订阅。</span><span class="sxs-lookup"><span data-stu-id="55702-211">The set of subscriptions on the list.</span></span>

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
    "Lists": "#"
  },
  "suppressions": []
}
-->
