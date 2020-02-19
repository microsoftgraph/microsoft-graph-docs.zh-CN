---
author: JeremyKelley
description: ”列表”资源代表网站中的列表。
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4df869eeba7b66dad0bddef48b7d5686d8899702
ms.sourcegitcommit: f51ba08d604d93f5f6af9ee8979cbf76baa285ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/19/2020
ms.locfileid: "42108460"
---
# <a name="list-resource"></a><span data-ttu-id="454c1-103">List 资源</span><span class="sxs-lookup"><span data-stu-id="454c1-103">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="454c1-104">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="454c1-104">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="454c1-105">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="454c1-105">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="454c1-106">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="454c1-106">Tasks on a list</span></span>

<span data-ttu-id="454c1-107">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="454c1-107">The following tasks are available for list resources.</span></span>
<span data-ttu-id="454c1-108">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="454c1-108">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="454c1-109">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="454c1-109">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="454c1-110">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="454c1-110">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="454c1-111">常见任务</span><span class="sxs-lookup"><span data-stu-id="454c1-111">Common task</span></span>               | <span data-ttu-id="454c1-112">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="454c1-112">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="454c1-113">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="454c1-113">[Get list][]</span></span>              | <span data-ttu-id="454c1-114">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="454c1-114">GET /lists/{list-id}</span></span>
| <span data-ttu-id="454c1-115">[创建列表][]</span><span class="sxs-lookup"><span data-stu-id="454c1-115">[Create list][]</span></span>           | <span data-ttu-id="454c1-116">POST/lists</span><span class="sxs-lookup"><span data-stu-id="454c1-116">POST /lists</span></span>
| <span data-ttu-id="454c1-117">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="454c1-117">[Enumerate list items][]</span></span>  | <span data-ttu-id="454c1-118">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="454c1-118">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="454c1-119">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="454c1-119">[Update list item][]</span></span>      | <span data-ttu-id="454c1-120">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="454c1-120">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="454c1-121">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="454c1-121">[Delete list item][]</span></span>      | <span data-ttu-id="454c1-122">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="454c1-122">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="454c1-123">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="454c1-123">[Create list item][]</span></span>      | <span data-ttu-id="454c1-124">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="454c1-124">POST /lists/{list-id}</span></span>
| <span data-ttu-id="454c1-125">[获取最近的活动][]</span><span class="sxs-lookup"><span data-stu-id="454c1-125">[Get recent activities][]</span></span> | <span data-ttu-id="454c1-126">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="454c1-126">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="454c1-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="454c1-134">JSON representation</span></span>

<span data-ttu-id="454c1-135">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="454c1-135">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="454c1-136">属性</span><span class="sxs-lookup"><span data-stu-id="454c1-136">Properties</span></span>

<span data-ttu-id="454c1-137">\*\*list \*\*资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="454c1-137">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="454c1-138">属性名称</span><span class="sxs-lookup"><span data-stu-id="454c1-138">Property name</span></span>    | <span data-ttu-id="454c1-139">类型</span><span class="sxs-lookup"><span data-stu-id="454c1-139">Type</span></span>                             | <span data-ttu-id="454c1-140">说明</span><span class="sxs-lookup"><span data-stu-id="454c1-140">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="454c1-141">**columns**</span><span class="sxs-lookup"><span data-stu-id="454c1-141">**columns**</span></span>      | <span data-ttu-id="454c1-142">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="454c1-142">Collection([columnDefinition][])</span></span> | <span data-ttu-id="454c1-143">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="454c1-143">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="454c1-144">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="454c1-144">**contentTypes**</span></span> | <span data-ttu-id="454c1-145">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="454c1-145">Collection([contentType][])</span></span>      | <span data-ttu-id="454c1-146">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="454c1-146">The collection of content types present in this list.</span></span>
| <span data-ttu-id="454c1-147">**displayName**</span><span class="sxs-lookup"><span data-stu-id="454c1-147">**displayName**</span></span>  | <span data-ttu-id="454c1-148">string</span><span class="sxs-lookup"><span data-stu-id="454c1-148">string</span></span>                           | <span data-ttu-id="454c1-149">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="454c1-149">The displayable title of the list.</span></span>
| <span data-ttu-id="454c1-150">**list**</span><span class="sxs-lookup"><span data-stu-id="454c1-150">**list**</span></span>         | <span data-ttu-id="454c1-151">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="454c1-151">[listInfo][]</span></span>                     | <span data-ttu-id="454c1-152">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="454c1-152">Provides additional details about the list.</span></span>
| <span data-ttu-id="454c1-153">**system**</span><span class="sxs-lookup"><span data-stu-id="454c1-153">**system**</span></span>       | <span data-ttu-id="454c1-154">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="454c1-154">[systemFacet][]</span></span>                  | <span data-ttu-id="454c1-155">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="454c1-155">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="454c1-156">只读。</span><span class="sxs-lookup"><span data-stu-id="454c1-156">Read-only.</span></span>

