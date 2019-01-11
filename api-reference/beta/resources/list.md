---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.openlocfilehash: 03121447e0b9d7d091005283ed12ef7d93e68108
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870460"
---
# <a name="list-resource"></a><span data-ttu-id="ef098-102">List 资源</span><span class="sxs-lookup"><span data-stu-id="ef098-102">List resource</span></span>

> <span data-ttu-id="ef098-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ef098-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef098-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ef098-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ef098-105">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="ef098-105">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="ef098-106">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="ef098-106">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="ef098-107">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="ef098-107">Tasks on a list</span></span>

<span data-ttu-id="ef098-108">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="ef098-108">The following tasks are available for list resources.</span></span>
<span data-ttu-id="ef098-109">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="ef098-109">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="ef098-110">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="ef098-110">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="ef098-111">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="ef098-111">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="ef098-112">常见任务</span><span class="sxs-lookup"><span data-stu-id="ef098-112">Common task</span></span>               | <span data-ttu-id="ef098-113">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="ef098-113">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="ef098-114">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="ef098-114">[Get list][]</span></span>              | <span data-ttu-id="ef098-115">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="ef098-115">GET /lists/{list-id}</span></span>
| <span data-ttu-id="ef098-116">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="ef098-116">[Enumerate list items][]</span></span>  | <span data-ttu-id="ef098-117">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="ef098-117">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="ef098-118">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="ef098-118">[Update list item][]</span></span>      | <span data-ttu-id="ef098-119">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ef098-119">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="ef098-120">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="ef098-120">[Delete list item][]</span></span>      | <span data-ttu-id="ef098-121">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ef098-121">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="ef098-122">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="ef098-122">[Create list item][]</span></span>      | <span data-ttu-id="ef098-123">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="ef098-123">POST /lists/{list-id}</span></span>
| <span data-ttu-id="ef098-124">[获取最近的活动][]</span><span class="sxs-lookup"><span data-stu-id="ef098-124">[Get recent activities][]</span></span> | <span data-ttu-id="ef098-125">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="ef098-125">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="ef098-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef098-132">JSON representation</span></span>

<span data-ttu-id="ef098-133">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef098-133">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ef098-134">属性</span><span class="sxs-lookup"><span data-stu-id="ef098-134">Properties</span></span>

<span data-ttu-id="ef098-135">\*\*list \*\*资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="ef098-135">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="ef098-136">属性名称</span><span class="sxs-lookup"><span data-stu-id="ef098-136">Property name</span></span>    | <span data-ttu-id="ef098-137">类型</span><span class="sxs-lookup"><span data-stu-id="ef098-137">Type</span></span>                             | <span data-ttu-id="ef098-138">说明</span><span class="sxs-lookup"><span data-stu-id="ef098-138">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="ef098-139">**columns**</span><span class="sxs-lookup"><span data-stu-id="ef098-139">**columns**</span></span>      | <span data-ttu-id="ef098-140">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="ef098-140">Collection([columnDefinition][])</span></span> | <span data-ttu-id="ef098-141">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="ef098-141">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="ef098-142">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="ef098-142">**contentTypes**</span></span> | <span data-ttu-id="ef098-143">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="ef098-143">Collection([contentType][])</span></span>      | <span data-ttu-id="ef098-144">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="ef098-144">The collection of content types present in this list.</span></span>
| <span data-ttu-id="ef098-145">**displayName**</span><span class="sxs-lookup"><span data-stu-id="ef098-145">**displayName**</span></span>  | <span data-ttu-id="ef098-146">string</span><span class="sxs-lookup"><span data-stu-id="ef098-146">string</span></span>                           | <span data-ttu-id="ef098-147">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="ef098-147">The displayable title of the list.</span></span>
| <span data-ttu-id="ef098-148">**list**</span><span class="sxs-lookup"><span data-stu-id="ef098-148">**list**</span></span>         | <span data-ttu-id="ef098-149">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="ef098-149">[listInfo][]</span></span>                     | <span data-ttu-id="ef098-150">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="ef098-150">Provides additional details about the list.</span></span>
| <span data-ttu-id="ef098-151">**system**</span><span class="sxs-lookup"><span data-stu-id="ef098-151">**system**</span></span>       | <span data-ttu-id="ef098-152">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="ef098-152">[systemFacet][]</span></span>                  | <span data-ttu-id="ef098-153">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="ef098-153">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="ef098-154">只读。</span><span class="sxs-lookup"><span data-stu-id="ef098-154">Read-only.</span></span>

