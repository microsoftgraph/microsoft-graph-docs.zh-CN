---
author: JeremyKelley
description: ”列表”资源代表网站中的列表。
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: a7e59cf2e81371428e3816acc6e89c4a102ca40e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522958"
---
# <a name="list-resource"></a><span data-ttu-id="aa498-103">List 资源</span><span class="sxs-lookup"><span data-stu-id="aa498-103">List resource</span></span>

<span data-ttu-id="aa498-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="aa498-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa498-105">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="aa498-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="aa498-106">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="aa498-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="aa498-107">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="aa498-107">Tasks on a list</span></span>

<span data-ttu-id="aa498-108">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="aa498-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="aa498-109">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="aa498-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="aa498-110">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="aa498-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="aa498-111">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="aa498-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="aa498-112">常见任务</span><span class="sxs-lookup"><span data-stu-id="aa498-112">Common task</span></span>               | <span data-ttu-id="aa498-113">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="aa498-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="aa498-114">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="aa498-114">[Get list][]</span></span>              | <span data-ttu-id="aa498-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="aa498-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="aa498-116">[创建列表][]</span><span class="sxs-lookup"><span data-stu-id="aa498-116">[Create list][]</span></span>           | <span data-ttu-id="aa498-117">POST /列表</span><span class="sxs-lookup"><span data-stu-id="aa498-117">POST /lists</span></span>
| <span data-ttu-id="aa498-118">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="aa498-118">[Enumerate list items][]</span></span>  | <span data-ttu-id="aa498-119">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="aa498-119">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="aa498-120">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="aa498-120">[Update list item][]</span></span>      | <span data-ttu-id="aa498-121">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="aa498-121">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="aa498-122">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="aa498-122">[Delete list item][]</span></span>      | <span data-ttu-id="aa498-123">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="aa498-123">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="aa498-124">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="aa498-124">[Create list item][]</span></span>      | <span data-ttu-id="aa498-125">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="aa498-125">POST /lists/{list-id}</span></span>
| <span data-ttu-id="aa498-126">[获取最近的活动][]</span><span class="sxs-lookup"><span data-stu-id="aa498-126">[Get recent activities][]</span></span> | <span data-ttu-id="aa498-127">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="aa498-127">GET /lists/{list-id}/activities</span></span>
| <span data-ttu-id="aa498-128">[获取 WebSocket 频道][]</span><span class="sxs-lookup"><span data-stu-id="aa498-128">[Get WebSocket channel][]</span></span> | <span data-ttu-id="aa498-129">获取/lists/{list-id}/subscriptions/socketIo</span><span class="sxs-lookup"><span data-stu-id="aa498-129">GET /lists/{list-id}/subscriptions/socketIo</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="aa498-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa498-138">JSON representation</span></span>

<span data-ttu-id="aa498-139">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa498-139">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="aa498-140">属性</span><span class="sxs-lookup"><span data-stu-id="aa498-140">Properties</span></span>

<span data-ttu-id="aa498-141">\*\*list \*\*资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="aa498-141">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="aa498-142">属性名称</span><span class="sxs-lookup"><span data-stu-id="aa498-142">Property name</span></span>    | <span data-ttu-id="aa498-143">类型</span><span class="sxs-lookup"><span data-stu-id="aa498-143">Type</span></span>                             | <span data-ttu-id="aa498-144">说明</span><span class="sxs-lookup"><span data-stu-id="aa498-144">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="aa498-145">**columns**</span><span class="sxs-lookup"><span data-stu-id="aa498-145">**columns**</span></span>      | <span data-ttu-id="aa498-146">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="aa498-146">Collection([columnDefinition][])</span></span> | <span data-ttu-id="aa498-147">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="aa498-147">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="aa498-148">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="aa498-148">**contentTypes**</span></span> | <span data-ttu-id="aa498-149">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="aa498-149">Collection([contentType][])</span></span>      | <span data-ttu-id="aa498-150">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="aa498-150">The collection of content types present in this list.</span></span>
| <span data-ttu-id="aa498-151">**displayName**</span><span class="sxs-lookup"><span data-stu-id="aa498-151">**displayName**</span></span>  | <span data-ttu-id="aa498-152">string</span><span class="sxs-lookup"><span data-stu-id="aa498-152">string</span></span>                           | <span data-ttu-id="aa498-153">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="aa498-153">The displayable title of the list.</span></span>
| <span data-ttu-id="aa498-154">**list**</span><span class="sxs-lookup"><span data-stu-id="aa498-154">**list**</span></span>         | <span data-ttu-id="aa498-155">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="aa498-155">[listInfo][]</span></span>                     | <span data-ttu-id="aa498-156">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="aa498-156">Provides additional details about the list.</span></span>
| <span data-ttu-id="aa498-157">**system**</span><span class="sxs-lookup"><span data-stu-id="aa498-157">**system**</span></span>       | <span data-ttu-id="aa498-158">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="aa498-158">[systemFacet][]</span></span>                  | <span data-ttu-id="aa498-159">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="aa498-159">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="aa498-160">只读。</span><span class="sxs-lookup"><span data-stu-id="aa498-160">Read-only.</span></span>

