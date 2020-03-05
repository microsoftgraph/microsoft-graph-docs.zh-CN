---
author: JeremyKelley
ms.author: JeremyKelley
title: listItem 资源
description: 表示 SharePoint 列表中的项目。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 96c61daea047f969f88352429a46fc7efb8b776d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447561"
---
# <a name="listitem-resource"></a><span data-ttu-id="ffb8e-103">listItem 资源</span><span class="sxs-lookup"><span data-stu-id="ffb8e-103">listItem resource</span></span>

<span data-ttu-id="ffb8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ffb8e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ffb8e-105">表示 SharePoint **[列表][]** 中的项目。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-105">Represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="ffb8e-106">该列表中的列值可通过 `fieldValueSet` 字典获得。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-106">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="ffb8e-107">方法</span><span class="sxs-lookup"><span data-stu-id="ffb8e-107">Methods</span></span>

<span data-ttu-id="ffb8e-108">下列方法可用于 **listItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-108">The following methods are available for **listItem** resources.</span></span>
<span data-ttu-id="ffb8e-109">所有示例都与 **[list][]** 相关：`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-109">All examples are relative to a **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="ffb8e-110">方法</span><span class="sxs-lookup"><span data-stu-id="ffb8e-110">Method</span></span>                    | <span data-ttu-id="ffb8e-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="ffb8e-111">Return Type</span></span> | <span data-ttu-id="ffb8e-112">说明</span><span class="sxs-lookup"><span data-stu-id="ffb8e-112">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="ffb8e-113">[获取][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-113">[Get][]</span></span>                   | <span data-ttu-id="ffb8e-114">listItem</span><span class="sxs-lookup"><span data-stu-id="ffb8e-114">listItem</span></span>| <span data-ttu-id="ffb8e-115">获取列表中的项。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-115">Get an item in a list.</span></span>
| <span data-ttu-id="ffb8e-116">[获取列值][Get]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-116">[Get column values][Get]</span></span>       | <span data-ttu-id="ffb8e-117">listItem</span><span class="sxs-lookup"><span data-stu-id="ffb8e-117">listItem</span></span> | <span data-ttu-id="ffb8e-118">从 listItem 获取列的值。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-118">Get column values from listItem.</span></span>
| <span data-ttu-id="ffb8e-119">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-119">[Get analytics][]</span></span>              | <span data-ttu-id="ffb8e-120">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-120">[itemAnalytics][]</span></span>| <span data-ttu-id="ffb8e-121">对此资源可获取分析。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-121">Get analytics for this resource.</span></span> 
| <span data-ttu-id="ffb8e-122">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-122">[Get activities by interval][]</span></span> | <span data-ttu-id="ffb8e-123">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-123">[itemActivityStat][]</span></span>| <span data-ttu-id="ffb8e-124">在指定的时间间隔内获取 itemActivityStats 的集合。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-124">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="ffb8e-125">[Create][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-125">[Create][]</span></span>                     | <span data-ttu-id="ffb8e-126">listItem</span><span class="sxs-lookup"><span data-stu-id="ffb8e-126">listItem</span></span> | <span data-ttu-id="ffb8e-127">在列表中创建新的 listItem。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-127">Create a new listItem in a list.</span></span>
| <span data-ttu-id="ffb8e-128">[删除][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-128">[Delete][]</span></span>                     | <span data-ttu-id="ffb8e-129">无内容</span><span class="sxs-lookup"><span data-stu-id="ffb8e-129">No Content</span></span> | <span data-ttu-id="ffb8e-130">从 list 中删除项。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-130">Removes an item from a list.</span></span>
| <span data-ttu-id="ffb8e-131">[Update][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-131">[Update][]</span></span>                     | <span data-ttu-id="ffb8e-132">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-132">[fieldValueSet][]</span></span>| <span data-ttu-id="ffb8e-133">更新 listItem 上的属性。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-133">Update the properties on a listItem.</span></span>
| <span data-ttu-id="ffb8e-134">[更新列值][Update]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-134">[Update column values][Update]</span></span> | <span data-ttu-id="ffb8e-135">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-135">[fieldValueSet][]</span></span>| <span data-ttu-id="ffb8e-136">更新 listItem 上的列值。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-136">Update column values on a listItem.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ffb8e-145">属性</span><span class="sxs-lookup"><span data-stu-id="ffb8e-145">Properties</span></span>

<span data-ttu-id="ffb8e-146">**listItem** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-146">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="ffb8e-147">属性名称</span><span class="sxs-lookup"><span data-stu-id="ffb8e-147">Property name</span></span> | <span data-ttu-id="ffb8e-148">类型</span><span class="sxs-lookup"><span data-stu-id="ffb8e-148">Type</span></span>                | <span data-ttu-id="ffb8e-149">说明</span><span class="sxs-lookup"><span data-stu-id="ffb8e-149">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="ffb8e-150">contentType</span><span class="sxs-lookup"><span data-stu-id="ffb8e-150">contentType</span></span>   | <span data-ttu-id="ffb8e-151">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-151">[contentTypeInfo][]</span></span> | <span data-ttu-id="ffb8e-152">此列表项的内容类型</span><span class="sxs-lookup"><span data-stu-id="ffb8e-152">The content type of this list item</span></span>

<span data-ttu-id="ffb8e-153">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-153">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="ffb8e-154">属性名称</span><span class="sxs-lookup"><span data-stu-id="ffb8e-154">Property name</span></span>        | <span data-ttu-id="ffb8e-155">类型</span><span class="sxs-lookup"><span data-stu-id="ffb8e-155">Type</span></span>              | <span data-ttu-id="ffb8e-156">说明</span><span class="sxs-lookup"><span data-stu-id="ffb8e-156">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="ffb8e-157">id</span><span class="sxs-lookup"><span data-stu-id="ffb8e-157">id</span></span>                   | <span data-ttu-id="ffb8e-158">string</span><span class="sxs-lookup"><span data-stu-id="ffb8e-158">string</span></span>            | <span data-ttu-id="ffb8e-p103">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="ffb8e-161">name</span><span class="sxs-lookup"><span data-stu-id="ffb8e-161">name</span></span>                 | <span data-ttu-id="ffb8e-162">string</span><span class="sxs-lookup"><span data-stu-id="ffb8e-162">string</span></span>            | <span data-ttu-id="ffb8e-163">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-163">The name / title of the item.</span></span>
| <span data-ttu-id="ffb8e-164">createdBy</span><span class="sxs-lookup"><span data-stu-id="ffb8e-164">createdBy</span></span>            | <span data-ttu-id="ffb8e-165">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-165">[identitySet][]</span></span>   | <span data-ttu-id="ffb8e-166">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-166">Identity of the creator of this item.</span></span> <span data-ttu-id="ffb8e-167">只读。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-167">Read-only.</span></span>
| <span data-ttu-id="ffb8e-168">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffb8e-168">createdDateTime</span></span>      | <span data-ttu-id="ffb8e-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffb8e-169">DateTimeOffset</span></span>    | <span data-ttu-id="ffb8e-p105">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="ffb8e-172">说明</span><span class="sxs-lookup"><span data-stu-id="ffb8e-172">description</span></span>          | <span data-ttu-id="ffb8e-173">string</span><span class="sxs-lookup"><span data-stu-id="ffb8e-173">string</span></span>            | <span data-ttu-id="ffb8e-174">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-174">The descriptive text for the item.</span></span>
| <span data-ttu-id="ffb8e-175">eTag</span><span class="sxs-lookup"><span data-stu-id="ffb8e-175">eTag</span></span>                 | <span data-ttu-id="ffb8e-176">字符串</span><span class="sxs-lookup"><span data-stu-id="ffb8e-176">string</span></span>            | <span data-ttu-id="ffb8e-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="ffb8e-179">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ffb8e-179">lastModifiedBy</span></span>       | <span data-ttu-id="ffb8e-180">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-180">[identitySet][]</span></span>   | <span data-ttu-id="ffb8e-181">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-181">Identity of the last modifier of this item.</span></span> <span data-ttu-id="ffb8e-182">只读。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-182">Read-only.</span></span>
| <span data-ttu-id="ffb8e-183">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ffb8e-183">lastModifiedDateTime</span></span> | <span data-ttu-id="ffb8e-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffb8e-184">DateTimeOffset</span></span>    | <span data-ttu-id="ffb8e-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ffb8e-187">parentReference</span><span class="sxs-lookup"><span data-stu-id="ffb8e-187">parentReference</span></span>      | <span data-ttu-id="ffb8e-188">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-188">[itemReference][]</span></span> | <span data-ttu-id="ffb8e-p109">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="ffb8e-191">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ffb8e-191">sharepointIds</span></span>        | <span data-ttu-id="ffb8e-192">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-192">[sharepointIds][]</span></span> | <span data-ttu-id="ffb8e-p110">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="ffb8e-195">webUrl</span><span class="sxs-lookup"><span data-stu-id="ffb8e-195">webUrl</span></span>               | <span data-ttu-id="ffb8e-196">string (url)</span><span class="sxs-lookup"><span data-stu-id="ffb8e-196">string (url)</span></span>      | <span data-ttu-id="ffb8e-p111">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="ffb8e-199">关系</span><span class="sxs-lookup"><span data-stu-id="ffb8e-199">Relationships</span></span>

 <span data-ttu-id="ffb8e-200">**listItem** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-200">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="ffb8e-201">关系名称</span><span class="sxs-lookup"><span data-stu-id="ffb8e-201">Relationship name</span></span> | <span data-ttu-id="ffb8e-202">类型</span><span class="sxs-lookup"><span data-stu-id="ffb8e-202">Type</span></span>                           | <span data-ttu-id="ffb8e-203">说明</span><span class="sxs-lookup"><span data-stu-id="ffb8e-203">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="ffb8e-204">activities</span><span class="sxs-lookup"><span data-stu-id="ffb8e-204">activities</span></span>        | <span data-ttu-id="ffb8e-205">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="ffb8e-205">[itemActivity][] collection</span></span>    | <span data-ttu-id="ffb8e-206">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-206">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="ffb8e-207">分析</span><span class="sxs-lookup"><span data-stu-id="ffb8e-207">analytics</span></span>         | <span data-ttu-id="ffb8e-208">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="ffb8e-208">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="ffb8e-209">此项目上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-209">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="ffb8e-210">driveItem</span><span class="sxs-lookup"><span data-stu-id="ffb8e-210">driveItem</span></span>         | <span data-ttu-id="ffb8e-211">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-211">[driveItem][]</span></span>                  | <span data-ttu-id="ffb8e-212">对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-212">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="ffb8e-213">fields</span><span class="sxs-lookup"><span data-stu-id="ffb8e-213">fields</span></span>            | <span data-ttu-id="ffb8e-214">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="ffb8e-214">[fieldValueSet][]</span></span>              | <span data-ttu-id="ffb8e-215">在此列表项上设置的列的值。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-215">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="ffb8e-216">版本</span><span class="sxs-lookup"><span data-stu-id="ffb8e-216">versions</span></span>          | <span data-ttu-id="ffb8e-217">[listItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="ffb8e-217">[listItemVersion][] collection</span></span> | <span data-ttu-id="ffb8e-218">先前版本的列表项的列表。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-218">The list of previous versions of the list item.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="ffb8e-230">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ffb8e-230">JSON representation</span></span>

<span data-ttu-id="ffb8e-231">下面是 **listItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-231">Here is a JSON representation of a **listItem** resource.</span></span>

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
