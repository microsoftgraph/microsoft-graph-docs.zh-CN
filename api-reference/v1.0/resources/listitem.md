---
author: JeremyKelley
ms.author: JeremyKelley
title: listItem 资源
description: 表示 SharePoint 列表中的项目。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: e9a9010e8700d7e6ebd6a2e3d030fba7cab79f83
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703761"
---
# <a name="listitem-resource"></a><span data-ttu-id="85f12-103">listItem 资源</span><span class="sxs-lookup"><span data-stu-id="85f12-103">listItem resource</span></span>

<span data-ttu-id="85f12-104">表示 SharePoint **[列表][]** 中的项目。</span><span class="sxs-lookup"><span data-stu-id="85f12-104">Represents an item in a sharepoint list.</span></span>
<span data-ttu-id="85f12-105">该列表中的列值可通过 `fieldValueSet` 字典获得。</span><span class="sxs-lookup"><span data-stu-id="85f12-105">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="85f12-106">方法</span><span class="sxs-lookup"><span data-stu-id="85f12-106">Methods</span></span>

<span data-ttu-id="85f12-107">下列方法可用于 **listItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="85f12-107">The following methods are available for **listItem** resources.</span></span>
<span data-ttu-id="85f12-108">所有示例都与 **[list][]** 相关：`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`。</span><span class="sxs-lookup"><span data-stu-id="85f12-108">All examples are relative to a **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="85f12-109">方法</span><span class="sxs-lookup"><span data-stu-id="85f12-109">Method</span></span>                    | <span data-ttu-id="85f12-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="85f12-110">Return Type</span></span> | <span data-ttu-id="85f12-111">说明</span><span class="sxs-lookup"><span data-stu-id="85f12-111">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="85f12-112">[获取][]</span><span class="sxs-lookup"><span data-stu-id="85f12-112">[Get][]</span></span>                   | <span data-ttu-id="85f12-113">listItem</span><span class="sxs-lookup"><span data-stu-id="85f12-113">listItem</span></span>| <span data-ttu-id="85f12-114">获取列表中的项。</span><span class="sxs-lookup"><span data-stu-id="85f12-114">Get an item in a list.</span></span>
| <span data-ttu-id="85f12-115">[获取列值][Get]</span><span class="sxs-lookup"><span data-stu-id="85f12-115">[Get column values][Get]</span></span>       | <span data-ttu-id="85f12-116">listItem</span><span class="sxs-lookup"><span data-stu-id="85f12-116">listItem</span></span> | <span data-ttu-id="85f12-117">从 listItem 获取列的值。</span><span class="sxs-lookup"><span data-stu-id="85f12-117">Get column values from listItem.</span></span>
| <span data-ttu-id="85f12-118">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="85f12-118">[Get analytics][]</span></span>              | <span data-ttu-id="85f12-119">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="85f12-119">[itemAnalytics][]</span></span>| <span data-ttu-id="85f12-120">对此资源可获取分析。</span><span class="sxs-lookup"><span data-stu-id="85f12-120">Get analytics for this resource.</span></span> 
| <span data-ttu-id="85f12-121">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="85f12-121">[Get activities by interval][]</span></span> | <span data-ttu-id="85f12-122">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="85f12-122">[itemActivityStat][]</span></span>| <span data-ttu-id="85f12-123">在指定的时间间隔内获取 itemActivityStats 的集合。</span><span class="sxs-lookup"><span data-stu-id="85f12-123">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="85f12-124">[Create][]</span><span class="sxs-lookup"><span data-stu-id="85f12-124">[Create][]</span></span>                     | <span data-ttu-id="85f12-125">listItem</span><span class="sxs-lookup"><span data-stu-id="85f12-125">listItem</span></span> | <span data-ttu-id="85f12-126">在列表中创建新的 listItem。</span><span class="sxs-lookup"><span data-stu-id="85f12-126">Create a new listItem in a list.</span></span>
| <span data-ttu-id="85f12-127">[删除][]</span><span class="sxs-lookup"><span data-stu-id="85f12-127">[Delete][]</span></span>                     | <span data-ttu-id="85f12-128">无内容</span><span class="sxs-lookup"><span data-stu-id="85f12-128">No Content</span></span> | <span data-ttu-id="85f12-129">从 list 中删除项。</span><span class="sxs-lookup"><span data-stu-id="85f12-129">Removes an item from a list.</span></span>
| <span data-ttu-id="85f12-130">[Update][]</span><span class="sxs-lookup"><span data-stu-id="85f12-130">[Update][]</span></span>                     | <span data-ttu-id="85f12-131">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="85f12-131">[fieldValueSet][]</span></span>| <span data-ttu-id="85f12-132">更新 listItem 上的属性。</span><span class="sxs-lookup"><span data-stu-id="85f12-132">Update the properties on a listItem.</span></span>
| <span data-ttu-id="85f12-133">[更新列值][Update]</span><span class="sxs-lookup"><span data-stu-id="85f12-133">[Update column values][Update]</span></span> | <span data-ttu-id="85f12-134">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="85f12-134">[fieldValueSet][]</span></span>| <span data-ttu-id="85f12-135">更新 listItem 上的列值。</span><span class="sxs-lookup"><span data-stu-id="85f12-135">Update column values on a listItem.</span></span>

