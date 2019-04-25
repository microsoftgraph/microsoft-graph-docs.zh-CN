---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: List
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: aafae9e9214f98ade129d46b63f0e7f930ac4a9c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581531"
---
# <a name="list-resource"></a><span data-ttu-id="340e6-102">List 资源</span><span class="sxs-lookup"><span data-stu-id="340e6-102">List resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="340e6-103">**list** 资源表示 [site][] 中的列表。</span><span class="sxs-lookup"><span data-stu-id="340e6-103">The **list** resource represents a list in a [site][].</span></span>
<span data-ttu-id="340e6-104">此资源包含列表的顶级属性，其中包括模板和字段定义。</span><span class="sxs-lookup"><span data-stu-id="340e6-104">This resource contains the top level properties of the list, including template and field definitions.</span></span>

## <a name="tasks-on-a-list"></a><span data-ttu-id="340e6-105">list 上的任务</span><span class="sxs-lookup"><span data-stu-id="340e6-105">Tasks on a list</span></span>

<span data-ttu-id="340e6-106">下面列出了可执行的 list 资源任务。</span><span class="sxs-lookup"><span data-stu-id="340e6-106">The following tasks are available for list resources.</span></span>
<span data-ttu-id="340e6-107">**注意：** 此测试版只允许导航列表，不允许创建或更新列表。</span><span class="sxs-lookup"><span data-stu-id="340e6-107">**Note:** This beta only allows navigating lists, not creating or updating them.</span></span>
<span data-ttu-id="340e6-108">但是，可以创建或更新[列表项][listItem]。</span><span class="sxs-lookup"><span data-stu-id="340e6-108">You can, however, create or update [list items][listItem].</span></span>

<span data-ttu-id="340e6-109">下面的所有示例都与网站相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}`。</span><span class="sxs-lookup"><span data-stu-id="340e6-109">All examples below are relative to a site, eg: `https://graph.microsoft.com/beta/sites/{site-id}`.</span></span>

| <span data-ttu-id="340e6-110">常见任务</span><span class="sxs-lookup"><span data-stu-id="340e6-110">Common task</span></span>               | <span data-ttu-id="340e6-111">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="340e6-111">HTTP method</span></span>
|:--------------------------|:------------------------------
| <span data-ttu-id="340e6-112">[获取列表][]</span><span class="sxs-lookup"><span data-stu-id="340e6-112">[Get list][]</span></span>              | <span data-ttu-id="340e6-113">GET /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="340e6-113">GET /lists/{list-id}</span></span>
| <span data-ttu-id="340e6-114">[枚举列表项][]</span><span class="sxs-lookup"><span data-stu-id="340e6-114">[Enumerate list items][]</span></span>  | <span data-ttu-id="340e6-115">GET /lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="340e6-115">GET /lists/{list-id}/items</span></span>
| <span data-ttu-id="340e6-116">[更新列表项][]</span><span class="sxs-lookup"><span data-stu-id="340e6-116">[Update list item][]</span></span>      | <span data-ttu-id="340e6-117">PATCH /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="340e6-117">PATCH /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="340e6-118">[删除列表项][]</span><span class="sxs-lookup"><span data-stu-id="340e6-118">[Delete list item][]</span></span>      | <span data-ttu-id="340e6-119">DELETE /lists/{list-id}/items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="340e6-119">DELETE /lists/{list-id}/items/{item-id}</span></span>
| <span data-ttu-id="340e6-120">[创建列表项][]</span><span class="sxs-lookup"><span data-stu-id="340e6-120">[Create list item][]</span></span>      | <span data-ttu-id="340e6-121">POST /lists/{list-id}</span><span class="sxs-lookup"><span data-stu-id="340e6-121">POST /lists/{list-id}</span></span>
| <span data-ttu-id="340e6-122">[获取最近的活动][]</span><span class="sxs-lookup"><span data-stu-id="340e6-122">[Get recent activities][]</span></span> | <span data-ttu-id="340e6-123">GET /lists/{list-id}/activities</span><span class="sxs-lookup"><span data-stu-id="340e6-123">GET /lists/{list-id}/activities</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="340e6-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="340e6-130">JSON representation</span></span>

<span data-ttu-id="340e6-131">下面是 **list** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="340e6-131">Here is a JSON representation of a **list** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="340e6-132">属性</span><span class="sxs-lookup"><span data-stu-id="340e6-132">Properties</span></span>

<span data-ttu-id="340e6-133">\*\*list \*\*资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="340e6-133">The **list** resource has the following properties.</span></span>

