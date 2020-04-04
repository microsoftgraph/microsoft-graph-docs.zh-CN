---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 列表
localization_priority: Priority
ms.prod: sharepoint
description: ”列表”资源代表网站中的列表。
doc_type: resourcePageType
ms.openlocfilehash: a63f4bdbf3ef8290a9295bc0ecb9abdee5452b45
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2020
ms.locfileid: "43108443"
---
# <a name="list-resource"></a><span data-ttu-id="1a0f8-103">List 资源</span><span class="sxs-lookup"><span data-stu-id="1a0f8-103">List resource</span></span>

<span data-ttu-id="1a0f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a0f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a0f8-105">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="1a0f8-106">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="1a0f8-107">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="1a0f8-107">Tasks on a list</span></span>

<span data-ttu-id="1a0f8-108">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="1a0f8-109">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="1a0f8-110">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="1a0f8-111">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/v1.0/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="1a0f8-112">常见任务</span><span class="sxs-lookup"><span data-stu-id="1a0f8-112">Common task</span></span>               | <span data-ttu-id="1a0f8-113">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="1a0f8-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="1a0f8-114">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-114">[Get list][]</span></span>              | <span data-ttu-id="1a0f8-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="1a0f8-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="1a0f8-116">[创建列表][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-116">[Create list][]</span></span>           | <span data-ttu-id="1a0f8-117">POST /列表</span><span class="sxs-lookup"><span data-stu-id="1a0f8-117">POST /lists</span></span>
| <span data-ttu-id="1a0f8-118">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-118">[Enumerate list items][]</span></span>  | <span data-ttu-id="1a0f8-119">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="1a0f8-119">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="1a0f8-120">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-120">[Update list item][]</span></span>      | <span data-ttu-id="1a0f8-121">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="1a0f8-121">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="1a0f8-122">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-122">[Delete list item][]</span></span>      | <span data-ttu-id="1a0f8-123">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="1a0f8-123">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="1a0f8-124">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-124">[Create list item][]</span></span>      | <span data-ttu-id="1a0f8-125">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="1a0f8-125">POST /lists/{list-id}</span></span>
| <span data-ttu-id="1a0f8-126">[获取 WebSocket 频道][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-126">[Get WebSocket channel][]</span></span> | <span data-ttu-id="1a0f8-127">GET /lists/{list-id}/subscriptions/socketIo</span><span class="sxs-lookup"><span data-stu-id="1a0f8-127">GET /lists/{list-id}/subscriptions/socketIo</span></span>

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
[获取 WebSocket 频道]: ../api/subscriptions-socketio.md
[Get WebSocket channel]: ../api/subscriptions-socketio.md

## <a name="json-representation"></a><span data-ttu-id="1a0f8-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a0f8-135">JSON representation</span></span>

<span data-ttu-id="1a0f8-136">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-136">Here is a JSON representation of a **list** resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "items",
    "drive"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.list"
}-->

```json
{
  "columns": [ { "@odata.type": "microsoft.graph.columnDefinition" }],
  "contentTypes": [ { "@odata.type": "microsoft.graph.contentType" }],
  "displayName": "title of list",
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "items": [ { "@odata.type": "microsoft.graph.listItem" } ],
  "list": {
    "@odata.type": "microsoft.graph.listInfo",
    "hidden": false,
    "template": "documentLibrary | genericList | survey | links | announcements | contacts | accessRequest ..."
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
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },
  "webUrl": "url to visit the list in a browser"
}
```

## <a name="properties"></a><span data-ttu-id="1a0f8-137">属性</span><span class="sxs-lookup"><span data-stu-id="1a0f8-137">Properties</span></span>

<span data-ttu-id="1a0f8-138">\*\*list \*\*资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-138">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="1a0f8-139">属性名称</span><span class="sxs-lookup"><span data-stu-id="1a0f8-139">Property name</span></span>    | <span data-ttu-id="1a0f8-140">类型</span><span class="sxs-lookup"><span data-stu-id="1a0f8-140">Type</span></span>                             | <span data-ttu-id="1a0f8-141">说明</span><span class="sxs-lookup"><span data-stu-id="1a0f8-141">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="1a0f8-142">**displayName**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-142">**displayName**</span></span>  | <span data-ttu-id="1a0f8-143">string</span><span class="sxs-lookup"><span data-stu-id="1a0f8-143">string</span></span>                           | <span data-ttu-id="1a0f8-144">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-144">The displayable title of the list.</span></span>
| <span data-ttu-id="1a0f8-145">**list**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-145">**list**</span></span>         | <span data-ttu-id="1a0f8-146">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-146">[listInfo][]</span></span>                     | <span data-ttu-id="1a0f8-147">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-147">Provides additional details about the list.</span></span>
| <span data-ttu-id="1a0f8-148">**system**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-148">**system**</span></span>       | <span data-ttu-id="1a0f8-149">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-149">[systemFacet][]</span></span>                  | <span data-ttu-id="1a0f8-150">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-150">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="1a0f8-151">只读。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-151">Read-only.</span></span>

<span data-ttu-id="1a0f8-152">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-152">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="1a0f8-153">属性名称</span><span class="sxs-lookup"><span data-stu-id="1a0f8-153">Property name</span></span>            | <span data-ttu-id="1a0f8-154">类型</span><span class="sxs-lookup"><span data-stu-id="1a0f8-154">Type</span></span>              | <span data-ttu-id="1a0f8-155">说明</span><span class="sxs-lookup"><span data-stu-id="1a0f8-155">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="1a0f8-156">**id**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-156">**id**</span></span>                   | <span data-ttu-id="1a0f8-157">string</span><span class="sxs-lookup"><span data-stu-id="1a0f8-157">string</span></span>            | <span data-ttu-id="1a0f8-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="1a0f8-160">**名称**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-160">**name**</span></span>                 | <span data-ttu-id="1a0f8-161">string</span><span class="sxs-lookup"><span data-stu-id="1a0f8-161">string</span></span>            | <span data-ttu-id="1a0f8-162">项目名称。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-162">The name of the item.</span></span>
| <span data-ttu-id="1a0f8-163">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-163">**createdBy**</span></span>            | <span data-ttu-id="1a0f8-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-164">[identitySet][]</span></span>   | <span data-ttu-id="1a0f8-165">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-165">Identity of the creator of this item.</span></span> <span data-ttu-id="1a0f8-166">只读。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-166">Read-only.</span></span>
| <span data-ttu-id="1a0f8-167">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-167">**createdDateTime**</span></span>      | <span data-ttu-id="1a0f8-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a0f8-168">DateTimeOffset</span></span>    | <span data-ttu-id="1a0f8-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="1a0f8-171">**说明**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-171">**description**</span></span>          | <span data-ttu-id="1a0f8-172">string</span><span class="sxs-lookup"><span data-stu-id="1a0f8-172">string</span></span>            | <span data-ttu-id="1a0f8-173">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-173">The descriptive text for the item.</span></span>
| <span data-ttu-id="1a0f8-174">**eTag**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-174">**eTag**</span></span>                 | <span data-ttu-id="1a0f8-175">string</span><span class="sxs-lookup"><span data-stu-id="1a0f8-175">string</span></span>            | <span data-ttu-id="1a0f8-p107">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="1a0f8-178">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-178">**lastModifiedBy**</span></span>       | <span data-ttu-id="1a0f8-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-179">[identitySet][]</span></span>   | <span data-ttu-id="1a0f8-180">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="1a0f8-181">只读。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-181">Read-only.</span></span>
| <span data-ttu-id="1a0f8-182">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-182">**lastModifiedDateTime**</span></span> | <span data-ttu-id="1a0f8-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a0f8-183">DateTimeOffset</span></span>    | <span data-ttu-id="1a0f8-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="1a0f8-186">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-186">**parentReference**</span></span>      | <span data-ttu-id="1a0f8-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-187">[itemReference][]</span></span> | <span data-ttu-id="1a0f8-p110">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="1a0f8-190">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-190">**sharepointIds**</span></span>        | <span data-ttu-id="1a0f8-191">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-191">[sharepointIds][]</span></span> | <span data-ttu-id="1a0f8-p111">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="1a0f8-194">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-194">**webUrl**</span></span>               | <span data-ttu-id="1a0f8-195">string (url)</span><span class="sxs-lookup"><span data-stu-id="1a0f8-195">string (url)</span></span>      | <span data-ttu-id="1a0f8-p112">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="1a0f8-198">关系</span><span class="sxs-lookup"><span data-stu-id="1a0f8-198">Relationships</span></span>

<span data-ttu-id="1a0f8-199">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-199">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="1a0f8-200">关系名称</span><span class="sxs-lookup"><span data-stu-id="1a0f8-200">Relationship name</span></span> | <span data-ttu-id="1a0f8-201">类型</span><span class="sxs-lookup"><span data-stu-id="1a0f8-201">Type</span></span>                             | <span data-ttu-id="1a0f8-202">说明</span><span class="sxs-lookup"><span data-stu-id="1a0f8-202">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="1a0f8-203">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-203">**drive**</span></span>         | <span data-ttu-id="1a0f8-204">[drive][]</span><span class="sxs-lookup"><span data-stu-id="1a0f8-204">[drive][]</span></span>                        | <span data-ttu-id="1a0f8-205">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-205">Only present on document libraries.</span></span> <span data-ttu-id="1a0f8-206">允许使用 [driveItems][driveItem] 作为 [drive][] 资源访问列表。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-206">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="1a0f8-207">**项目**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-207">**items**</span></span>         | <span data-ttu-id="1a0f8-208">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="1a0f8-208">Collection([listItem][])</span></span>         | <span data-ttu-id="1a0f8-209">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-209">All items contained in the list.</span></span>
| <span data-ttu-id="1a0f8-210">**columns**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-210">**columns**</span></span>       | <span data-ttu-id="1a0f8-211">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="1a0f8-211">Collection([columnDefinition][])</span></span> | <span data-ttu-id="1a0f8-212">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-212">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="1a0f8-213">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-213">**contentTypes**</span></span>  | <span data-ttu-id="1a0f8-214">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="1a0f8-214">Collection([contentType][])</span></span>      | <span data-ttu-id="1a0f8-215">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-215">The collection of content types present in this list.</span></span>
| <span data-ttu-id="1a0f8-216">**订阅**</span><span class="sxs-lookup"><span data-stu-id="1a0f8-216">**subscriptions**</span></span> | <span data-ttu-id="1a0f8-217">集合（[订阅][]）</span><span class="sxs-lookup"><span data-stu-id="1a0f8-217">Collection([subscription][])</span></span>     | <span data-ttu-id="1a0f8-218">列表上的订阅集。</span><span class="sxs-lookup"><span data-stu-id="1a0f8-218">The set of subscriptions on the list.</span></span>

[baseItem]: baseitem.md
[contentType]: contenttype.md
[drive]: drive.md
[driveItem]: driveitem.md
[columnDefinition]: columndefinition.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
[listInfo]: listinfo.md
[listItem]: listitem.md
[sharepointIds]: sharepointids.md
[site]: site.md
[systemFacet]: systemfacet.md
[订阅]: subscription.md
[subscription]: subscription.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/Lists",
  "tocBookmarks": {
    "Lists": "#"
  }
} -->