[Get]: ../api/listitem-get.md
[获取分析结果]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivitystat-getactivitybyinterval.md
[Get activities by interval]: ../api/itemactivitystat-getactivitybyinterval.md
[Create]: ../api/listitem-create.md
[删除]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[Update]: ../api/listitem-update.md

[itemActivityStat]: itemactivitystat.md
[fieldValueSet]: fieldvalueset.md

## <a name="properties"></a><span data-ttu-id="85f12-144">属性</span><span class="sxs-lookup"><span data-stu-id="85f12-144">Properties</span></span>

<span data-ttu-id="85f12-145">**listItem** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="85f12-145">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="85f12-146">属性名称</span><span class="sxs-lookup"><span data-stu-id="85f12-146">Property name</span></span> | <span data-ttu-id="85f12-147">类型</span><span class="sxs-lookup"><span data-stu-id="85f12-147">Type</span></span>                | <span data-ttu-id="85f12-148">说明</span><span class="sxs-lookup"><span data-stu-id="85f12-148">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="85f12-149">contentType</span><span class="sxs-lookup"><span data-stu-id="85f12-149">contentType</span></span>   | <span data-ttu-id="85f12-150">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="85f12-150">[contentTypeInfo][]</span></span> | <span data-ttu-id="85f12-151">此列表项的内容类型</span><span class="sxs-lookup"><span data-stu-id="85f12-151">The content type of this list item</span></span>

