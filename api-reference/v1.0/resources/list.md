---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 列表
localization_priority: Priority
ms.prod: sharepoint
description: ”列表”资源代表网站中的列表。
doc_type: resourcePageType
ms.openlocfilehash: db6fceb1f7806b5356a4e75f1e4fb6a247bd5b00
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108481"
---
# <a name="list-resource"></a><span data-ttu-id="bbda7-103">List 资源</span><span class="sxs-lookup"><span data-stu-id="bbda7-103">List resource</span></span>

<span data-ttu-id="bbda7-104">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="bbda7-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="bbda7-105">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="bbda7-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="bbda7-106">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="bbda7-106">Tasks on a list</span></span>

<span data-ttu-id="bbda7-107">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="bbda7-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="bbda7-108">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="bbda7-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="bbda7-109">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="bbda7-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="bbda7-110">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/v1.0/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="bbda7-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="bbda7-111">常见任务</span><span class="sxs-lookup"><span data-stu-id="bbda7-111">Common task</span></span>               | <span data-ttu-id="bbda7-112">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="bbda7-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="bbda7-113">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-113">[Get list][]</span></span>              | <span data-ttu-id="bbda7-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="bbda7-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="bbda7-115">[创建列表][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-115">[Create list][]</span></span>           | <span data-ttu-id="bbda7-116">POST /列表</span><span class="sxs-lookup"><span data-stu-id="bbda7-116">POST /lists</span></span>
| <span data-ttu-id="bbda7-117">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-117">[Enumerate list items][]</span></span>  | <span data-ttu-id="bbda7-118">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="bbda7-118">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="bbda7-119">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-119">[Update list item][]</span></span>      | <span data-ttu-id="bbda7-120">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="bbda7-120">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="bbda7-121">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-121">[Delete list item][]</span></span>      | <span data-ttu-id="bbda7-122">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="bbda7-122">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="bbda7-123">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-123">[Create list item][]</span></span>      | <span data-ttu-id="bbda7-124">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="bbda7-124">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="bbda7-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bbda7-131">JSON representation</span></span>

<span data-ttu-id="bbda7-132">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bbda7-132">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="bbda7-133">属性</span><span class="sxs-lookup"><span data-stu-id="bbda7-133">Properties</span></span>

<span data-ttu-id="bbda7-134">\*\*list \*\*资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="bbda7-134">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="bbda7-135">属性名称</span><span class="sxs-lookup"><span data-stu-id="bbda7-135">Property name</span></span>    | <span data-ttu-id="bbda7-136">类型</span><span class="sxs-lookup"><span data-stu-id="bbda7-136">Type</span></span>                             | <span data-ttu-id="bbda7-137">说明</span><span class="sxs-lookup"><span data-stu-id="bbda7-137">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="bbda7-138">**displayName**</span><span class="sxs-lookup"><span data-stu-id="bbda7-138">**displayName**</span></span>  | <span data-ttu-id="bbda7-139">string</span><span class="sxs-lookup"><span data-stu-id="bbda7-139">string</span></span>                           | <span data-ttu-id="bbda7-140">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="bbda7-140">The displayable title of the list.</span></span>
| <span data-ttu-id="bbda7-141">**list**</span><span class="sxs-lookup"><span data-stu-id="bbda7-141">**list**</span></span>         | <span data-ttu-id="bbda7-142">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-142">[listInfo][]</span></span>                     | <span data-ttu-id="bbda7-143">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="bbda7-143">Provides additional details about the list.</span></span>
| <span data-ttu-id="bbda7-144">**system**</span><span class="sxs-lookup"><span data-stu-id="bbda7-144">**system**</span></span>       | <span data-ttu-id="bbda7-145">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-145">[systemFacet][]</span></span>                  | <span data-ttu-id="bbda7-146">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="bbda7-146">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="bbda7-147">只读。</span><span class="sxs-lookup"><span data-stu-id="bbda7-147">Read-only.</span></span>

<span data-ttu-id="bbda7-148">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="bbda7-148">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="bbda7-149">属性名称</span><span class="sxs-lookup"><span data-stu-id="bbda7-149">Property name</span></span>            | <span data-ttu-id="bbda7-150">类型</span><span class="sxs-lookup"><span data-stu-id="bbda7-150">Type</span></span>              | <span data-ttu-id="bbda7-151">说明</span><span class="sxs-lookup"><span data-stu-id="bbda7-151">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="bbda7-152">**id**</span><span class="sxs-lookup"><span data-stu-id="bbda7-152">**id**</span></span>                   | <span data-ttu-id="bbda7-153">string</span><span class="sxs-lookup"><span data-stu-id="bbda7-153">string</span></span>            | <span data-ttu-id="bbda7-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="bbda7-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="bbda7-156">**名称**</span><span class="sxs-lookup"><span data-stu-id="bbda7-156">**name**</span></span>                 | <span data-ttu-id="bbda7-157">string</span><span class="sxs-lookup"><span data-stu-id="bbda7-157">string</span></span>            | <span data-ttu-id="bbda7-158">项目名称。</span><span class="sxs-lookup"><span data-stu-id="bbda7-158">The name of the item.</span></span>
| <span data-ttu-id="bbda7-159">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="bbda7-159">**createdBy**</span></span>            | <span data-ttu-id="bbda7-160">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-160">[identitySet][]</span></span>   | <span data-ttu-id="bbda7-161">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="bbda7-161">Identity of the creator of this item.</span></span> <span data-ttu-id="bbda7-162">只读。</span><span class="sxs-lookup"><span data-stu-id="bbda7-162">Read-only.</span></span>
| <span data-ttu-id="bbda7-163">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="bbda7-163">**createdDateTime**</span></span>      | <span data-ttu-id="bbda7-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbda7-164">DateTimeOffset</span></span>    | <span data-ttu-id="bbda7-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="bbda7-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="bbda7-167">**说明**</span><span class="sxs-lookup"><span data-stu-id="bbda7-167">**description**</span></span>          | <span data-ttu-id="bbda7-168">string</span><span class="sxs-lookup"><span data-stu-id="bbda7-168">string</span></span>            | <span data-ttu-id="bbda7-169">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="bbda7-169">The descriptive text for the item.</span></span>
| <span data-ttu-id="bbda7-170">**eTag**</span><span class="sxs-lookup"><span data-stu-id="bbda7-170">**eTag**</span></span>                 | <span data-ttu-id="bbda7-171">string</span><span class="sxs-lookup"><span data-stu-id="bbda7-171">string</span></span>            | <span data-ttu-id="bbda7-p107">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="bbda7-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="bbda7-174">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="bbda7-174">**lastModifiedBy**</span></span>       | <span data-ttu-id="bbda7-175">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-175">[identitySet][]</span></span>   | <span data-ttu-id="bbda7-176">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="bbda7-176">Identity of the last modifier of this item.</span></span> <span data-ttu-id="bbda7-177">只读。</span><span class="sxs-lookup"><span data-stu-id="bbda7-177">Read-only.</span></span>
| <span data-ttu-id="bbda7-178">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="bbda7-178">**lastModifiedDateTime**</span></span> | <span data-ttu-id="bbda7-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbda7-179">DateTimeOffset</span></span>    | <span data-ttu-id="bbda7-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="bbda7-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="bbda7-182">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="bbda7-182">**parentReference**</span></span>      | <span data-ttu-id="bbda7-183">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-183">[itemReference][]</span></span> | <span data-ttu-id="bbda7-p110">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="bbda7-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="bbda7-186">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="bbda7-186">**sharepointIds**</span></span>        | <span data-ttu-id="bbda7-187">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-187">[sharepointIds][]</span></span> | <span data-ttu-id="bbda7-p111">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="bbda7-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="bbda7-190">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="bbda7-190">**webUrl**</span></span>               | <span data-ttu-id="bbda7-191">string (url)</span><span class="sxs-lookup"><span data-stu-id="bbda7-191">string (url)</span></span>      | <span data-ttu-id="bbda7-p112">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="bbda7-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="bbda7-194">关系</span><span class="sxs-lookup"><span data-stu-id="bbda7-194">Relationships</span></span>

<span data-ttu-id="bbda7-195">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="bbda7-195">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="bbda7-196">关系名称</span><span class="sxs-lookup"><span data-stu-id="bbda7-196">Relationship name</span></span> | <span data-ttu-id="bbda7-197">类型</span><span class="sxs-lookup"><span data-stu-id="bbda7-197">Type</span></span>                             | <span data-ttu-id="bbda7-198">说明</span><span class="sxs-lookup"><span data-stu-id="bbda7-198">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="bbda7-199">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="bbda7-199">**drive**</span></span>         | <span data-ttu-id="bbda7-200">[drive][]</span><span class="sxs-lookup"><span data-stu-id="bbda7-200">[drive][]</span></span>                        | <span data-ttu-id="bbda7-201">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="bbda7-201">Only present on document libraries.</span></span> <span data-ttu-id="bbda7-202">允许使用 [driveItems][driveItem] 作为 [drive][] 资源访问列表。</span><span class="sxs-lookup"><span data-stu-id="bbda7-202">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="bbda7-203">**项目**</span><span class="sxs-lookup"><span data-stu-id="bbda7-203">**items**</span></span>         | <span data-ttu-id="bbda7-204">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="bbda7-204">Collection([listItem][])</span></span>         | <span data-ttu-id="bbda7-205">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="bbda7-205">All items contained in the list.</span></span>
| <span data-ttu-id="bbda7-206">**columns**</span><span class="sxs-lookup"><span data-stu-id="bbda7-206">**columns**</span></span>       | <span data-ttu-id="bbda7-207">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="bbda7-207">Collection([columnDefinition][])</span></span> | <span data-ttu-id="bbda7-208">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="bbda7-208">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="bbda7-209">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="bbda7-209">**contentTypes**</span></span>  | <span data-ttu-id="bbda7-210">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="bbda7-210">Collection([contentType][])</span></span>      | <span data-ttu-id="bbda7-211">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="bbda7-211">The collection of content types present in this list.</span></span>

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
