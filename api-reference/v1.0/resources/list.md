---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: List
localization_priority: Priority
ms.openlocfilehash: 121b65dcf67e847f507c24385f89324224b41a85
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827291"
---
# <a name="list-resource"></a><span data-ttu-id="994e9-102">List 资源</span><span class="sxs-lookup"><span data-stu-id="994e9-102">List resource</span></span>

<span data-ttu-id="994e9-103">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="994e9-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="994e9-104">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="994e9-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="994e9-105">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="994e9-105">Tasks on a list</span></span>

<span data-ttu-id="994e9-106">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="994e9-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="994e9-107">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="994e9-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="994e9-108">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="994e9-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="994e9-109">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/v1.0/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="994e9-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="994e9-110">常见任务</span><span class="sxs-lookup"><span data-stu-id="994e9-110">Common task</span></span>               | <span data-ttu-id="994e9-111">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="994e9-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="994e9-112">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="994e9-112">[Get list][]</span></span>              | <span data-ttu-id="994e9-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="994e9-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="994e9-114">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="994e9-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="994e9-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="994e9-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="994e9-116">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="994e9-116">[Update list item][]</span></span>      | <span data-ttu-id="994e9-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="994e9-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="994e9-118">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="994e9-118">[Delete list item][]</span></span>      | <span data-ttu-id="994e9-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="994e9-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="994e9-120">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="994e9-120">[Create list item][]</span></span>      | <span data-ttu-id="994e9-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="994e9-121">POST /lists/{list-id}</span></span>

[获取列表]: ../api/list-get.md
[Get list]: ../api/list-get.md
[枚举列表项]: ../api/listitem-list.md
[Enumerate list items]: ../api/listitem-list.md
[更新列表项]: ../api/listitem-update.md
[Update list item]: ../api/listitem-update.md
[删除列表项]: ../api/listitem-delete.md
[Delete list item]: ../api/listitem-delete.md
[创建列表项]: ../api/listitem-create.md
[Create list item]: ../api/listitem-create.md

## <a name="json-representation"></a><span data-ttu-id="994e9-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="994e9-127">JSON representation</span></span>

<span data-ttu-id="994e9-128">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="994e9-128">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="994e9-129">属性</span><span class="sxs-lookup"><span data-stu-id="994e9-129">Properties</span></span>

<span data-ttu-id="994e9-130">\*\*list \*\*资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="994e9-130">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="994e9-131">属性名称</span><span class="sxs-lookup"><span data-stu-id="994e9-131">Property name</span></span>    | <span data-ttu-id="994e9-132">类型</span><span class="sxs-lookup"><span data-stu-id="994e9-132">Type</span></span>                             | <span data-ttu-id="994e9-133">Description</span><span class="sxs-lookup"><span data-stu-id="994e9-133">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="994e9-134">**displayName**</span><span class="sxs-lookup"><span data-stu-id="994e9-134">**displayName**</span></span>  | <span data-ttu-id="994e9-135">string</span><span class="sxs-lookup"><span data-stu-id="994e9-135">string</span></span>                           | <span data-ttu-id="994e9-136">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="994e9-136">The displayable title of the list.</span></span>
| <span data-ttu-id="994e9-137">**list**</span><span class="sxs-lookup"><span data-stu-id="994e9-137">**list**</span></span>         | <span data-ttu-id="994e9-138">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="994e9-138">[listInfo][]</span></span>                     | <span data-ttu-id="994e9-139">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="994e9-139">Provides additional details about the list.</span></span>
| <span data-ttu-id="994e9-140">**system**</span><span class="sxs-lookup"><span data-stu-id="994e9-140">**system**</span></span>       | <span data-ttu-id="994e9-141">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="994e9-141">[systemFacet][]</span></span>                  | <span data-ttu-id="994e9-142">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="994e9-142">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="994e9-143">只读。</span><span class="sxs-lookup"><span data-stu-id="994e9-143">Read-only.</span></span>