<span data-ttu-id="ef098-155">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="ef098-155">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="ef098-156">属性名称</span><span class="sxs-lookup"><span data-stu-id="ef098-156">Property name</span></span>            | <span data-ttu-id="ef098-157">类型</span><span class="sxs-lookup"><span data-stu-id="ef098-157">Type</span></span>             | <span data-ttu-id="ef098-158">说明</span><span class="sxs-lookup"><span data-stu-id="ef098-158">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="ef098-159">**id**</span><span class="sxs-lookup"><span data-stu-id="ef098-159">**id**</span></span>                   | <span data-ttu-id="ef098-160">string</span><span class="sxs-lookup"><span data-stu-id="ef098-160">string</span></span>           | <span data-ttu-id="ef098-p105">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="ef098-p105">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="ef098-163">**名称**</span><span class="sxs-lookup"><span data-stu-id="ef098-163">**name**</span></span>                 | <span data-ttu-id="ef098-164">string</span><span class="sxs-lookup"><span data-stu-id="ef098-164">string</span></span>           | <span data-ttu-id="ef098-165">项目名称。</span><span class="sxs-lookup"><span data-stu-id="ef098-165">The name of the item.</span></span>
| <span data-ttu-id="ef098-166">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="ef098-166">**createdBy**</span></span>            | <span data-ttu-id="ef098-167">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ef098-167">[identitySet][]</span></span>  | <span data-ttu-id="ef098-168">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="ef098-168">Identity of the creator of this item.</span></span> <span data-ttu-id="ef098-169">只读。</span><span class="sxs-lookup"><span data-stu-id="ef098-169">Read-only.</span></span>
| <span data-ttu-id="ef098-170">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="ef098-170">**createdDateTime**</span></span>      | <span data-ttu-id="ef098-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef098-171">DateTimeOffset</span></span>   | <span data-ttu-id="ef098-p107">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="ef098-p107">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="ef098-174">**说明**</span><span class="sxs-lookup"><span data-stu-id="ef098-174">**description**</span></span>          | <span data-ttu-id="ef098-175">string</span><span class="sxs-lookup"><span data-stu-id="ef098-175">string</span></span>           | <span data-ttu-id="ef098-176">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="ef098-176">The descriptive text for the item.</span></span>
| <span data-ttu-id="ef098-177">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="ef098-177">**lastModifiedBy**</span></span>       | <span data-ttu-id="ef098-178">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ef098-178">[identitySet][]</span></span>  | <span data-ttu-id="ef098-179">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="ef098-179">Identity of the last modifier of this item.</span></span> <span data-ttu-id="ef098-180">只读。</span><span class="sxs-lookup"><span data-stu-id="ef098-180">Read-only.</span></span>
| <span data-ttu-id="ef098-181">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ef098-181">**lastModifiedDateTime**</span></span> | <span data-ttu-id="ef098-182">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef098-182">DateTimeOffset</span></span>   | <span data-ttu-id="ef098-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="ef098-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ef098-185">**WebUrl**</span><span class="sxs-lookup"><span data-stu-id="ef098-185">**webUrl**</span></span>               | <span data-ttu-id="ef098-186">string (url)</span><span class="sxs-lookup"><span data-stu-id="ef098-186">string (url)</span></span>     | <span data-ttu-id="ef098-p110">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="ef098-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="ef098-189">关系</span><span class="sxs-lookup"><span data-stu-id="ef098-189">Relationships</span></span>

<span data-ttu-id="ef098-190">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="ef098-190">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="ef098-191">关系名称</span><span class="sxs-lookup"><span data-stu-id="ef098-191">Relationship name</span></span> | <span data-ttu-id="ef098-192">类型</span><span class="sxs-lookup"><span data-stu-id="ef098-192">Type</span></span>                        | <span data-ttu-id="ef098-193">说明</span><span class="sxs-lookup"><span data-stu-id="ef098-193">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="ef098-194">**activities**</span><span class="sxs-lookup"><span data-stu-id="ef098-194">**activities**</span></span>    | <span data-ttu-id="ef098-195">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="ef098-195">[itemActivity][] collection</span></span> | <span data-ttu-id="ef098-196">最近发生在此列表内的活动。</span><span class="sxs-lookup"><span data-stu-id="ef098-196">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="ef098-197">**drive**</span><span class="sxs-lookup"><span data-stu-id="ef098-197">**drive**</span></span>         | <span data-ttu-id="ef098-198">[drive][]</span><span class="sxs-lookup"><span data-stu-id="ef098-198">[drive][]</span></span>                   | <span data-ttu-id="ef098-199">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="ef098-199">Only present on document libraries.</span></span> <span data-ttu-id="ef098-200">允许访问作为具有 [driveItems][driveItem] 的 [drive][] 资源的列表。</span><span class="sxs-lookup"><span data-stu-id="ef098-200">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="ef098-201">**items**</span><span class="sxs-lookup"><span data-stu-id="ef098-201">**items**</span></span>         | <span data-ttu-id="ef098-202">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="ef098-202">Collection([listItem][])</span></span>    | <span data-ttu-id="ef098-203">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="ef098-203">All items contained in the list.</span></span>

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