| <span data-ttu-id="340e6-134">属性名称</span><span class="sxs-lookup"><span data-stu-id="340e6-134">Property name</span></span>    | <span data-ttu-id="340e6-135">类型</span><span class="sxs-lookup"><span data-stu-id="340e6-135">Type</span></span>                             | <span data-ttu-id="340e6-136">说明</span><span class="sxs-lookup"><span data-stu-id="340e6-136">Description</span></span>
|:-----------------|:---------------------------------|:---------------------------
| <span data-ttu-id="340e6-137">**columns**</span><span class="sxs-lookup"><span data-stu-id="340e6-137">**columns**</span></span>      | <span data-ttu-id="340e6-138">Collection([columnDefinition][])</span><span class="sxs-lookup"><span data-stu-id="340e6-138">Collection([columnDefinition][])</span></span> | <span data-ttu-id="340e6-139">此列表的字段定义集合。</span><span class="sxs-lookup"><span data-stu-id="340e6-139">The collection of field definitions for this list.</span></span>
| <span data-ttu-id="340e6-140">**contentTypes**</span><span class="sxs-lookup"><span data-stu-id="340e6-140">**contentTypes**</span></span> | <span data-ttu-id="340e6-141">Collection([contentType][])</span><span class="sxs-lookup"><span data-stu-id="340e6-141">Collection([contentType][])</span></span>      | <span data-ttu-id="340e6-142">此列表中出现的内容类型的集合。</span><span class="sxs-lookup"><span data-stu-id="340e6-142">The collection of content types present in this list.</span></span>
| <span data-ttu-id="340e6-143">**displayName**</span><span class="sxs-lookup"><span data-stu-id="340e6-143">**displayName**</span></span>  | <span data-ttu-id="340e6-144">string</span><span class="sxs-lookup"><span data-stu-id="340e6-144">string</span></span>                           | <span data-ttu-id="340e6-145">列表的可显示标题。</span><span class="sxs-lookup"><span data-stu-id="340e6-145">The displayable title of the list.</span></span>
| <span data-ttu-id="340e6-146">**list**</span><span class="sxs-lookup"><span data-stu-id="340e6-146">**list**</span></span>         | <span data-ttu-id="340e6-147">[listInfo][]</span><span class="sxs-lookup"><span data-stu-id="340e6-147">[listInfo][]</span></span>                     | <span data-ttu-id="340e6-148">提供关于列表的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="340e6-148">Provides additional details about the list.</span></span>
| <span data-ttu-id="340e6-149">**system**</span><span class="sxs-lookup"><span data-stu-id="340e6-149">**system**</span></span>       | <span data-ttu-id="340e6-150">[systemFacet][]</span><span class="sxs-lookup"><span data-stu-id="340e6-150">[systemFacet][]</span></span>                  | <span data-ttu-id="340e6-151">如果存在，则表示这是系统管理的列表。</span><span class="sxs-lookup"><span data-stu-id="340e6-151">If present, indicates that this is a system-managed list.</span></span> <span data-ttu-id="340e6-152">只读。</span><span class="sxs-lookup"><span data-stu-id="340e6-152">Read-only.</span></span>

