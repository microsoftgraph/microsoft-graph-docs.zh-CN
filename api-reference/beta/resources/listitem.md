---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 435544db272b26e6fe3ac0e09803858eec9d05f6
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480878"
---
# <a name="listitem-resource"></a><span data-ttu-id="44494-102">ListItem 资源</span><span class="sxs-lookup"><span data-stu-id="44494-102">ListItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44494-103">此资源表示 SharePoint **[list][]** 中的项目。</span><span class="sxs-lookup"><span data-stu-id="44494-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="44494-104">该列表中的列值可通过 `fieldValueSet` 字典获得。</span><span class="sxs-lookup"><span data-stu-id="44494-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="44494-105">listItem 上的任务</span><span class="sxs-lookup"><span data-stu-id="44494-105">Tasks on a listItem</span></span>

<span data-ttu-id="44494-106">下列任务可用于 **listItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="44494-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="44494-107">下面的所有示例都与**[list][]** 相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`。</span><span class="sxs-lookup"><span data-stu-id="44494-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="44494-108">常见任务</span><span class="sxs-lookup"><span data-stu-id="44494-108">Common task</span></span>                    | <span data-ttu-id="44494-109">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="44494-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="44494-110">[获取][]</span><span class="sxs-lookup"><span data-stu-id="44494-110">[Get][]</span></span>                        | <span data-ttu-id="44494-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="44494-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="44494-112">[获取列值][Get]</span><span class="sxs-lookup"><span data-stu-id="44494-112">[Get column values][Get]</span></span>       | <span data-ttu-id="44494-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="44494-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="44494-114">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="44494-114">[Get analytics][]</span></span>              | <span data-ttu-id="44494-115">获取/items/{item-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="44494-115">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="44494-116">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="44494-116">[Get activities by interval][]</span></span> | <span data-ttu-id="44494-117">获取/items/{item-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="44494-117">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="44494-118">[创建][]</span><span class="sxs-lookup"><span data-stu-id="44494-118">[Create][]</span></span>                     | <span data-ttu-id="44494-119">POST /items</span><span class="sxs-lookup"><span data-stu-id="44494-119">POST /items</span></span>
| <span data-ttu-id="44494-120">[删除][]</span><span class="sxs-lookup"><span data-stu-id="44494-120">[Delete][]</span></span>                     | <span data-ttu-id="44494-121">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="44494-121">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="44494-122">[更新][]</span><span class="sxs-lookup"><span data-stu-id="44494-122">[Update][]</span></span>                     | <span data-ttu-id="44494-123">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="44494-123">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="44494-124">[更新列值][Update]</span><span class="sxs-lookup"><span data-stu-id="44494-124">[Update column values][Update]</span></span> | <span data-ttu-id="44494-125">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="44494-125">PATCH /items/{item-id}/fields</span></span>

[获取]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[获取分析结果]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[删除]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[更新]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="44494-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44494-132">JSON representation</span></span>

<span data-ttu-id="44494-133">下面是 **listItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44494-133">Here is a JSON representation of a **listItem** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type": "microsoft.graph.listItem"
}-->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "sharepointIds": { "@odata.type": "microsoft.graph.sharepointIds" },

  /* relationships */
  "activities": [{"@odata.type": "microsoft.graph.itemActivity"}],
  "analytics": { "@odata.type": "microsoft.graph.itemAnalytics" },
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "versions": [{"@odata.type": "microsoft.graph.listItemVersion"}],

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference"},
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="44494-134">属性</span><span class="sxs-lookup"><span data-stu-id="44494-134">Properties</span></span>

<span data-ttu-id="44494-135">**listItem** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="44494-135">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="44494-136">属性名称</span><span class="sxs-lookup"><span data-stu-id="44494-136">Property name</span></span> | <span data-ttu-id="44494-137">类型</span><span class="sxs-lookup"><span data-stu-id="44494-137">Type</span></span>                | <span data-ttu-id="44494-138">说明</span><span class="sxs-lookup"><span data-stu-id="44494-138">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="44494-139">contentType</span><span class="sxs-lookup"><span data-stu-id="44494-139">contentType</span></span>   | <span data-ttu-id="44494-140">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="44494-140">[contentTypeInfo][]</span></span> | <span data-ttu-id="44494-141">此列表项的内容类型</span><span class="sxs-lookup"><span data-stu-id="44494-141">The content type of this list item</span></span>

