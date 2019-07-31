---
author: JeremyKelley
description: list 资源表示 site 中的列表。
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: b79172049278758c77ac620f00c391d52633792b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009991"
---
# <a name="list-resource"></a><span data-ttu-id="a17c7-103">List 资源</span><span class="sxs-lookup"><span data-stu-id="a17c7-103">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a17c7-104">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="a17c7-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="a17c7-105">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="a17c7-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="a17c7-106">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="a17c7-106">Tasks on a list</span></span>

<span data-ttu-id="a17c7-107">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="a17c7-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="a17c7-108">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="a17c7-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="a17c7-109">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="a17c7-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="a17c7-110">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="a17c7-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="a17c7-111">常见任务</span><span class="sxs-lookup"><span data-stu-id="a17c7-111">Common task</span></span>               | <span data-ttu-id="a17c7-112">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="a17c7-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="a17c7-113">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="a17c7-113">[Get list][]</span></span>              | <span data-ttu-id="a17c7-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="a17c7-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="a17c7-115">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="a17c7-115">[Enumerate list items][]</span></span>  | <span data-ttu-id="a17c7-116">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="a17c7-116">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="a17c7-117">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="a17c7-117">[Update list item][]</span></span>      | <span data-ttu-id="a17c7-118">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="a17c7-118">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="a17c7-119">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="a17c7-119">[Delete list item][]</span></span>      | <span data-ttu-id="a17c7-120">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="a17c7-120">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="a17c7-121">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="a17c7-121">[Create list item][]</span></span>      | <span data-ttu-id="a17c7-122">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="a17c7-122">POST /lists/{list-id}</span></span>
| <span data-ttu-id="a17c7-123">[获取最近的活动][]</span><span class="sxs-lookup"><span data-stu-id="a17c7-123">[Get recent activities][]</span></span> | <span data-ttu-id="a17c7-124">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="a17c7-124">GET /lists/{list-id}/activities</span></span>

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
[获取最近的活动]: ../api/activities-list.md
[Get recent activities]: ../api/activities-list.md

## <a name="json-representation"></a><span data-ttu-id="a17c7-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a17c7-131">JSON representation</span></span>

<span data-ttu-id="a17c7-132">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a17c7-132">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a17c7-133">属性</span><span class="sxs-lookup"><span data-stu-id="a17c7-133">Properties</span></span>

<span data-ttu-id="a17c7-134">\*\*list \*\*资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="a17c7-134">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="a17c7-135">属性名称</span><span class="sxs-lookup"><span data-stu-id="a17c7-135">Property name</span></span>    | <span data-ttu-id="a17c7-136">类型</span><span class="sxs-lookup"><span data-stu-id="a17c7-136">Type</span></span>                             | <span data-ttu-id="a17c7-137">说明</span><span class="sxs-lookup"><span data-stu-id="a17c7-137">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="a17c7-138">**columns**</span><span class="sxs-lookup"><span data-stu-id="a17c7-138">**columns**</span></span>      | <span data-ttu-id="a17c7-139">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="a17c7-139">Collection([columnDefinition][])</span></span> | <span data-ttu-id="a17c7-140">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="a17c7-140">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="a17c7-141">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="a17c7-141">**contentTypes**</span></span> | <span data-ttu-id="a17c7-142">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="a17c7-142">Collection([contentType][])</span></span>      | <span data-ttu-id="a17c7-143">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="a17c7-143">The collection of content types present in this list.</span></span>
| <span data-ttu-id="a17c7-144">**displayName**</span><span class="sxs-lookup"><span data-stu-id="a17c7-144">**displayName**</span></span>  | <span data-ttu-id="a17c7-145">string</span><span class="sxs-lookup"><span data-stu-id="a17c7-145">string</span></span>                           | <span data-ttu-id="a17c7-146">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="a17c7-146">The displayable title of the list.</span></span>
| <span data-ttu-id="a17c7-147">**list**</span><span class="sxs-lookup"><span data-stu-id="a17c7-147">**list**</span></span>         | <span data-ttu-id="a17c7-148">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="a17c7-148">[listInfo][]</span></span>                     | <span data-ttu-id="a17c7-149">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="a17c7-149">Provides additional details about the list.</span></span>
| <span data-ttu-id="a17c7-150">**system**</span><span class="sxs-lookup"><span data-stu-id="a17c7-150">**system**</span></span>       | <span data-ttu-id="a17c7-151">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="a17c7-151">[systemFacet][]</span></span>                  | <span data-ttu-id="a17c7-152">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="a17c7-152">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="a17c7-153">只读。</span><span class="sxs-lookup"><span data-stu-id="a17c7-153">Read-only.</span></span>