<span data-ttu-id="aa498-161">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="aa498-161">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="aa498-162">属性名称</span><span class="sxs-lookup"><span data-stu-id="aa498-162">Property name</span></span>            | <span data-ttu-id="aa498-163">类型</span><span class="sxs-lookup"><span data-stu-id="aa498-163">Type</span></span>             | <span data-ttu-id="aa498-164">说明</span><span class="sxs-lookup"><span data-stu-id="aa498-164">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="aa498-165">**id**</span><span class="sxs-lookup"><span data-stu-id="aa498-165">**id**</span></span>                   | <span data-ttu-id="aa498-166">string</span><span class="sxs-lookup"><span data-stu-id="aa498-166">string</span></span>           | <span data-ttu-id="aa498-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="aa498-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="aa498-169">**名称**</span><span class="sxs-lookup"><span data-stu-id="aa498-169">**name**</span></span>                 | <span data-ttu-id="aa498-170">string</span><span class="sxs-lookup"><span data-stu-id="aa498-170">string</span></span>           | <span data-ttu-id="aa498-171">项目名称。</span><span class="sxs-lookup"><span data-stu-id="aa498-171">The name of the item.</span></span>
| <span data-ttu-id="aa498-172">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="aa498-172">**createdBy**</span></span>            | <span data-ttu-id="aa498-173">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="aa498-173">[identitySet][]</span></span>  | <span data-ttu-id="aa498-174">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="aa498-174">Identity of the creator of this item.</span></span> <span data-ttu-id="aa498-175">只读。</span><span class="sxs-lookup"><span data-stu-id="aa498-175">Read-only.</span></span>
| <span data-ttu-id="aa498-176">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="aa498-176">**createdDateTime**</span></span>      | <span data-ttu-id="aa498-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa498-177">DateTimeOffset</span></span>   | <span data-ttu-id="aa498-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="aa498-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="aa498-180">**说明**</span><span class="sxs-lookup"><span data-stu-id="aa498-180">**description**</span></span>          | <span data-ttu-id="aa498-181">string</span><span class="sxs-lookup"><span data-stu-id="aa498-181">string</span></span>           | <span data-ttu-id="aa498-182">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="aa498-182">The descriptive text for the item.</span></span>
| <span data-ttu-id="aa498-183">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="aa498-183">**lastModifiedBy**</span></span>       | <span data-ttu-id="aa498-184">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="aa498-184">[identitySet][]</span></span>  | <span data-ttu-id="aa498-185">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="aa498-185">Identity of the last modifier of this item.</span></span> <span data-ttu-id="aa498-186">只读。</span><span class="sxs-lookup"><span data-stu-id="aa498-186">Read-only.</span></span>
| <span data-ttu-id="aa498-187">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="aa498-187">**lastModifiedDateTime**</span></span> | <span data-ttu-id="aa498-188">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa498-188">DateTimeOffset</span></span>   | <span data-ttu-id="aa498-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="aa498-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="aa498-191">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="aa498-191">**webUrl**</span></span>               | <span data-ttu-id="aa498-192">string (url)</span><span class="sxs-lookup"><span data-stu-id="aa498-192">string (url)</span></span>     | <span data-ttu-id="aa498-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="aa498-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="aa498-195">关系</span><span class="sxs-lookup"><span data-stu-id="aa498-195">Relationships</span></span>

<span data-ttu-id="aa498-196">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="aa498-196">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="aa498-197">关系名称</span><span class="sxs-lookup"><span data-stu-id="aa498-197">Relationship name</span></span> | <span data-ttu-id="aa498-198">类型</span><span class="sxs-lookup"><span data-stu-id="aa498-198">Type</span></span>                        | <span data-ttu-id="aa498-199">说明</span><span class="sxs-lookup"><span data-stu-id="aa498-199">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="aa498-200">**activities**</span><span class="sxs-lookup"><span data-stu-id="aa498-200">**activities**</span></span>    | <span data-ttu-id="aa498-201">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="aa498-201">[itemActivity][] collection</span></span> | <span data-ttu-id="aa498-202">最近发生在此列表内的活动。</span><span class="sxs-lookup"><span data-stu-id="aa498-202">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="aa498-203">**drive**</span><span class="sxs-lookup"><span data-stu-id="aa498-203">**drive**</span></span>         | <span data-ttu-id="aa498-204">[drive][]</span><span class="sxs-lookup"><span data-stu-id="aa498-204">[drive][]</span></span>                   | <span data-ttu-id="aa498-205">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="aa498-205">Only present on document libraries.</span></span> <span data-ttu-id="aa498-206">允许使用 [driveItems][driveItem] 作为 [drive][] 资源访问列表。</span><span class="sxs-lookup"><span data-stu-id="aa498-206">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="aa498-207">**项目**</span><span class="sxs-lookup"><span data-stu-id="aa498-207">**items**</span></span>         | <span data-ttu-id="aa498-208">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="aa498-208">Collection([listItem][])</span></span>    | <span data-ttu-id="aa498-209">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="aa498-209">All items contained in the list.</span></span>
| <span data-ttu-id="aa498-210">订阅</span><span class="sxs-lookup"><span data-stu-id="aa498-210">subscriptions</span></span>      | <span data-ttu-id="aa498-211">[订阅][]集合</span><span class="sxs-lookup"><span data-stu-id="aa498-211">[subscription][] collection</span></span> | <span data-ttu-id="aa498-212">列表上的一组订阅。</span><span class="sxs-lookup"><span data-stu-id="aa498-212">The set of subscriptions on the list.</span></span>

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