<span data-ttu-id="44494-142">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="44494-142">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="44494-143">属性名称</span><span class="sxs-lookup"><span data-stu-id="44494-143">Property name</span></span>        | <span data-ttu-id="44494-144">类型</span><span class="sxs-lookup"><span data-stu-id="44494-144">Type</span></span>              | <span data-ttu-id="44494-145">说明</span><span class="sxs-lookup"><span data-stu-id="44494-145">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="44494-146">id</span><span class="sxs-lookup"><span data-stu-id="44494-146">id</span></span>                   | <span data-ttu-id="44494-147">string</span><span class="sxs-lookup"><span data-stu-id="44494-147">string</span></span>            | <span data-ttu-id="44494-p103">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="44494-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="44494-150">name</span><span class="sxs-lookup"><span data-stu-id="44494-150">name</span></span>                 | <span data-ttu-id="44494-151">string</span><span class="sxs-lookup"><span data-stu-id="44494-151">string</span></span>            | <span data-ttu-id="44494-152">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="44494-152">The name / title of the item.</span></span>
| <span data-ttu-id="44494-153">createdBy</span><span class="sxs-lookup"><span data-stu-id="44494-153">createdBy</span></span>            | <span data-ttu-id="44494-154">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="44494-154">[identitySet][]</span></span>   | <span data-ttu-id="44494-155">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="44494-155">Identity of the creator of this item.</span></span> <span data-ttu-id="44494-156">只读。</span><span class="sxs-lookup"><span data-stu-id="44494-156">Read-only.</span></span>
| <span data-ttu-id="44494-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="44494-157">createdDateTime</span></span>      | <span data-ttu-id="44494-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44494-158">DateTimeOffset</span></span>    | <span data-ttu-id="44494-p105">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="44494-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="44494-161">说明</span><span class="sxs-lookup"><span data-stu-id="44494-161">description</span></span>          | <span data-ttu-id="44494-162">string</span><span class="sxs-lookup"><span data-stu-id="44494-162">string</span></span>            | <span data-ttu-id="44494-163">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="44494-163">The descriptive text for the item.</span></span>
| <span data-ttu-id="44494-164">eTag</span><span class="sxs-lookup"><span data-stu-id="44494-164">eTag</span></span>                 | <span data-ttu-id="44494-165">string</span><span class="sxs-lookup"><span data-stu-id="44494-165">string</span></span>            | <span data-ttu-id="44494-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="44494-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="44494-168">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="44494-168">lastModifiedBy</span></span>       | <span data-ttu-id="44494-169">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="44494-169">[identitySet][]</span></span>   | <span data-ttu-id="44494-170">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="44494-170">Identity of the last modifier of this item.</span></span> <span data-ttu-id="44494-171">只读。</span><span class="sxs-lookup"><span data-stu-id="44494-171">Read-only.</span></span>
| <span data-ttu-id="44494-172">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="44494-172">lastModifiedDateTime</span></span> | <span data-ttu-id="44494-173">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44494-173">DateTimeOffset</span></span>    | <span data-ttu-id="44494-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="44494-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="44494-176">parentReference</span><span class="sxs-lookup"><span data-stu-id="44494-176">parentReference</span></span>      | <span data-ttu-id="44494-177">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="44494-177">[itemReference][]</span></span> | <span data-ttu-id="44494-p109">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="44494-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="44494-180">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="44494-180">sharepointIds</span></span>        | <span data-ttu-id="44494-181">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="44494-181">[sharepointIds][]</span></span> | <span data-ttu-id="44494-p110">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="44494-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="44494-184">WebUrl</span><span class="sxs-lookup"><span data-stu-id="44494-184">webUrl</span></span>               | <span data-ttu-id="44494-185">string (url)</span><span class="sxs-lookup"><span data-stu-id="44494-185">string (url)</span></span>      | <span data-ttu-id="44494-p111">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="44494-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="44494-188">关系</span><span class="sxs-lookup"><span data-stu-id="44494-188">Relationships</span></span>

 <span data-ttu-id="44494-189">**listItem** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="44494-189">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="44494-190">关系名称</span><span class="sxs-lookup"><span data-stu-id="44494-190">Relationship name</span></span> | <span data-ttu-id="44494-191">类型</span><span class="sxs-lookup"><span data-stu-id="44494-191">Type</span></span>                           | <span data-ttu-id="44494-192">说明</span><span class="sxs-lookup"><span data-stu-id="44494-192">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="44494-193">activities</span><span class="sxs-lookup"><span data-stu-id="44494-193">activities</span></span>        | <span data-ttu-id="44494-194">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="44494-194">[itemActivity][] collection</span></span>    | <span data-ttu-id="44494-195">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="44494-195">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="44494-196">分析</span><span class="sxs-lookup"><span data-stu-id="44494-196">analytics</span></span>         | <span data-ttu-id="44494-197">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="44494-197">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="44494-198">有关此项上发生的视图活动的分析。</span><span class="sxs-lookup"><span data-stu-id="44494-198">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="44494-199">driveItem</span><span class="sxs-lookup"><span data-stu-id="44494-199">driveItem</span></span>         | <span data-ttu-id="44494-200">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="44494-200">[driveItem][]</span></span>                  | <span data-ttu-id="44494-201">对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。</span><span class="sxs-lookup"><span data-stu-id="44494-201">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="44494-202">fields</span><span class="sxs-lookup"><span data-stu-id="44494-202">fields</span></span>            | <span data-ttu-id="44494-203">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="44494-203">[fieldValueSet][]</span></span>              | <span data-ttu-id="44494-204">在此列表项上设置的列的值。</span><span class="sxs-lookup"><span data-stu-id="44494-204">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="44494-205">versions</span><span class="sxs-lookup"><span data-stu-id="44494-205">versions</span></span>          | <span data-ttu-id="44494-206">[listItemVersion][]集合</span><span class="sxs-lookup"><span data-stu-id="44494-206">[listItemVersion][] collection</span></span> | <span data-ttu-id="44494-207">列表项的以前版本的列表。</span><span class="sxs-lookup"><span data-stu-id="44494-207">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  },
  "suppressions": [
    "Error: /api-reference/beta/resources/listitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