<span data-ttu-id="454c1-157">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="454c1-157">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="454c1-158">属性名称</span><span class="sxs-lookup"><span data-stu-id="454c1-158">Property name</span></span>            | <span data-ttu-id="454c1-159">类型</span><span class="sxs-lookup"><span data-stu-id="454c1-159">Type</span></span>             | <span data-ttu-id="454c1-160">说明</span><span class="sxs-lookup"><span data-stu-id="454c1-160">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="454c1-161">**id**</span><span class="sxs-lookup"><span data-stu-id="454c1-161">**id**</span></span>                   | <span data-ttu-id="454c1-162">string</span><span class="sxs-lookup"><span data-stu-id="454c1-162">string</span></span>           | <span data-ttu-id="454c1-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="454c1-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="454c1-165">**名称**</span><span class="sxs-lookup"><span data-stu-id="454c1-165">**name**</span></span>                 | <span data-ttu-id="454c1-166">string</span><span class="sxs-lookup"><span data-stu-id="454c1-166">string</span></span>           | <span data-ttu-id="454c1-167">项目名称。</span><span class="sxs-lookup"><span data-stu-id="454c1-167">The name of the item.</span></span>
| <span data-ttu-id="454c1-168">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="454c1-168">**createdBy**</span></span>            | <span data-ttu-id="454c1-169">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="454c1-169">[identitySet][]</span></span>  | <span data-ttu-id="454c1-170">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="454c1-170">Identity of the creator of this item.</span></span> <span data-ttu-id="454c1-171">只读。</span><span class="sxs-lookup"><span data-stu-id="454c1-171">Read-only.</span></span>
| <span data-ttu-id="454c1-172">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="454c1-172">**createdDateTime**</span></span>      | <span data-ttu-id="454c1-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="454c1-173">DateTimeOffset</span></span>   | <span data-ttu-id="454c1-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="454c1-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="454c1-176">**说明**</span><span class="sxs-lookup"><span data-stu-id="454c1-176">**description**</span></span>          | <span data-ttu-id="454c1-177">string</span><span class="sxs-lookup"><span data-stu-id="454c1-177">string</span></span>           | <span data-ttu-id="454c1-178">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="454c1-178">The descriptive text for the item.</span></span>
| <span data-ttu-id="454c1-179">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="454c1-179">**lastModifiedBy**</span></span>       | <span data-ttu-id="454c1-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="454c1-180">[identitySet][]</span></span>  | <span data-ttu-id="454c1-181">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="454c1-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="454c1-182">只读。</span><span class="sxs-lookup"><span data-stu-id="454c1-182">Read-only.</span></span>
| <span data-ttu-id="454c1-183">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="454c1-183">**lastModifiedDateTime**</span></span> | <span data-ttu-id="454c1-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="454c1-184">DateTimeOffset</span></span>   | <span data-ttu-id="454c1-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="454c1-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="454c1-187">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="454c1-187">**webUrl**</span></span>               | <span data-ttu-id="454c1-188">string (url)</span><span class="sxs-lookup"><span data-stu-id="454c1-188">string (url)</span></span>     | <span data-ttu-id="454c1-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="454c1-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="454c1-191">关系</span><span class="sxs-lookup"><span data-stu-id="454c1-191">Relationships</span></span>

<span data-ttu-id="454c1-192">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="454c1-192">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="454c1-193">关系名称</span><span class="sxs-lookup"><span data-stu-id="454c1-193">Relationship name</span></span> | <span data-ttu-id="454c1-194">类型</span><span class="sxs-lookup"><span data-stu-id="454c1-194">Type</span></span>                        | <span data-ttu-id="454c1-195">说明</span><span class="sxs-lookup"><span data-stu-id="454c1-195">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="454c1-196">**activities**</span><span class="sxs-lookup"><span data-stu-id="454c1-196">**activities**</span></span>    | <span data-ttu-id="454c1-197">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="454c1-197">[itemActivity][] collection</span></span> | <span data-ttu-id="454c1-198">最近发生在此列表内的活动。</span><span class="sxs-lookup"><span data-stu-id="454c1-198">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="454c1-199">**drive**</span><span class="sxs-lookup"><span data-stu-id="454c1-199">**drive**</span></span>         | <span data-ttu-id="454c1-200">[drive][]</span><span class="sxs-lookup"><span data-stu-id="454c1-200">[drive][]</span></span>                   | <span data-ttu-id="454c1-201">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="454c1-201">Only present on document libraries.</span></span> <span data-ttu-id="454c1-202">允许使用 [driveItems][driveItem] 作为 [drive][] 资源访问列表。</span><span class="sxs-lookup"><span data-stu-id="454c1-202">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="454c1-203">**项目**</span><span class="sxs-lookup"><span data-stu-id="454c1-203">**items**</span></span>         | <span data-ttu-id="454c1-204">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="454c1-204">Collection([listItem][])</span></span>    | <span data-ttu-id="454c1-205">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="454c1-205">All items contained in the list.</span></span>

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