<span data-ttu-id="340e6-153">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="340e6-153">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="340e6-154">属性名称</span><span class="sxs-lookup"><span data-stu-id="340e6-154">Property name</span></span>            | <span data-ttu-id="340e6-155">类型</span><span class="sxs-lookup"><span data-stu-id="340e6-155">Type</span></span>             | <span data-ttu-id="340e6-156">说明</span><span class="sxs-lookup"><span data-stu-id="340e6-156">Description</span></span>
|:-------------------------|:-----------------|:-------------------------------
| <span data-ttu-id="340e6-157">**id**</span><span class="sxs-lookup"><span data-stu-id="340e6-157">**id**</span></span>                   | <span data-ttu-id="340e6-158">string</span><span class="sxs-lookup"><span data-stu-id="340e6-158">string</span></span>           | <span data-ttu-id="340e6-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="340e6-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="340e6-161">**名称**</span><span class="sxs-lookup"><span data-stu-id="340e6-161">**name**</span></span>                 | <span data-ttu-id="340e6-162">string</span><span class="sxs-lookup"><span data-stu-id="340e6-162">string</span></span>           | <span data-ttu-id="340e6-163">项目名称。</span><span class="sxs-lookup"><span data-stu-id="340e6-163">The name of the item.</span></span>
| <span data-ttu-id="340e6-164">**createdBy**</span><span class="sxs-lookup"><span data-stu-id="340e6-164">**createdBy**</span></span>            | <span data-ttu-id="340e6-165">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="340e6-165">[identitySet][]</span></span>  | <span data-ttu-id="340e6-166">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="340e6-166">Identity of the creator of this item.</span></span> <span data-ttu-id="340e6-167">只读。</span><span class="sxs-lookup"><span data-stu-id="340e6-167">Read-only.</span></span>
| <span data-ttu-id="340e6-168">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="340e6-168">**createdDateTime**</span></span>      | <span data-ttu-id="340e6-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="340e6-169">DateTimeOffset</span></span>   | <span data-ttu-id="340e6-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="340e6-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="340e6-172">**说明**</span><span class="sxs-lookup"><span data-stu-id="340e6-172">**description**</span></span>          | <span data-ttu-id="340e6-173">string</span><span class="sxs-lookup"><span data-stu-id="340e6-173">string</span></span>           | <span data-ttu-id="340e6-174">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="340e6-174">The descriptive text for the item.</span></span>
| <span data-ttu-id="340e6-175">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="340e6-175">**lastModifiedBy**</span></span>       | <span data-ttu-id="340e6-176">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="340e6-176">[identitySet][]</span></span>  | <span data-ttu-id="340e6-177">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="340e6-177">Identity of the last modifier of this item.</span></span> <span data-ttu-id="340e6-178">只读。</span><span class="sxs-lookup"><span data-stu-id="340e6-178">Read-only.</span></span>
| <span data-ttu-id="340e6-179">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="340e6-179">**lastModifiedDateTime**</span></span> | <span data-ttu-id="340e6-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="340e6-180">DateTimeOffset</span></span>   | <span data-ttu-id="340e6-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="340e6-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="340e6-183">**webUrl**</span><span class="sxs-lookup"><span data-stu-id="340e6-183">**webUrl**</span></span>               | <span data-ttu-id="340e6-184">string (url)</span><span class="sxs-lookup"><span data-stu-id="340e6-184">string (url)</span></span>     | <span data-ttu-id="340e6-p109">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="340e6-p109">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="340e6-187">关系</span><span class="sxs-lookup"><span data-stu-id="340e6-187">Relationships</span></span>

<span data-ttu-id="340e6-188">**list** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="340e6-188">The **list** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="340e6-189">关系名称</span><span class="sxs-lookup"><span data-stu-id="340e6-189">Relationship name</span></span> | <span data-ttu-id="340e6-190">类型</span><span class="sxs-lookup"><span data-stu-id="340e6-190">Type</span></span>                        | <span data-ttu-id="340e6-191">说明</span><span class="sxs-lookup"><span data-stu-id="340e6-191">Description</span></span>
|:------------------|:----------------------------|:------------------------------
| <span data-ttu-id="340e6-192">**activities**</span><span class="sxs-lookup"><span data-stu-id="340e6-192">**activities**</span></span>    | <span data-ttu-id="340e6-193">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="340e6-193">[itemActivity][] collection</span></span> | <span data-ttu-id="340e6-194">最近发生在此列表内的活动。</span><span class="sxs-lookup"><span data-stu-id="340e6-194">The recent activities that took place within this list.</span></span>
| <span data-ttu-id="340e6-195">**驱动器**</span><span class="sxs-lookup"><span data-stu-id="340e6-195">**drive**</span></span>         | <span data-ttu-id="340e6-196">[drive][]</span><span class="sxs-lookup"><span data-stu-id="340e6-196">[drive][]</span></span>                   | <span data-ttu-id="340e6-197">仅存在于文档库中。</span><span class="sxs-lookup"><span data-stu-id="340e6-197">Only present on document libraries.</span></span> <span data-ttu-id="340e6-198">允许访问作为具有 [driveItems][driveItem] 的 [drive][] 资源的列表。</span><span class="sxs-lookup"><span data-stu-id="340e6-198">Allows access to the list as a [drive][] resource with [driveItems][driveItem].</span></span>
| <span data-ttu-id="340e6-199">**items**</span><span class="sxs-lookup"><span data-stu-id="340e6-199">**items**</span></span>         | <span data-ttu-id="340e6-200">Collection([listItem][])</span><span class="sxs-lookup"><span data-stu-id="340e6-200">Collection([listItem][])</span></span>    | <span data-ttu-id="340e6-201">列表中包含的所有项。</span><span class="sxs-lookup"><span data-stu-id="340e6-201">All items contained in the list.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