<span data-ttu-id="a17c7-154">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="a17c7-154">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="a17c7-155">属性名</span><span class="sxs-lookup"><span data-stu-id="a17c7-155">Property name</span></span>            | <span data-ttu-id="a17c7-156">类型</span><span class="sxs-lookup"><span data-stu-id="a17c7-156">Type</span></span>             | <span data-ttu-id="a17c7-157">说明</span><span class="sxs-lookup"><span data-stu-id="a17c7-157">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="a17c7-158">**id**</span><span class="sxs-lookup"><span data-stu-id="a17c7-158">**id**</span></span>                   | <span data-ttu-id="a17c7-159">string</span><span class="sxs-lookup"><span data-stu-id="a17c7-159">string</span></span>           | <span data-ttu-id="a17c7-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="a17c7-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="a17c7-162">**名称**</span><span class="sxs-lookup"><span data-stu-id="a17c7-162">**name**</span></span>                 | <span data-ttu-id="a17c7-163">string</span><span class="sxs-lookup"><span data-stu-id="a17c7-163">string</span></span>           | <span data-ttu-id="a17c7-164">项目名称。</span><span class="sxs-lookup"><span data-stu-id="a17c7-164">The name of the item.</span></span>
| <span data-ttu-id="a17c7-165">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="a17c7-165">**createdBy**</span></span>            | <span data-ttu-id="a17c7-166">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a17c7-166">[identitySet][]</span></span>  | <span data-ttu-id="a17c7-167">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="a17c7-167">Identity of the creator of this item.</span></span> <span data-ttu-id="a17c7-168">只读。</span><span class="sxs-lookup"><span data-stu-id="a17c7-168">Read-only.</span></span>
| <span data-ttu-id="a17c7-169">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="a17c7-169">**createdDateTime**</span></span>      | <span data-ttu-id="a17c7-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a17c7-170">DateTimeOffset</span></span>   | <span data-ttu-id="a17c7-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="a17c7-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="a17c7-173">**说明**</span><span class="sxs-lookup"><span data-stu-id="a17c7-173">**description**</span></span>          | <span data-ttu-id="a17c7-174">string</span><span class="sxs-lookup"><span data-stu-id="a17c7-174">string</span></span>           | <span data-ttu-id="a17c7-175">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="a17c7-175">The descriptive text for the item.</span></span>
| <span data-ttu-id="a17c7-176">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="a17c7-176">**lastModifiedBy**</span></span>       | <span data-ttu-id="a17c7-177">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="a17c7-177">[identitySet][]</span></span>  | <span data-ttu-id="a17c7-178">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="a17c7-178">Identity of the last modifier of this item.</span></span> <span data-ttu-id="a17c7-179">只读。</span><span class="sxs-lookup"><span data-stu-id="a17c7-179">Read-only.</span></span>
| <span data-ttu-id="a17c7-180">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="a17c7-180">**lastModifiedDateTime**</span></span> | <span data-ttu-id="a17c7-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a17c7-181">DateTimeOffset</span></span>   | <span data-ttu-id="a17c7-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="a17c7-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="a17c7-184">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="a17c7-184">**webUrl**</span></span>               | <span data-ttu-id="a17c7-185">string (url)</span><span class="sxs-lookup"><span data-stu-id="a17c7-185">string (url)</span></span>     | <span data-ttu-id="a17c7-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="a17c7-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="a17c7-188">关系</span><span class="sxs-lookup"><span data-stu-id="a17c7-188">Relationships</span></span>

<span data-ttu-id="a17c7-189">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="a17c7-189">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="a17c7-190">关系名称</span><span class="sxs-lookup"><span data-stu-id="a17c7-190">Relationship name</span></span> | <span data-ttu-id="a17c7-191">类型</span><span class="sxs-lookup"><span data-stu-id="a17c7-191">Type</span></span>                        | <span data-ttu-id="a17c7-192">说明</span><span class="sxs-lookup"><span data-stu-id="a17c7-192">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="a17c7-193">**activities**</span><span class="sxs-lookup"><span data-stu-id="a17c7-193">**activities**</span></span>    | <span data-ttu-id="a17c7-194">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="a17c7-194">[itemActivity][] collection</span></span> | <span data-ttu-id="a17c7-195">最近发生在此列表内的活动。</span><span class="sxs-lookup"><span data-stu-id="a17c7-195">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="a17c7-196">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="a17c7-196">**drive**</span></span>         | <span data-ttu-id="a17c7-197">[drive][]</span><span class="sxs-lookup"><span data-stu-id="a17c7-197">[drive][]</span></span>                   | <span data-ttu-id="a17c7-198">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="a17c7-198">Only present on document libraries.</span></span> <span data-ttu-id="a17c7-199">允许访问作为具有 [driveItems][driveItem] 的 [drive][] 资源的列表。</span><span class="sxs-lookup"><span data-stu-id="a17c7-199">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="a17c7-200">**items**</span><span class="sxs-lookup"><span data-stu-id="a17c7-200">**items**</span></span>         | <span data-ttu-id="a17c7-201">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="a17c7-201">Collection([listItem][])</span></span>    | <span data-ttu-id="a17c7-202">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="a17c7-202">All items contained in the list.</span></span>

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
