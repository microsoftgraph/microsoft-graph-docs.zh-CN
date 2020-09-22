---
author: JeremyKelley
ms.author: JeremyKelley
title: listItem 资源
description: 表示 SharePoint 列表中的项目。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 276a8f61cc12cb2860bab0025d430f039b96b89a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025212"
---
# <a name="listitem-resource"></a><span data-ttu-id="7c277-103">listItem 资源</span><span class="sxs-lookup"><span data-stu-id="7c277-103">listItem resource</span></span>

<span data-ttu-id="7c277-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c277-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c277-105">表示 SharePoint **[列表][]** 中的项目。</span><span class="sxs-lookup"><span data-stu-id="7c277-105">Represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="7c277-106">该列表中的列值可通过 `fieldValueSet` 字典获得。</span><span class="sxs-lookup"><span data-stu-id="7c277-106">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="7c277-107">方法</span><span class="sxs-lookup"><span data-stu-id="7c277-107">Methods</span></span>

<span data-ttu-id="7c277-108">下列方法可用于 **listItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="7c277-108">The following methods are available for **listItem** resources.</span></span>
<span data-ttu-id="7c277-109">所有示例都与 **[list][]** 相关：`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`。</span><span class="sxs-lookup"><span data-stu-id="7c277-109">All examples are relative to a **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="7c277-110">方法</span><span class="sxs-lookup"><span data-stu-id="7c277-110">Method</span></span>                    | <span data-ttu-id="7c277-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="7c277-111">Return Type</span></span> | <span data-ttu-id="7c277-112">说明</span><span class="sxs-lookup"><span data-stu-id="7c277-112">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="7c277-113">[获取][]</span><span class="sxs-lookup"><span data-stu-id="7c277-113">[Get][]</span></span>                   | <span data-ttu-id="7c277-114">listItem</span><span class="sxs-lookup"><span data-stu-id="7c277-114">listItem</span></span>| <span data-ttu-id="7c277-115">获取列表中的项。</span><span class="sxs-lookup"><span data-stu-id="7c277-115">Get an item in a list.</span></span>
| <span data-ttu-id="7c277-116">[获取列值][Get]</span><span class="sxs-lookup"><span data-stu-id="7c277-116">[Get column values][Get]</span></span>       | <span data-ttu-id="7c277-117">listItem</span><span class="sxs-lookup"><span data-stu-id="7c277-117">listItem</span></span> | <span data-ttu-id="7c277-118">从 listItem 获取列的值。</span><span class="sxs-lookup"><span data-stu-id="7c277-118">Get column values from listItem.</span></span>
| <span data-ttu-id="7c277-119">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="7c277-119">[Get analytics][]</span></span>              | <span data-ttu-id="7c277-120">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="7c277-120">[itemAnalytics][]</span></span>| <span data-ttu-id="7c277-121">对此资源可获取分析。</span><span class="sxs-lookup"><span data-stu-id="7c277-121">Get analytics for this resource.</span></span> 
| <span data-ttu-id="7c277-122">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="7c277-122">[Get activities by interval][]</span></span> | <span data-ttu-id="7c277-123">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="7c277-123">[itemActivityStat][]</span></span>| <span data-ttu-id="7c277-124">在指定的时间间隔内获取 itemActivityStats 的集合。</span><span class="sxs-lookup"><span data-stu-id="7c277-124">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="7c277-125">[Create][]</span><span class="sxs-lookup"><span data-stu-id="7c277-125">[Create][]</span></span>                     | <span data-ttu-id="7c277-126">listItem</span><span class="sxs-lookup"><span data-stu-id="7c277-126">listItem</span></span> | <span data-ttu-id="7c277-127">在列表中创建新的 listItem。</span><span class="sxs-lookup"><span data-stu-id="7c277-127">Create a new listItem in a list.</span></span>
| <span data-ttu-id="7c277-128">[删除][]</span><span class="sxs-lookup"><span data-stu-id="7c277-128">[Delete][]</span></span>                     | <span data-ttu-id="7c277-129">无内容</span><span class="sxs-lookup"><span data-stu-id="7c277-129">No Content</span></span> | <span data-ttu-id="7c277-130">从 list 中删除项。</span><span class="sxs-lookup"><span data-stu-id="7c277-130">Removes an item from a list.</span></span>
| <span data-ttu-id="7c277-131">[Update][]</span><span class="sxs-lookup"><span data-stu-id="7c277-131">[Update][]</span></span>                     | <span data-ttu-id="7c277-132">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="7c277-132">[fieldValueSet][]</span></span>| <span data-ttu-id="7c277-133">更新 listItem 上的属性。</span><span class="sxs-lookup"><span data-stu-id="7c277-133">Update the properties on a listItem.</span></span>
| <span data-ttu-id="7c277-134">[更新列值][Update]</span><span class="sxs-lookup"><span data-stu-id="7c277-134">[Update column values][Update]</span></span> | <span data-ttu-id="7c277-135">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="7c277-135">[fieldValueSet][]</span></span>| <span data-ttu-id="7c277-136">更新 listItem 上的列值。</span><span class="sxs-lookup"><span data-stu-id="7c277-136">Update column values on a listItem.</span></span>

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

