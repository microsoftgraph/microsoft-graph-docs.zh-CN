---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: List
ms.openlocfilehash: ba0c01ce1887a32bd8b671cf511104e9128b5efb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="list-resource"></a><span data-ttu-id="d2329-102">List 资源</span><span class="sxs-lookup"><span data-stu-id="d2329-102">List resource</span></span>

<span data-ttu-id="d2329-103">**list** 资源表示[网站][]中的一个列表。</span><span class="sxs-lookup"><span data-stu-id="d2329-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="d2329-104">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="d2329-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="d2329-105">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="d2329-105">Tasks on a list</span></span>

<span data-ttu-id="d2329-106">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="d2329-106">The following tasks are available for {type} resources.</span></span>
<span data-ttu-id="d2329-107">**注意：**此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="d2329-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="d2329-108">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="d2329-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="d2329-109">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="d2329-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="d2329-110">常见任务</span><span class="sxs-lookup"><span data-stu-id="d2329-110">Common task</span></span>               | <span data-ttu-id="d2329-111">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="d2329-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="d2329-112">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="d2329-112">[Get list][]</span></span>              | <span data-ttu-id="d2329-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="d2329-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="d2329-114">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="d2329-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="d2329-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="d2329-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="d2329-116">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="d2329-116">[Update List Item][]</span></span>      | <span data-ttu-id="d2329-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="d2329-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="d2329-118">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="d2329-118">[Delete list item][]</span></span>      | <span data-ttu-id="d2329-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="d2329-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="d2329-120">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="d2329-120">[Create List Item][]</span></span>      | <span data-ttu-id="d2329-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="d2329-121">POST /lists/{list-id}</span></span>

[获取列表]: ../api/list_get.md
[枚举列表项]: ../api/listitem_list.md
[更新列表项]: ../api/listItem_update.md
[删除列表项]: ../api/listItem_delete.md
[创建列表项]: ../api/listItem_create.md

## <a name="json-representation"></a><span data-ttu-id="d2329-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2329-127">JSON representation</span></span>

<span data-ttu-id="d2329-128">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2329-128">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.list",
       "keyProperty": "id", 
       "optionalProperties": [ "items", "drive"] } -->

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
    "template": "documentLibrary | genericList | survey | links | announcements | contacts ..."
  },
  "system": false,

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

## <a name="properties"></a><span data-ttu-id="d2329-129">属性</span><span class="sxs-lookup"><span data-stu-id="d2329-129">Properties</span></span>

<span data-ttu-id="d2329-130">**list** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="d2329-130">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="d2329-131">属性名称</span><span class="sxs-lookup"><span data-stu-id="d2329-131">Property name</span></span>    | <span data-ttu-id="d2329-132">类型</span><span class="sxs-lookup"><span data-stu-id="d2329-132">Type</span></span>                             | <span data-ttu-id="d2329-133">说明</span><span class="sxs-lookup"><span data-stu-id="d2329-133">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="d2329-134">**columns**</span><span class="sxs-lookup"><span data-stu-id="d2329-134">**columns**</span></span>      | <span data-ttu-id="d2329-135">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="d2329-135">Collection([columnDefinition][])</span></span> | <span data-ttu-id="d2329-136">此列表的字段定义的集合。</span><span class="sxs-lookup"><span data-stu-id="d2329-136">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="d2329-137">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="d2329-137"><ContentTypes></span></span> | <span data-ttu-id="d2329-138">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="d2329-138">Collection([contentType][])</span></span>      | <span data-ttu-id="d2329-139">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="d2329-139">The collection of content types present in this list.</span></span>
| <span data-ttu-id="d2329-140">**displayName**</span><span class="sxs-lookup"><span data-stu-id="d2329-140">**displayName**</span></span>  | <span data-ttu-id="d2329-141">string</span><span class="sxs-lookup"><span data-stu-id="d2329-141">string</span></span>                           | <span data-ttu-id="d2329-142">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="d2329-142">The new title of the list.</span></span>
| <span data-ttu-id="d2329-143">**list**</span><span class="sxs-lookup"><span data-stu-id="d2329-143">**list**</span></span>         | <span data-ttu-id="d2329-144">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="d2329-144">[listInfo][]</span></span>                     | <span data-ttu-id="d2329-145">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="d2329-145">Provides additional details about the list.</span></span>
| <span data-ttu-id="d2329-146">**system**</span><span class="sxs-lookup"><span data-stu-id="d2329-146">**System**</span></span>       | <span data-ttu-id="d2329-147">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="d2329-147">[systemFacet][]</span></span>                  | <span data-ttu-id="d2329-148">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="d2329-148">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="d2329-149">只读。</span><span class="sxs-lookup"><span data-stu-id="d2329-149">Read-only.</span></span>

