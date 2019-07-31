---
author: JeremyKelley
description: 此资源表示 SharePoint list 中的项目。
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 3c05125257eeec9d7b21a7d1eb03de79bc189ccd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009977"
---
# <a name="listitem-resource"></a><span data-ttu-id="981bc-103">ListItem 资源</span><span class="sxs-lookup"><span data-stu-id="981bc-103">ListItem resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="981bc-104">此资源表示 SharePoint **[list][]** 中的项目。</span><span class="sxs-lookup"><span data-stu-id="981bc-104">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="981bc-105">该列表中的列值可通过 `fieldValueSet` 字典获得。</span><span class="sxs-lookup"><span data-stu-id="981bc-105">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="981bc-106">listItem 上的任务</span><span class="sxs-lookup"><span data-stu-id="981bc-106">Tasks on a listItem</span></span>

<span data-ttu-id="981bc-107">下列任务可用于 **listItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="981bc-107">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="981bc-108">下面的所有示例都与**[list][]** 相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`。</span><span class="sxs-lookup"><span data-stu-id="981bc-108">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="981bc-109">常见任务</span><span class="sxs-lookup"><span data-stu-id="981bc-109">Common task</span></span>                    | <span data-ttu-id="981bc-110">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="981bc-110">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="981bc-111">[获取][]</span><span class="sxs-lookup"><span data-stu-id="981bc-111">[Get][]</span></span>                        | <span data-ttu-id="981bc-112">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="981bc-112">GET /items/{item-id}</span></span>
| <span data-ttu-id="981bc-113">[获取列值][Get]</span><span class="sxs-lookup"><span data-stu-id="981bc-113">[Get column values][Get]</span></span>       | <span data-ttu-id="981bc-114">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="981bc-114">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="981bc-115">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="981bc-115">[Get analytics][]</span></span>              | <span data-ttu-id="981bc-116">获取/items/{item-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="981bc-116">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="981bc-117">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="981bc-117">[Get activities by interval][]</span></span> | <span data-ttu-id="981bc-118">获取/items/{item-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="981bc-118">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="981bc-119">[创建][]</span><span class="sxs-lookup"><span data-stu-id="981bc-119">[Create][]</span></span>                     | <span data-ttu-id="981bc-120">POST /items</span><span class="sxs-lookup"><span data-stu-id="981bc-120">POST /items</span></span>
| <span data-ttu-id="981bc-121">[删除][]</span><span class="sxs-lookup"><span data-stu-id="981bc-121">[Delete][]</span></span>                     | <span data-ttu-id="981bc-122">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="981bc-122">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="981bc-123">[更新][]</span><span class="sxs-lookup"><span data-stu-id="981bc-123">[Update][]</span></span>                     | <span data-ttu-id="981bc-124">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="981bc-124">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="981bc-125">[更新列值][Update]</span><span class="sxs-lookup"><span data-stu-id="981bc-125">[Update column values][Update]</span></span> | <span data-ttu-id="981bc-126">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="981bc-126">PATCH /items/{item-id}/fields</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="981bc-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="981bc-133">JSON representation</span></span>

<span data-ttu-id="981bc-134">下面是 **listItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="981bc-134">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="981bc-135">属性</span><span class="sxs-lookup"><span data-stu-id="981bc-135">Properties</span></span>

<span data-ttu-id="981bc-136">**listItem** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="981bc-136">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="981bc-137">属性名</span><span class="sxs-lookup"><span data-stu-id="981bc-137">Property name</span></span> | <span data-ttu-id="981bc-138">类型</span><span class="sxs-lookup"><span data-stu-id="981bc-138">Type</span></span>                | <span data-ttu-id="981bc-139">说明</span><span class="sxs-lookup"><span data-stu-id="981bc-139">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="981bc-140">contentType</span><span class="sxs-lookup"><span data-stu-id="981bc-140">contentType</span></span>   | <span data-ttu-id="981bc-141">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="981bc-141">[contentTypeInfo][]</span></span> | <span data-ttu-id="981bc-142">此列表项的内容类型</span><span class="sxs-lookup"><span data-stu-id="981bc-142">The content type of this list item</span></span>

<span data-ttu-id="981bc-143">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="981bc-143">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="981bc-144">属性名称</span><span class="sxs-lookup"><span data-stu-id="981bc-144">Property name</span></span>        | <span data-ttu-id="981bc-145">类型</span><span class="sxs-lookup"><span data-stu-id="981bc-145">Type</span></span>              | <span data-ttu-id="981bc-146">说明</span><span class="sxs-lookup"><span data-stu-id="981bc-146">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="981bc-147">id</span><span class="sxs-lookup"><span data-stu-id="981bc-147">id</span></span>                   | <span data-ttu-id="981bc-148">string</span><span class="sxs-lookup"><span data-stu-id="981bc-148">string</span></span>            | <span data-ttu-id="981bc-p103">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="981bc-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="981bc-151">name</span><span class="sxs-lookup"><span data-stu-id="981bc-151">name</span></span>                 | <span data-ttu-id="981bc-152">string</span><span class="sxs-lookup"><span data-stu-id="981bc-152">string</span></span>            | <span data-ttu-id="981bc-153">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="981bc-153">The name / title of the item.</span></span>
| <span data-ttu-id="981bc-154">createdBy</span><span class="sxs-lookup"><span data-stu-id="981bc-154">createdBy</span></span>            | <span data-ttu-id="981bc-155">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="981bc-155">[identitySet][]</span></span>   | <span data-ttu-id="981bc-156">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="981bc-156">Identity of the creator of this item.</span></span> <span data-ttu-id="981bc-157">只读。</span><span class="sxs-lookup"><span data-stu-id="981bc-157">Read-only.</span></span>
| <span data-ttu-id="981bc-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="981bc-158">createdDateTime</span></span>      | <span data-ttu-id="981bc-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="981bc-159">DateTimeOffset</span></span>    | <span data-ttu-id="981bc-p105">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="981bc-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="981bc-162">说明</span><span class="sxs-lookup"><span data-stu-id="981bc-162">description</span></span>          | <span data-ttu-id="981bc-163">string</span><span class="sxs-lookup"><span data-stu-id="981bc-163">string</span></span>            | <span data-ttu-id="981bc-164">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="981bc-164">The descriptive text for the item.</span></span>
| <span data-ttu-id="981bc-165">eTag</span><span class="sxs-lookup"><span data-stu-id="981bc-165">eTag</span></span>                 | <span data-ttu-id="981bc-166">字符串</span><span class="sxs-lookup"><span data-stu-id="981bc-166">string</span></span>            | <span data-ttu-id="981bc-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="981bc-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="981bc-169">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="981bc-169">lastModifiedBy</span></span>       | <span data-ttu-id="981bc-170">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="981bc-170">[identitySet][]</span></span>   | <span data-ttu-id="981bc-171">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="981bc-171">Identity of the last modifier of this item.</span></span> <span data-ttu-id="981bc-172">只读。</span><span class="sxs-lookup"><span data-stu-id="981bc-172">Read-only.</span></span>
| <span data-ttu-id="981bc-173">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="981bc-173">lastModifiedDateTime</span></span> | <span data-ttu-id="981bc-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="981bc-174">DateTimeOffset</span></span>    | <span data-ttu-id="981bc-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="981bc-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="981bc-177">parentReference</span><span class="sxs-lookup"><span data-stu-id="981bc-177">parentReference</span></span>      | <span data-ttu-id="981bc-178">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="981bc-178">[itemReference][]</span></span> | <span data-ttu-id="981bc-p109">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="981bc-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="981bc-181">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="981bc-181">sharepointIds</span></span>        | <span data-ttu-id="981bc-182">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="981bc-182">[sharepointIds][]</span></span> | <span data-ttu-id="981bc-p110">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="981bc-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="981bc-185">webUrl</span><span class="sxs-lookup"><span data-stu-id="981bc-185">webUrl</span></span>               | <span data-ttu-id="981bc-186">string (url)</span><span class="sxs-lookup"><span data-stu-id="981bc-186">string (url)</span></span>      | <span data-ttu-id="981bc-p111">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="981bc-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="981bc-189">关系</span><span class="sxs-lookup"><span data-stu-id="981bc-189">Relationships</span></span>

 <span data-ttu-id="981bc-190">**listItem** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="981bc-190">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="981bc-191">关系名称</span><span class="sxs-lookup"><span data-stu-id="981bc-191">Relationship name</span></span> | <span data-ttu-id="981bc-192">类型</span><span class="sxs-lookup"><span data-stu-id="981bc-192">Type</span></span>                           | <span data-ttu-id="981bc-193">说明</span><span class="sxs-lookup"><span data-stu-id="981bc-193">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="981bc-194">activities</span><span class="sxs-lookup"><span data-stu-id="981bc-194">activities</span></span>        | <span data-ttu-id="981bc-195">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="981bc-195">[itemActivity][] collection</span></span>    | <span data-ttu-id="981bc-196">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="981bc-196">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="981bc-197">分析</span><span class="sxs-lookup"><span data-stu-id="981bc-197">analytics</span></span>         | <span data-ttu-id="981bc-198">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="981bc-198">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="981bc-199">此项目上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="981bc-199">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="981bc-200">driveItem</span><span class="sxs-lookup"><span data-stu-id="981bc-200">driveItem</span></span>         | <span data-ttu-id="981bc-201">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="981bc-201">[driveItem][]</span></span>                  | <span data-ttu-id="981bc-202">对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。</span><span class="sxs-lookup"><span data-stu-id="981bc-202">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="981bc-203">fields</span><span class="sxs-lookup"><span data-stu-id="981bc-203">fields</span></span>            | <span data-ttu-id="981bc-204">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="981bc-204">[fieldValueSet][]</span></span>              | <span data-ttu-id="981bc-205">在此列表项上设置的列的值。</span><span class="sxs-lookup"><span data-stu-id="981bc-205">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="981bc-206">版本</span><span class="sxs-lookup"><span data-stu-id="981bc-206">versions</span></span>          | <span data-ttu-id="981bc-207">[listItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="981bc-207">[listItemVersion][] collection</span></span> | <span data-ttu-id="981bc-208">先前版本的列表项的列表。</span><span class="sxs-lookup"><span data-stu-id="981bc-208">The list of previous versions of the list item.</span></span>

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
  "suppressions": []
}
-->