<span data-ttu-id="994e9-144">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="994e9-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="994e9-145">属性名称</span><span class="sxs-lookup"><span data-stu-id="994e9-145">Property name</span></span>            | <span data-ttu-id="994e9-146">类型</span><span class="sxs-lookup"><span data-stu-id="994e9-146">Type</span></span>              | <span data-ttu-id="994e9-147">说明</span><span class="sxs-lookup"><span data-stu-id="994e9-147">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="994e9-148">**id**</span><span class="sxs-lookup"><span data-stu-id="994e9-148">**id**</span></span>                   | <span data-ttu-id="994e9-149">string</span><span class="sxs-lookup"><span data-stu-id="994e9-149">string</span></span>            | <span data-ttu-id="994e9-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="994e9-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="994e9-152">**名称**</span><span class="sxs-lookup"><span data-stu-id="994e9-152">**name**</span></span>                 | <span data-ttu-id="994e9-153">string</span><span class="sxs-lookup"><span data-stu-id="994e9-153">string</span></span>            | <span data-ttu-id="994e9-154">项目名称。</span><span class="sxs-lookup"><span data-stu-id="994e9-154">The name of the item.</span></span>
| <span data-ttu-id="994e9-155">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="994e9-155">**createdBy**</span></span>            | <span data-ttu-id="994e9-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="994e9-156">[identitySet][]</span></span>   | <span data-ttu-id="994e9-157">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="994e9-157">Identity of the creator of this item.</span></span> <span data-ttu-id="994e9-158">只读。</span><span class="sxs-lookup"><span data-stu-id="994e9-158">Read-only.</span></span>
| <span data-ttu-id="994e9-159">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="994e9-159">**createdDateTime**</span></span>      | <span data-ttu-id="994e9-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="994e9-160">DateTimeOffset</span></span>    | <span data-ttu-id="994e9-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="994e9-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="994e9-163">**说明**</span><span class="sxs-lookup"><span data-stu-id="994e9-163">**description**</span></span>          | <span data-ttu-id="994e9-164">string</span><span class="sxs-lookup"><span data-stu-id="994e9-164">string</span></span>            | <span data-ttu-id="994e9-165">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="994e9-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="994e9-166">**eTag**</span><span class="sxs-lookup"><span data-stu-id="994e9-166">**eTag**</span></span>                 | <span data-ttu-id="994e9-167">string</span><span class="sxs-lookup"><span data-stu-id="994e9-167">string</span></span>            | <span data-ttu-id="994e9-p107">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="994e9-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="994e9-170">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="994e9-170">**lastModifiedBy**</span></span>       | <span data-ttu-id="994e9-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="994e9-171">[identitySet][]</span></span>   | <span data-ttu-id="994e9-172">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="994e9-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="994e9-173">只读。</span><span class="sxs-lookup"><span data-stu-id="994e9-173">Read-only.</span></span>
| <span data-ttu-id="994e9-174">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="994e9-174">**lastModifiedDateTime**</span></span> | <span data-ttu-id="994e9-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="994e9-175">DateTimeOffset</span></span>    | <span data-ttu-id="994e9-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="994e9-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="994e9-178">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="994e9-178">**parentReference**</span></span>      | <span data-ttu-id="994e9-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="994e9-179">[itemReference][]</span></span> | <span data-ttu-id="994e9-p110">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="994e9-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="994e9-182">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="994e9-182">**sharepointIds**</span></span>        | <span data-ttu-id="994e9-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="994e9-183">[sharepointIds][]</span></span> | <span data-ttu-id="994e9-p111">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="994e9-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="994e9-186">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="994e9-186">**webUrl**</span></span>               | <span data-ttu-id="994e9-187">string (url)</span><span class="sxs-lookup"><span data-stu-id="994e9-187">string (url)</span></span>      | <span data-ttu-id="994e9-p112">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="994e9-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="994e9-190">关系</span><span class="sxs-lookup"><span data-stu-id="994e9-190">Relationships</span></span>

<span data-ttu-id="994e9-191">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="994e9-191">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="994e9-192">关系名称</span><span class="sxs-lookup"><span data-stu-id="994e9-192">Relationship name</span></span> | <span data-ttu-id="994e9-193">类型</span><span class="sxs-lookup"><span data-stu-id="994e9-193">Type</span></span>                             | <span data-ttu-id="994e9-194">说明</span><span class="sxs-lookup"><span data-stu-id="994e9-194">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="994e9-195">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="994e9-195">**drive**</span></span>         | <span data-ttu-id="994e9-196">[drive][]</span><span class="sxs-lookup"><span data-stu-id="994e9-196">[drive][]</span></span>                        | <span data-ttu-id="994e9-197">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="994e9-197">Only present on document libraries.</span></span> <span data-ttu-id="994e9-198">允许访问作为具有 [driveItems][driveItem] 的 [drive][] 资源的列表。</span><span class="sxs-lookup"><span data-stu-id="994e9-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="994e9-199">**items**</span><span class="sxs-lookup"><span data-stu-id="994e9-199">**items**</span></span>         | <span data-ttu-id="994e9-200">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="994e9-200">Collection([listItem][])</span></span>         | <span data-ttu-id="994e9-201">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="994e9-201">All items contained in the list.</span></span>
| <span data-ttu-id="994e9-202">**columns**</span><span class="sxs-lookup"><span data-stu-id="994e9-202">**columns**</span></span>       | <span data-ttu-id="994e9-203">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="994e9-203">Collection([columnDefinition][])</span></span> | <span data-ttu-id="994e9-204">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="994e9-204">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="994e9-205">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="994e9-205">**contentTypes**</span></span>  | <span data-ttu-id="994e9-206">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="994e9-206">Collection([contentType][])</span></span>      | <span data-ttu-id="994e9-207">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="994e9-207">The collection of content types present in this list.</span></span>

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
