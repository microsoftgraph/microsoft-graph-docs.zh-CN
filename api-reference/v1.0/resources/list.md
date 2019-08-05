---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 列表
localization_priority: Priority
ms.prod: sharepoint
description: ”列表”资源代表网站中的列表。
doc_type: resourcePageType
ms.openlocfilehash: 51821bb20188c004af3f2aca868c3cfd953ce19c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036405"
---
# <a name="list-resource"></a><span data-ttu-id="af981-103">List 资源</span><span class="sxs-lookup"><span data-stu-id="af981-103">List resource</span></span>

<span data-ttu-id="af981-104">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="af981-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="af981-105">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="af981-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="af981-106">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="af981-106">Tasks on a list</span></span>

<span data-ttu-id="af981-107">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="af981-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="af981-108">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="af981-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="af981-109">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="af981-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="af981-110">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/v1.0/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="af981-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="af981-111">常见任务</span><span class="sxs-lookup"><span data-stu-id="af981-111">Common task</span></span>               | <span data-ttu-id="af981-112">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="af981-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="af981-113">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="af981-113">[Get list][]</span></span>              | <span data-ttu-id="af981-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="af981-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="af981-115">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="af981-115">[Enumerate list items][]</span></span>  | <span data-ttu-id="af981-116">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="af981-116">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="af981-117">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="af981-117">[Update list item][]</span></span>      | <span data-ttu-id="af981-118">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="af981-118">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="af981-119">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="af981-119">[Delete list item][]</span></span>      | <span data-ttu-id="af981-120">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="af981-120">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="af981-121">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="af981-121">[Create list item][]</span></span>      | <span data-ttu-id="af981-122">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="af981-122">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="af981-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af981-128">JSON representation</span></span>

<span data-ttu-id="af981-129">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af981-129">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="af981-130">属性</span><span class="sxs-lookup"><span data-stu-id="af981-130">Properties</span></span>

<span data-ttu-id="af981-131">\*\*list \*\*资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="af981-131">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="af981-132">属性名称</span><span class="sxs-lookup"><span data-stu-id="af981-132">Property name</span></span>    | <span data-ttu-id="af981-133">类型</span><span class="sxs-lookup"><span data-stu-id="af981-133">Type</span></span>                             | <span data-ttu-id="af981-134">说明</span><span class="sxs-lookup"><span data-stu-id="af981-134">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="af981-135">**displayName**</span><span class="sxs-lookup"><span data-stu-id="af981-135">**displayName**</span></span>  | <span data-ttu-id="af981-136">string</span><span class="sxs-lookup"><span data-stu-id="af981-136">string</span></span>                           | <span data-ttu-id="af981-137">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="af981-137">The displayable title of the list.</span></span>
| <span data-ttu-id="af981-138">**list**</span><span class="sxs-lookup"><span data-stu-id="af981-138">**list**</span></span>         | <span data-ttu-id="af981-139">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="af981-139">[listInfo][]</span></span>                     | <span data-ttu-id="af981-140">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="af981-140">Provides additional details about the list.</span></span>
| <span data-ttu-id="af981-141">**system**</span><span class="sxs-lookup"><span data-stu-id="af981-141">**system**</span></span>       | <span data-ttu-id="af981-142">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="af981-142">[systemFacet][]</span></span>                  | <span data-ttu-id="af981-143">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="af981-143">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="af981-144">只读。</span><span class="sxs-lookup"><span data-stu-id="af981-144">Read-only.</span></span>

