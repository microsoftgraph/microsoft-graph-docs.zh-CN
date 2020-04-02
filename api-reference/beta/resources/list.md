---
author: JeremyKelley
description: ”列表”资源代表网站中的列表。
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 861e3c0b90c68ebf7a4a554e94097f790182727e
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43109045"
---
# <a name="list-resource"></a><span data-ttu-id="d8cf9-103">List 资源</span><span class="sxs-lookup"><span data-stu-id="d8cf9-103">List resource</span></span>

<span data-ttu-id="d8cf9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8cf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8cf9-105">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="d8cf9-106">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="d8cf9-107">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="d8cf9-107">Tasks on a list</span></span>

<span data-ttu-id="d8cf9-108">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="d8cf9-109">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="d8cf9-110">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="d8cf9-111">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="d8cf9-112">常见任务</span><span class="sxs-lookup"><span data-stu-id="d8cf9-112">Common task</span></span>               | <span data-ttu-id="d8cf9-113">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="d8cf9-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="d8cf9-114">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-114">[Get list][]</span></span>              | <span data-ttu-id="d8cf9-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="d8cf9-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="d8cf9-116">[创建列表][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-116">[Create list][]</span></span>           | <span data-ttu-id="d8cf9-117">POST /列表</span><span class="sxs-lookup"><span data-stu-id="d8cf9-117">POST /lists</span></span>
| <span data-ttu-id="d8cf9-118">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-118">[Enumerate list items][]</span></span>  | <span data-ttu-id="d8cf9-119">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="d8cf9-119">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="d8cf9-120">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-120">[Update list item][]</span></span>      | <span data-ttu-id="d8cf9-121">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="d8cf9-121">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="d8cf9-122">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-122">[Delete list item][]</span></span>      | <span data-ttu-id="d8cf9-123">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="d8cf9-123">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="d8cf9-124">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-124">[Create list item][]</span></span>      | <span data-ttu-id="d8cf9-125">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="d8cf9-125">POST /lists/{list-id}</span></span>
| <span data-ttu-id="d8cf9-126">[获取最近的活动][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-126">[Get recent activities][]</span></span> | <span data-ttu-id="d8cf9-127">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="d8cf9-127">GET /lists/{list-id}/activities</span></span>
| <span data-ttu-id="d8cf9-128">[获取 WebSocket 频道][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-128">[Get WebSocket channel][]</span></span> | <span data-ttu-id="d8cf9-129">获取/lists/{list-id}/subscriptions/socketIo</span><span class="sxs-lookup"><span data-stu-id="d8cf9-129">GET /lists/{list-id}/subscriptions/socketIo</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="d8cf9-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8cf9-138">JSON representation</span></span>

<span data-ttu-id="d8cf9-139">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-139">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d8cf9-140">属性</span><span class="sxs-lookup"><span data-stu-id="d8cf9-140">Properties</span></span>

<span data-ttu-id="d8cf9-141">\*\*list \*\*资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-141">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="d8cf9-142">属性名称</span><span class="sxs-lookup"><span data-stu-id="d8cf9-142">Property name</span></span>    | <span data-ttu-id="d8cf9-143">类型</span><span class="sxs-lookup"><span data-stu-id="d8cf9-143">Type</span></span>                             | <span data-ttu-id="d8cf9-144">说明</span><span class="sxs-lookup"><span data-stu-id="d8cf9-144">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="d8cf9-145">**columns**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-145">**columns**</span></span>      | <span data-ttu-id="d8cf9-146">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="d8cf9-146">Collection([columnDefinition][])</span></span> | <span data-ttu-id="d8cf9-147">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-147">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="d8cf9-148">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-148">**contentTypes**</span></span> | <span data-ttu-id="d8cf9-149">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="d8cf9-149">Collection([contentType][])</span></span>      | <span data-ttu-id="d8cf9-150">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-150">The collection of content types present in this list.</span></span>
| <span data-ttu-id="d8cf9-151">**displayName**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-151">**displayName**</span></span>  | <span data-ttu-id="d8cf9-152">string</span><span class="sxs-lookup"><span data-stu-id="d8cf9-152">string</span></span>                           | <span data-ttu-id="d8cf9-153">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-153">The displayable title of the list.</span></span>
| <span data-ttu-id="d8cf9-154">**list**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-154">**list**</span></span>         | <span data-ttu-id="d8cf9-155">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-155">[listInfo][]</span></span>                     | <span data-ttu-id="d8cf9-156">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-156">Provides additional details about the list.</span></span>
| <span data-ttu-id="d8cf9-157">**system**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-157">**system**</span></span>       | <span data-ttu-id="d8cf9-158">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-158">[systemFacet][]</span></span>                  | <span data-ttu-id="d8cf9-159">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-159">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="d8cf9-160">只读。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-160">Read-only.</span></span>

<span data-ttu-id="d8cf9-161">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-161">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="d8cf9-162">属性名称</span><span class="sxs-lookup"><span data-stu-id="d8cf9-162">Property name</span></span>            | <span data-ttu-id="d8cf9-163">类型</span><span class="sxs-lookup"><span data-stu-id="d8cf9-163">Type</span></span>             | <span data-ttu-id="d8cf9-164">说明</span><span class="sxs-lookup"><span data-stu-id="d8cf9-164">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="d8cf9-165">**id**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-165">**id**</span></span>                   | <span data-ttu-id="d8cf9-166">string</span><span class="sxs-lookup"><span data-stu-id="d8cf9-166">string</span></span>           | <span data-ttu-id="d8cf9-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="d8cf9-169">**名称**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-169">**name**</span></span>                 | <span data-ttu-id="d8cf9-170">string</span><span class="sxs-lookup"><span data-stu-id="d8cf9-170">string</span></span>           | <span data-ttu-id="d8cf9-171">项目名称。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-171">The name of the item.</span></span>
| <span data-ttu-id="d8cf9-172">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-172">**createdBy**</span></span>            | <span data-ttu-id="d8cf9-173">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-173">[identitySet][]</span></span>  | <span data-ttu-id="d8cf9-174">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-174">Identity of the creator of this item.</span></span> <span data-ttu-id="d8cf9-175">只读。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-175">Read-only.</span></span>
| <span data-ttu-id="d8cf9-176">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-176">**createdDateTime**</span></span>      | <span data-ttu-id="d8cf9-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8cf9-177">DateTimeOffset</span></span>   | <span data-ttu-id="d8cf9-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="d8cf9-180">**说明**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-180">**description**</span></span>          | <span data-ttu-id="d8cf9-181">string</span><span class="sxs-lookup"><span data-stu-id="d8cf9-181">string</span></span>           | <span data-ttu-id="d8cf9-182">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-182">The descriptive text for the item.</span></span>
| <span data-ttu-id="d8cf9-183">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-183">**lastModifiedBy**</span></span>       | <span data-ttu-id="d8cf9-184">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-184">[identitySet][]</span></span>  | <span data-ttu-id="d8cf9-185">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-185">Identity of the last modifier of this item.</span></span> <span data-ttu-id="d8cf9-186">只读。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-186">Read-only.</span></span>
| <span data-ttu-id="d8cf9-187">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-187">**lastModifiedDateTime**</span></span> | <span data-ttu-id="d8cf9-188">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8cf9-188">DateTimeOffset</span></span>   | <span data-ttu-id="d8cf9-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="d8cf9-191">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-191">**webUrl**</span></span>               | <span data-ttu-id="d8cf9-192">string (url)</span><span class="sxs-lookup"><span data-stu-id="d8cf9-192">string (url)</span></span>     | <span data-ttu-id="d8cf9-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="d8cf9-195">关系</span><span class="sxs-lookup"><span data-stu-id="d8cf9-195">Relationships</span></span>

<span data-ttu-id="d8cf9-196">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-196">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="d8cf9-197">关系名称</span><span class="sxs-lookup"><span data-stu-id="d8cf9-197">Relationship name</span></span> | <span data-ttu-id="d8cf9-198">类型</span><span class="sxs-lookup"><span data-stu-id="d8cf9-198">Type</span></span>                        | <span data-ttu-id="d8cf9-199">说明</span><span class="sxs-lookup"><span data-stu-id="d8cf9-199">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="d8cf9-200">**activities**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-200">**activities**</span></span>    | <span data-ttu-id="d8cf9-201">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="d8cf9-201">[itemActivity][] collection</span></span> | <span data-ttu-id="d8cf9-202">最近发生在此列表内的活动。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-202">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="d8cf9-203">**drive**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-203">**drive**</span></span>         | <span data-ttu-id="d8cf9-204">[drive][]</span><span class="sxs-lookup"><span data-stu-id="d8cf9-204">[drive][]</span></span>                   | <span data-ttu-id="d8cf9-205">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-205">Only present on document libraries.</span></span> <span data-ttu-id="d8cf9-206">允许使用 [driveItems][driveItem] 作为 [drive][] 资源访问列表。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-206">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="d8cf9-207">**项目**</span><span class="sxs-lookup"><span data-stu-id="d8cf9-207">**items**</span></span>         | <span data-ttu-id="d8cf9-208">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="d8cf9-208">Collection([listItem][])</span></span>    | <span data-ttu-id="d8cf9-209">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-209">All items contained in the list.</span></span>
| <span data-ttu-id="d8cf9-210">订阅</span><span class="sxs-lookup"><span data-stu-id="d8cf9-210">subscriptions</span></span>      | <span data-ttu-id="d8cf9-211">[订阅][]集合</span><span class="sxs-lookup"><span data-stu-id="d8cf9-211">[subscription][] collection</span></span> | <span data-ttu-id="d8cf9-212">列表上的一组订阅。</span><span class="sxs-lookup"><span data-stu-id="d8cf9-212">The set of subscriptions on the list.</span></span>

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
