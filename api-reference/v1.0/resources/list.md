---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: 列表
localization_priority: Priority
ms.prod: sharepoint
description: ”列表”资源代表网站中的列表。
doc_type: resourcePageType
ms.openlocfilehash: af970267f4aebcac986659324a30238a8510c010
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447582"
---
# <a name="list-resource"></a><span data-ttu-id="269e6-103">List 资源</span><span class="sxs-lookup"><span data-stu-id="269e6-103">List resource</span></span>

<span data-ttu-id="269e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="269e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="269e6-105">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="269e6-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="269e6-106">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="269e6-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="269e6-107">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="269e6-107">Tasks on a list</span></span>

<span data-ttu-id="269e6-108">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="269e6-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="269e6-109">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="269e6-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="269e6-110">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="269e6-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="269e6-111">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/v1.0/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="269e6-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}`.</span></span>

| <span data-ttu-id="269e6-112">常见任务</span><span class="sxs-lookup"><span data-stu-id="269e6-112">Common task</span></span>               | <span data-ttu-id="269e6-113">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="269e6-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="269e6-114">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="269e6-114">[Get list][]</span></span>              | <span data-ttu-id="269e6-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="269e6-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="269e6-116">[创建列表][]</span><span class="sxs-lookup"><span data-stu-id="269e6-116">[Create list][]</span></span>           | <span data-ttu-id="269e6-117">POST /列表</span><span class="sxs-lookup"><span data-stu-id="269e6-117">POST /lists</span></span>
| <span data-ttu-id="269e6-118">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="269e6-118">[Enumerate list items][]</span></span>  | <span data-ttu-id="269e6-119">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="269e6-119">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="269e6-120">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="269e6-120">[Update list item][]</span></span>      | <span data-ttu-id="269e6-121">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="269e6-121">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="269e6-122">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="269e6-122">[Delete list item][]</span></span>      | <span data-ttu-id="269e6-123">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="269e6-123">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="269e6-124">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="269e6-124">[Create list item][]</span></span>      | <span data-ttu-id="269e6-125">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="269e6-125">POST /lists/{list-id}</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="269e6-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="269e6-132">JSON representation</span></span>

<span data-ttu-id="269e6-133">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="269e6-133">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="269e6-134">属性</span><span class="sxs-lookup"><span data-stu-id="269e6-134">Properties</span></span>

<span data-ttu-id="269e6-135">\*\*list \*\*资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="269e6-135">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="269e6-136">属性名称</span><span class="sxs-lookup"><span data-stu-id="269e6-136">Property name</span></span>    | <span data-ttu-id="269e6-137">类型</span><span class="sxs-lookup"><span data-stu-id="269e6-137">Type</span></span>                             | <span data-ttu-id="269e6-138">说明</span><span class="sxs-lookup"><span data-stu-id="269e6-138">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="269e6-139">**displayName**</span><span class="sxs-lookup"><span data-stu-id="269e6-139">**displayName**</span></span>  | <span data-ttu-id="269e6-140">string</span><span class="sxs-lookup"><span data-stu-id="269e6-140">string</span></span>                           | <span data-ttu-id="269e6-141">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="269e6-141">The displayable title of the list.</span></span>
| <span data-ttu-id="269e6-142">**list**</span><span class="sxs-lookup"><span data-stu-id="269e6-142">**list**</span></span>         | <span data-ttu-id="269e6-143">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="269e6-143">[listInfo][]</span></span>                     | <span data-ttu-id="269e6-144">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="269e6-144">Provides additional details about the list.</span></span>
| <span data-ttu-id="269e6-145">**system**</span><span class="sxs-lookup"><span data-stu-id="269e6-145">**system**</span></span>       | <span data-ttu-id="269e6-146">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="269e6-146">[systemFacet][]</span></span>                  | <span data-ttu-id="269e6-147">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="269e6-147">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="269e6-148">只读。</span><span class="sxs-lookup"><span data-stu-id="269e6-148">Read-only.</span></span>

<span data-ttu-id="269e6-149">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="269e6-149">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="269e6-150">属性名称</span><span class="sxs-lookup"><span data-stu-id="269e6-150">Property name</span></span>            | <span data-ttu-id="269e6-151">类型</span><span class="sxs-lookup"><span data-stu-id="269e6-151">Type</span></span>              | <span data-ttu-id="269e6-152">说明</span><span class="sxs-lookup"><span data-stu-id="269e6-152">Description</span></span>
|:-------------------------|:------------------|:------------------------------
| <span data-ttu-id="269e6-153">**id**</span><span class="sxs-lookup"><span data-stu-id="269e6-153">**id**</span></span>                   | <span data-ttu-id="269e6-154">string</span><span class="sxs-lookup"><span data-stu-id="269e6-154">string</span></span>            | <span data-ttu-id="269e6-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="269e6-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="269e6-157">**名称**</span><span class="sxs-lookup"><span data-stu-id="269e6-157">**name**</span></span>                 | <span data-ttu-id="269e6-158">string</span><span class="sxs-lookup"><span data-stu-id="269e6-158">string</span></span>            | <span data-ttu-id="269e6-159">项目名称。</span><span class="sxs-lookup"><span data-stu-id="269e6-159">The name of the item.</span></span>
| <span data-ttu-id="269e6-160">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="269e6-160">**createdBy**</span></span>            | <span data-ttu-id="269e6-161">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="269e6-161">[identitySet][]</span></span>   | <span data-ttu-id="269e6-162">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="269e6-162">Identity of the creator of this item.</span></span> <span data-ttu-id="269e6-163">只读。</span><span class="sxs-lookup"><span data-stu-id="269e6-163">Read-only.</span></span>
| <span data-ttu-id="269e6-164">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="269e6-164">**createdDateTime**</span></span>      | <span data-ttu-id="269e6-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="269e6-165">DateTimeOffset</span></span>    | <span data-ttu-id="269e6-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="269e6-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="269e6-168">**说明**</span><span class="sxs-lookup"><span data-stu-id="269e6-168">**description**</span></span>          | <span data-ttu-id="269e6-169">string</span><span class="sxs-lookup"><span data-stu-id="269e6-169">string</span></span>            | <span data-ttu-id="269e6-170">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="269e6-170">The descriptive text for the item.</span></span>
| <span data-ttu-id="269e6-171">**eTag**</span><span class="sxs-lookup"><span data-stu-id="269e6-171">**eTag**</span></span>                 | <span data-ttu-id="269e6-172">string</span><span class="sxs-lookup"><span data-stu-id="269e6-172">string</span></span>            | <span data-ttu-id="269e6-p107">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="269e6-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="269e6-175">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="269e6-175">**lastModifiedBy**</span></span>       | <span data-ttu-id="269e6-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="269e6-176">[identitySet][]</span></span>   | <span data-ttu-id="269e6-177">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="269e6-177">Identity of the last modifier of this item.</span></span> <span data-ttu-id="269e6-178">只读。</span><span class="sxs-lookup"><span data-stu-id="269e6-178">Read-only.</span></span>
| <span data-ttu-id="269e6-179">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="269e6-179">**lastModifiedDateTime**</span></span> | <span data-ttu-id="269e6-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="269e6-180">DateTimeOffset</span></span>    | <span data-ttu-id="269e6-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="269e6-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="269e6-183">**parentReference**</span><span class="sxs-lookup"><span data-stu-id="269e6-183">**parentReference**</span></span>      | <span data-ttu-id="269e6-184">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="269e6-184">[itemReference][]</span></span> | <span data-ttu-id="269e6-p110">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="269e6-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="269e6-187">**sharepointIds**</span><span class="sxs-lookup"><span data-stu-id="269e6-187">**sharepointIds**</span></span>        | <span data-ttu-id="269e6-188">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="269e6-188">[sharepointIds][]</span></span> | <span data-ttu-id="269e6-p111">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="269e6-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="269e6-191">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="269e6-191">**webUrl**</span></span>               | <span data-ttu-id="269e6-192">string (url)</span><span class="sxs-lookup"><span data-stu-id="269e6-192">string (url)</span></span>      | <span data-ttu-id="269e6-p112">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="269e6-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="269e6-195">关系</span><span class="sxs-lookup"><span data-stu-id="269e6-195">Relationships</span></span>

<span data-ttu-id="269e6-196">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="269e6-196">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="269e6-197">关系名称</span><span class="sxs-lookup"><span data-stu-id="269e6-197">Relationship name</span></span> | <span data-ttu-id="269e6-198">类型</span><span class="sxs-lookup"><span data-stu-id="269e6-198">Type</span></span>                             | <span data-ttu-id="269e6-199">说明</span><span class="sxs-lookup"><span data-stu-id="269e6-199">Description</span></span>
|:------------------|:---------------------------------|:----------------------
| <span data-ttu-id="269e6-200">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="269e6-200">**drive**</span></span>         | <span data-ttu-id="269e6-201">[drive][]</span><span class="sxs-lookup"><span data-stu-id="269e6-201">[drive][]</span></span>                        | <span data-ttu-id="269e6-202">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="269e6-202">Only present on document libraries.</span></span> <span data-ttu-id="269e6-203">允许使用 [driveItems][driveItem] 作为 [drive][] 资源访问列表。</span><span class="sxs-lookup"><span data-stu-id="269e6-203">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="269e6-204">**项目**</span><span class="sxs-lookup"><span data-stu-id="269e6-204">**items**</span></span>         | <span data-ttu-id="269e6-205">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="269e6-205">Collection([listItem][])</span></span>         | <span data-ttu-id="269e6-206">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="269e6-206">All items contained in the list.</span></span>
| <span data-ttu-id="269e6-207">**columns**</span><span class="sxs-lookup"><span data-stu-id="269e6-207">**columns**</span></span>       | <span data-ttu-id="269e6-208">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="269e6-208">Collection([columnDefinition][])</span></span> | <span data-ttu-id="269e6-209">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="269e6-209">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="269e6-210">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="269e6-210">**contentTypes**</span></span>  | <span data-ttu-id="269e6-211">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="269e6-211">Collection([contentType][])</span></span>      | <span data-ttu-id="269e6-212">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="269e6-212">The collection of content types present in this list.</span></span>

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