## <a name="properties"></a><span data-ttu-id="7c277-145">属性</span><span class="sxs-lookup"><span data-stu-id="7c277-145">Properties</span></span>

<span data-ttu-id="7c277-146">**listItem** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="7c277-146">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="7c277-147">属性名称</span><span class="sxs-lookup"><span data-stu-id="7c277-147">Property name</span></span> | <span data-ttu-id="7c277-148">类型</span><span class="sxs-lookup"><span data-stu-id="7c277-148">Type</span></span>                | <span data-ttu-id="7c277-149">说明</span><span class="sxs-lookup"><span data-stu-id="7c277-149">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="7c277-150">contentType</span><span class="sxs-lookup"><span data-stu-id="7c277-150">contentType</span></span>   | <span data-ttu-id="7c277-151">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="7c277-151">[contentTypeInfo][]</span></span> | <span data-ttu-id="7c277-152">此列表项的内容类型</span><span class="sxs-lookup"><span data-stu-id="7c277-152">The content type of this list item</span></span>

<span data-ttu-id="7c277-153">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="7c277-153">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="7c277-154">属性名称</span><span class="sxs-lookup"><span data-stu-id="7c277-154">Property name</span></span>        | <span data-ttu-id="7c277-155">类型</span><span class="sxs-lookup"><span data-stu-id="7c277-155">Type</span></span>              | <span data-ttu-id="7c277-156">说明</span><span class="sxs-lookup"><span data-stu-id="7c277-156">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="7c277-157">id</span><span class="sxs-lookup"><span data-stu-id="7c277-157">id</span></span>                   | <span data-ttu-id="7c277-158">string</span><span class="sxs-lookup"><span data-stu-id="7c277-158">string</span></span>            | <span data-ttu-id="7c277-p103">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="7c277-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="7c277-161">name</span><span class="sxs-lookup"><span data-stu-id="7c277-161">name</span></span>                 | <span data-ttu-id="7c277-162">string</span><span class="sxs-lookup"><span data-stu-id="7c277-162">string</span></span>            | <span data-ttu-id="7c277-163">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="7c277-163">The name / title of the item.</span></span>
| <span data-ttu-id="7c277-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="7c277-164">createdBy</span></span>            | <span data-ttu-id="7c277-165">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7c277-165">[identitySet][]</span></span>   | <span data-ttu-id="7c277-166">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="7c277-166">Identity of the creator of this item.</span></span> <span data-ttu-id="7c277-167">只读。</span><span class="sxs-lookup"><span data-stu-id="7c277-167">Read-only.</span></span>
| <span data-ttu-id="7c277-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7c277-168">createdDateTime</span></span>      | <span data-ttu-id="7c277-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c277-169">DateTimeOffset</span></span>    | <span data-ttu-id="7c277-p105">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="7c277-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="7c277-172">说明</span><span class="sxs-lookup"><span data-stu-id="7c277-172">description</span></span>          | <span data-ttu-id="7c277-173">string</span><span class="sxs-lookup"><span data-stu-id="7c277-173">string</span></span>            | <span data-ttu-id="7c277-174">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="7c277-174">The descriptive text for the item.</span></span>
| <span data-ttu-id="7c277-175">eTag</span><span class="sxs-lookup"><span data-stu-id="7c277-175">eTag</span></span>                 | <span data-ttu-id="7c277-176">字符串</span><span class="sxs-lookup"><span data-stu-id="7c277-176">string</span></span>            | <span data-ttu-id="7c277-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="7c277-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="7c277-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="7c277-179">lastModifiedBy</span></span>       | <span data-ttu-id="7c277-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="7c277-180">[identitySet][]</span></span>   | <span data-ttu-id="7c277-181">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="7c277-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="7c277-182">只读。</span><span class="sxs-lookup"><span data-stu-id="7c277-182">Read-only.</span></span>
| <span data-ttu-id="7c277-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c277-183">lastModifiedDateTime</span></span> | <span data-ttu-id="7c277-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c277-184">DateTimeOffset</span></span>    | <span data-ttu-id="7c277-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="7c277-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="7c277-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="7c277-187">parentReference</span></span>      | <span data-ttu-id="7c277-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="7c277-188">[itemReference][]</span></span> | <span data-ttu-id="7c277-p109">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="7c277-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="7c277-191">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="7c277-191">sharepointIds</span></span>        | <span data-ttu-id="7c277-192">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="7c277-192">[sharepointIds][]</span></span> | <span data-ttu-id="7c277-p110">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="7c277-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="7c277-195">webUrl</span><span class="sxs-lookup"><span data-stu-id="7c277-195">webUrl</span></span>               | <span data-ttu-id="7c277-196">string (url)</span><span class="sxs-lookup"><span data-stu-id="7c277-196">string (url)</span></span>      | <span data-ttu-id="7c277-p111">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="7c277-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="7c277-199">关系</span><span class="sxs-lookup"><span data-stu-id="7c277-199">Relationships</span></span>

 <span data-ttu-id="7c277-200">**listItem** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="7c277-200">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="7c277-201">关系名称</span><span class="sxs-lookup"><span data-stu-id="7c277-201">Relationship name</span></span> | <span data-ttu-id="7c277-202">类型</span><span class="sxs-lookup"><span data-stu-id="7c277-202">Type</span></span>                           | <span data-ttu-id="7c277-203">说明</span><span class="sxs-lookup"><span data-stu-id="7c277-203">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="7c277-204">activities</span><span class="sxs-lookup"><span data-stu-id="7c277-204">activities</span></span>        | <span data-ttu-id="7c277-205">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="7c277-205">[itemActivity][] collection</span></span>    | <span data-ttu-id="7c277-206">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="7c277-206">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="7c277-207">分析</span><span class="sxs-lookup"><span data-stu-id="7c277-207">analytics</span></span>         | <span data-ttu-id="7c277-208">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="7c277-208">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="7c277-209">此项目上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="7c277-209">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="7c277-210">driveItem</span><span class="sxs-lookup"><span data-stu-id="7c277-210">driveItem</span></span>         | <span data-ttu-id="7c277-211">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="7c277-211">[driveItem][]</span></span>                  | <span data-ttu-id="7c277-212">对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。</span><span class="sxs-lookup"><span data-stu-id="7c277-212">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="7c277-213">fields</span><span class="sxs-lookup"><span data-stu-id="7c277-213">fields</span></span>            | <span data-ttu-id="7c277-214">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="7c277-214">[fieldValueSet][]</span></span>              | <span data-ttu-id="7c277-215">在此列表项上设置的列的值。</span><span class="sxs-lookup"><span data-stu-id="7c277-215">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="7c277-216">版本</span><span class="sxs-lookup"><span data-stu-id="7c277-216">versions</span></span>          | <span data-ttu-id="7c277-217">[listItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="7c277-217">[listItemVersion][] collection</span></span> | <span data-ttu-id="7c277-218">先前版本的列表项的列表。</span><span class="sxs-lookup"><span data-stu-id="7c277-218">The list of previous versions of the list item.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="7c277-230">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c277-230">JSON representation</span></span>

<span data-ttu-id="7c277-231">下面是 **listItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c277-231">Here is a JSON representation of a **listItem** resource.</span></span>

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