<span data-ttu-id="af981-145">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="af981-145">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="af981-146">属性名称</span><span class="sxs-lookup"><span data-stu-id="af981-146">Property name</span></span>            | <span data-ttu-id="af981-147">类型</span><span class="sxs-lookup"><span data-stu-id="af981-147">Type</span></span>              | <span data-ttu-id="af981-148">说明</span><span class="sxs-lookup"><span data-stu-id="af981-148">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="af981-149">**id**</span><span class="sxs-lookup"><span data-stu-id="af981-149">**id**</span></span>                   | <span data-ttu-id="af981-150">string</span><span class="sxs-lookup"><span data-stu-id="af981-150">string</span></span>            | <span data-ttu-id="af981-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="af981-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="af981-153">**名称**</span><span class="sxs-lookup"><span data-stu-id="af981-153">**name**</span></span>                 | <span data-ttu-id="af981-154">string</span><span class="sxs-lookup"><span data-stu-id="af981-154">string</span></span>            | <span data-ttu-id="af981-155">项目名称。</span><span class="sxs-lookup"><span data-stu-id="af981-155">The name of the item.</span></span>
| <span data-ttu-id="af981-156">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="af981-156">**createdBy**</span></span>            | <span data-ttu-id="af981-157">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="af981-157">[identitySet][]</span></span>   | <span data-ttu-id="af981-158">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="af981-158">Identity of the creator of this item.</span></span> <span data-ttu-id="af981-159">只读。</span><span class="sxs-lookup"><span data-stu-id="af981-159">Read-only.</span></span>
| <span data-ttu-id="af981-160">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="af981-160">**createdDateTime**</span></span>      | <span data-ttu-id="af981-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af981-161">DateTimeOffset</span></span>    | <span data-ttu-id="af981-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="af981-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="af981-164">**说明**</span><span class="sxs-lookup"><span data-stu-id="af981-164">**description**</span></span>          | <span data-ttu-id="af981-165">string</span><span class="sxs-lookup"><span data-stu-id="af981-165">string</span></span>            | <span data-ttu-id="af981-166">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="af981-166">The descriptive text for the item.</span></span>
| <span data-ttu-id="af981-167">**eTag**</span><span class="sxs-lookup"><span data-stu-id="af981-167">**eTag**</span></span>                 | <span data-ttu-id="af981-168">string</span><span class="sxs-lookup"><span data-stu-id="af981-168">string</span></span>            | <span data-ttu-id="af981-p107">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="af981-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="af981-171">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="af981-171">**lastModifiedBy**</span></span>       | <span data-ttu-id="af981-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="af981-172">[identitySet][]</span></span>   | <span data-ttu-id="af981-173">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="af981-173">Identity of the last modifier of this item.</span></span> <span data-ttu-id="af981-174">只读。</span><span class="sxs-lookup"><span data-stu-id="af981-174">Read-only.</span></span>
| <span data-ttu-id="af981-175">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="af981-175">**lastModifiedDateTime**</span></span> | <span data-ttu-id="af981-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af981-176">DateTimeOffset</span></span>    | <span data-ttu-id="af981-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="af981-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="af981-179">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="af981-179">**parentReference**</span></span>      | <span data-ttu-id="af981-180">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="af981-180">[itemReference][]</span></span> | <span data-ttu-id="af981-p110">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="af981-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="af981-183">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="af981-183">**sharepointIds**</span></span>        | <span data-ttu-id="af981-184">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="af981-184">[sharepointIds][]</span></span> | <span data-ttu-id="af981-p111">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="af981-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="af981-187">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="af981-187">**webUrl**</span></span>               | <span data-ttu-id="af981-188">string (url)</span><span class="sxs-lookup"><span data-stu-id="af981-188">string (url)</span></span>      | <span data-ttu-id="af981-p112">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="af981-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="af981-191">关系</span><span class="sxs-lookup"><span data-stu-id="af981-191">Relationships</span></span>

<span data-ttu-id="af981-192">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="af981-192">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="af981-193">关系名称</span><span class="sxs-lookup"><span data-stu-id="af981-193">Relationship name</span></span> | <span data-ttu-id="af981-194">类型</span><span class="sxs-lookup"><span data-stu-id="af981-194">Type</span></span>                             | <span data-ttu-id="af981-195">说明</span><span class="sxs-lookup"><span data-stu-id="af981-195">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="af981-196">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="af981-196">**drive**</span></span>         | <span data-ttu-id="af981-197">[drive][]</span><span class="sxs-lookup"><span data-stu-id="af981-197">[drive][]</span></span>                        | <span data-ttu-id="af981-198">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="af981-198">Only present on document libraries.</span></span> <span data-ttu-id="af981-199">允许使用 [driveItems][driveItem] 作为 [drive][] 资源访问列表。</span><span class="sxs-lookup"><span data-stu-id="af981-199">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="af981-200">**项目**</span><span class="sxs-lookup"><span data-stu-id="af981-200">**items**</span></span>         | <span data-ttu-id="af981-201">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="af981-201">Collection([listItem][])</span></span>         | <span data-ttu-id="af981-202">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="af981-202">All items contained in the list.</span></span>
| <span data-ttu-id="af981-203">**columns**</span><span class="sxs-lookup"><span data-stu-id="af981-203">**columns**</span></span>       | <span data-ttu-id="af981-204">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="af981-204">Collection([columnDefinition][])</span></span> | <span data-ttu-id="af981-205">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="af981-205">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="af981-206">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="af981-206">**contentTypes**</span></span>  | <span data-ttu-id="af981-207">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="af981-207">Collection([contentType][])</span></span>      | <span data-ttu-id="af981-208">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="af981-208">The collection of content types present in this list.</span></span>

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