<span data-ttu-id="85f12-152">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="85f12-152">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="85f12-153">属性名称</span><span class="sxs-lookup"><span data-stu-id="85f12-153">Property name</span></span>        | <span data-ttu-id="85f12-154">类型</span><span class="sxs-lookup"><span data-stu-id="85f12-154">Type</span></span>              | <span data-ttu-id="85f12-155">说明</span><span class="sxs-lookup"><span data-stu-id="85f12-155">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="85f12-156">id</span><span class="sxs-lookup"><span data-stu-id="85f12-156">id</span></span>                   | <span data-ttu-id="85f12-157">string</span><span class="sxs-lookup"><span data-stu-id="85f12-157">string</span></span>            | <span data-ttu-id="85f12-p103">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="85f12-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="85f12-160">name</span><span class="sxs-lookup"><span data-stu-id="85f12-160">name</span></span>                 | <span data-ttu-id="85f12-161">string</span><span class="sxs-lookup"><span data-stu-id="85f12-161">string</span></span>            | <span data-ttu-id="85f12-162">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="85f12-162">The name / title of the item.</span></span>
| <span data-ttu-id="85f12-163">createdBy</span><span class="sxs-lookup"><span data-stu-id="85f12-163">createdBy</span></span>            | <span data-ttu-id="85f12-164">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="85f12-164">[identitySet][]</span></span>   | <span data-ttu-id="85f12-165">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="85f12-165">Identity of the creator of this item.</span></span> <span data-ttu-id="85f12-166">只读。</span><span class="sxs-lookup"><span data-stu-id="85f12-166">Read-only.</span></span>
| <span data-ttu-id="85f12-167">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85f12-167">createdDateTime</span></span>      | <span data-ttu-id="85f12-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85f12-168">DateTimeOffset</span></span>    | <span data-ttu-id="85f12-p105">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="85f12-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="85f12-171">说明</span><span class="sxs-lookup"><span data-stu-id="85f12-171">description</span></span>          | <span data-ttu-id="85f12-172">string</span><span class="sxs-lookup"><span data-stu-id="85f12-172">string</span></span>            | <span data-ttu-id="85f12-173">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="85f12-173">The descriptive text for the item.</span></span>
| <span data-ttu-id="85f12-174">eTag</span><span class="sxs-lookup"><span data-stu-id="85f12-174">eTag</span></span>                 | <span data-ttu-id="85f12-175">字符串</span><span class="sxs-lookup"><span data-stu-id="85f12-175">string</span></span>            | <span data-ttu-id="85f12-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="85f12-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="85f12-178">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="85f12-178">lastModifiedBy</span></span>       | <span data-ttu-id="85f12-179">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="85f12-179">[identitySet][]</span></span>   | <span data-ttu-id="85f12-180">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="85f12-180">Identity of the last modifier of this item.</span></span> <span data-ttu-id="85f12-181">只读。</span><span class="sxs-lookup"><span data-stu-id="85f12-181">Read-only.</span></span>
| <span data-ttu-id="85f12-182">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="85f12-182">lastModifiedDateTime</span></span> | <span data-ttu-id="85f12-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85f12-183">DateTimeOffset</span></span>    | <span data-ttu-id="85f12-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="85f12-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="85f12-186">parentReference</span><span class="sxs-lookup"><span data-stu-id="85f12-186">parentReference</span></span>      | <span data-ttu-id="85f12-187">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="85f12-187">[itemReference][]</span></span> | <span data-ttu-id="85f12-p109">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="85f12-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="85f12-190">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="85f12-190">sharepointIds</span></span>        | <span data-ttu-id="85f12-191">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="85f12-191">[sharepointIds][]</span></span> | <span data-ttu-id="85f12-p110">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="85f12-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="85f12-194">webUrl</span><span class="sxs-lookup"><span data-stu-id="85f12-194">webUrl</span></span>               | <span data-ttu-id="85f12-195">string (url)</span><span class="sxs-lookup"><span data-stu-id="85f12-195">string (url)</span></span>      | <span data-ttu-id="85f12-p111">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="85f12-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="85f12-198">关系</span><span class="sxs-lookup"><span data-stu-id="85f12-198">Relationships</span></span>

 <span data-ttu-id="85f12-199">**listItem** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="85f12-199">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="85f12-200">关系名称</span><span class="sxs-lookup"><span data-stu-id="85f12-200">Relationship name</span></span> | <span data-ttu-id="85f12-201">类型</span><span class="sxs-lookup"><span data-stu-id="85f12-201">Type</span></span>                           | <span data-ttu-id="85f12-202">说明</span><span class="sxs-lookup"><span data-stu-id="85f12-202">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="85f12-203">activities</span><span class="sxs-lookup"><span data-stu-id="85f12-203">activities</span></span>        | <span data-ttu-id="85f12-204">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="85f12-204">[itemActivity][] collection</span></span>    | <span data-ttu-id="85f12-205">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="85f12-205">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="85f12-206">分析</span><span class="sxs-lookup"><span data-stu-id="85f12-206">analytics</span></span>         | <span data-ttu-id="85f12-207">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="85f12-207">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="85f12-208">此项目上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="85f12-208">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="85f12-209">driveItem</span><span class="sxs-lookup"><span data-stu-id="85f12-209">driveItem</span></span>         | <span data-ttu-id="85f12-210">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="85f12-210">[driveItem][]</span></span>                  | <span data-ttu-id="85f12-211">对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。</span><span class="sxs-lookup"><span data-stu-id="85f12-211">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="85f12-212">fields</span><span class="sxs-lookup"><span data-stu-id="85f12-212">fields</span></span>            | <span data-ttu-id="85f12-213">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="85f12-213">[fieldValueSet][]</span></span>              | <span data-ttu-id="85f12-214">在此列表项上设置的列的值。</span><span class="sxs-lookup"><span data-stu-id="85f12-214">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="85f12-215">版本</span><span class="sxs-lookup"><span data-stu-id="85f12-215">versions</span></span>          | <span data-ttu-id="85f12-216">[listItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="85f12-216">[listItemVersion][] collection</span></span> | <span data-ttu-id="85f12-217">先前版本的列表项的列表。</span><span class="sxs-lookup"><span data-stu-id="85f12-217">The list of previous versions of the list item.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="85f12-229">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85f12-229">JSON representation</span></span>

<span data-ttu-id="85f12-230">下面是 **listItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85f12-230">Here is a JSON representation of a **listItem** resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/listItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