<span data-ttu-id="d2329-150">以下属性继承自 ** [baseItem][]**。</span><span class="sxs-lookup"><span data-stu-id="d2329-150">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="d2329-151">属性名称</span><span class="sxs-lookup"><span data-stu-id="d2329-151">Property name</span></span>            | <span data-ttu-id="d2329-152">类型</span><span class="sxs-lookup"><span data-stu-id="d2329-152">Type</span></span>             | <span data-ttu-id="d2329-153">说明</span><span class="sxs-lookup"><span data-stu-id="d2329-153">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="d2329-154">**id**</span><span class="sxs-lookup"><span data-stu-id="d2329-154">**id**</span></span>                   | <span data-ttu-id="d2329-155">string</span><span class="sxs-lookup"><span data-stu-id="d2329-155">string</span></span>           | <span data-ttu-id="d2329-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="d2329-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="d2329-158">**名称**</span><span class="sxs-lookup"><span data-stu-id="d2329-158">**name**</span></span>                 | <span data-ttu-id="d2329-159">string</span><span class="sxs-lookup"><span data-stu-id="d2329-159">string</span></span>           | <span data-ttu-id="d2329-160">项目名称。</span><span class="sxs-lookup"><span data-stu-id="d2329-160">The name of the item.</span></span>
| <span data-ttu-id="d2329-161">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="d2329-161">**createdBy**</span></span>            | <span data-ttu-id="d2329-162">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d2329-162">[identitySet][]</span></span>  | <span data-ttu-id="d2329-163">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="d2329-163">Identity of the creator of this item.</span></span> <span data-ttu-id="d2329-164">只读。</span><span class="sxs-lookup"><span data-stu-id="d2329-164">Read-only.</span></span>
| <span data-ttu-id="d2329-165">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="d2329-165">**createdDateTime**</span></span>      | <span data-ttu-id="d2329-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2329-166">DateTimeOffset</span></span>   | <span data-ttu-id="d2329-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="d2329-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="d2329-169">**说明**</span><span class="sxs-lookup"><span data-stu-id="d2329-169">**description**</span></span>          | <span data-ttu-id="d2329-170">string</span><span class="sxs-lookup"><span data-stu-id="d2329-170">string</span></span>           | <span data-ttu-id="d2329-171">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="d2329-171">The descriptive text for the site.</span></span>
| <span data-ttu-id="d2329-172">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="d2329-172">**lastModifiedBy**</span></span>       | <span data-ttu-id="d2329-173">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="d2329-173">[identitySet][]</span></span>  | <span data-ttu-id="d2329-174">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="d2329-174">Identity of the last modifier of this item.</span></span> <span data-ttu-id="d2329-175">只读。</span><span class="sxs-lookup"><span data-stu-id="d2329-175">Read-only.</span></span>
| <span data-ttu-id="d2329-176">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="d2329-176">**lastModifiedDateTime**</span></span> | <span data-ttu-id="d2329-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2329-177">DateTimeOffset</span></span>   | <span data-ttu-id="d2329-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="d2329-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="d2329-180">**WebUrl**</span><span class="sxs-lookup"><span data-stu-id="d2329-180">**webUrl**</span></span>               | <span data-ttu-id="d2329-181">string (url)</span><span class="sxs-lookup"><span data-stu-id="d2329-181">string (url)</span></span>     | <span data-ttu-id="d2329-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="d2329-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="d2329-184">关系</span><span class="sxs-lookup"><span data-stu-id="d2329-184">Relationships</span></span>

<span data-ttu-id="d2329-185">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="d2329-185">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="d2329-186">关系名称</span><span class="sxs-lookup"><span data-stu-id="d2329-186">Relationship name</span></span> | <span data-ttu-id="d2329-187">类型</span><span class="sxs-lookup"><span data-stu-id="d2329-187">Type</span></span>                        | <span data-ttu-id="d2329-188">说明</span><span class="sxs-lookup"><span data-stu-id="d2329-188">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="d2329-189">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="d2329-189">**drive**</span></span>         | <span data-ttu-id="d2329-190">[drive][]</span><span class="sxs-lookup"><span data-stu-id="d2329-190">[drive][]</span></span>                   | <span data-ttu-id="d2329-191">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="d2329-191">Only present on document libraries.</span></span> <span data-ttu-id="d2329-192">允许访问作为具有 [driveItems][driveItem] 的 [drive][] 资源的列表。</span><span class="sxs-lookup"><span data-stu-id="d2329-192">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="d2329-193">**items**</span><span class="sxs-lookup"><span data-stu-id="d2329-193">**items**</span></span>         | <span data-ttu-id="d2329-194">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="d2329-194">Collection([listItem][])</span></span>    | <span data-ttu-id="d2329-195">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="d2329-195">All items contained in the drive.</span></span>

[baseItem]: baseItem.md
[contentType]: contentType.md
[drive]: drive.md
[driveItem]: driveItem.md
[columnDefinition]: columnDefinition.md
[identitySet]: identitySet.md
[listInfo]: listInfo.md
[listItem]: listItem.md
[site]: site.md
[systemFacet]: systemFacet.md

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
