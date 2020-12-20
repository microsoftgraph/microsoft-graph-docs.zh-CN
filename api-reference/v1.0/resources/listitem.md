---
author: JeremyKelley
title: listItem 资源
description: 表示 SharePoint 列表中的项目。
localization_priority: Priority
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 7e9e7b00ee87127b7844d2d7208d63c8e4fb6af5
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714114"
---
# <a name="listitem-resource"></a><span data-ttu-id="8f59e-103">listItem 资源</span><span class="sxs-lookup"><span data-stu-id="8f59e-103">listItem resource</span></span>

<span data-ttu-id="8f59e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f59e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f59e-105">表示 SharePoint [列表][]中的项目。</span><span class="sxs-lookup"><span data-stu-id="8f59e-105">Represents an item in a SharePoint [list][].</span></span>

<span data-ttu-id="8f59e-106">SharePoint 文档库中的所有项目可以表示为 **listItem** 或 [driveItem][] 资源。</span><span class="sxs-lookup"><span data-stu-id="8f59e-106">All items in a SharePoint document library can be represented as a **listItem** or [driveItem][] resource.</span></span>

<span data-ttu-id="8f59e-107">该列表中的列值可通过 `fieldValueSet` 字典获得。</span><span class="sxs-lookup"><span data-stu-id="8f59e-107">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="methods"></a><span data-ttu-id="8f59e-108">方法</span><span class="sxs-lookup"><span data-stu-id="8f59e-108">Methods</span></span>

<span data-ttu-id="8f59e-109">下列方法可用于 **listItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="8f59e-109">The following methods are available for **listItem** resources.</span></span>
<span data-ttu-id="8f59e-110">所有示例都与 **[list][]** 相关：`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`。</span><span class="sxs-lookup"><span data-stu-id="8f59e-110">All examples are relative to a **[list][]**: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="8f59e-111">方法</span><span class="sxs-lookup"><span data-stu-id="8f59e-111">Method</span></span>                    | <span data-ttu-id="8f59e-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="8f59e-112">Return Type</span></span> | <span data-ttu-id="8f59e-113">说明</span><span class="sxs-lookup"><span data-stu-id="8f59e-113">Description</span></span>
|:-------------------------------|:-------------------|:------
| <span data-ttu-id="8f59e-114">[获取][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-114">[Get][]</span></span>                   | <span data-ttu-id="8f59e-115">listItem</span><span class="sxs-lookup"><span data-stu-id="8f59e-115">listItem</span></span>| <span data-ttu-id="8f59e-116">获取列表中的项。</span><span class="sxs-lookup"><span data-stu-id="8f59e-116">Get an item in a list.</span></span>
| <span data-ttu-id="8f59e-117">[获取列值][Get]</span><span class="sxs-lookup"><span data-stu-id="8f59e-117">[Get column values][Get]</span></span>       | <span data-ttu-id="8f59e-118">listItem</span><span class="sxs-lookup"><span data-stu-id="8f59e-118">listItem</span></span> | <span data-ttu-id="8f59e-119">从 listItem 获取列的值。</span><span class="sxs-lookup"><span data-stu-id="8f59e-119">Get column values from listItem.</span></span>
| <span data-ttu-id="8f59e-120">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-120">[Get analytics][]</span></span>              | <span data-ttu-id="8f59e-121">[itemAnalytics][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-121">[itemAnalytics][]</span></span>| <span data-ttu-id="8f59e-122">对此资源可获取分析。</span><span class="sxs-lookup"><span data-stu-id="8f59e-122">Get analytics for this resource.</span></span> 
| <span data-ttu-id="8f59e-123">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-123">[Get activities by interval][]</span></span> | <span data-ttu-id="8f59e-124">[itemActivityStat][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-124">[itemActivityStat][]</span></span>| <span data-ttu-id="8f59e-125">在指定的时间间隔内获取 itemActivityStats 的集合。</span><span class="sxs-lookup"><span data-stu-id="8f59e-125">Get a collection of itemActivityStats within the specified time interval.</span></span>
| <span data-ttu-id="8f59e-126">[Create][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-126">[Create][]</span></span>                     | <span data-ttu-id="8f59e-127">listItem</span><span class="sxs-lookup"><span data-stu-id="8f59e-127">listItem</span></span> | <span data-ttu-id="8f59e-128">在列表中创建新的 listItem。</span><span class="sxs-lookup"><span data-stu-id="8f59e-128">Create a new listItem in a list.</span></span>
| <span data-ttu-id="8f59e-129">[删除][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-129">[Delete][]</span></span>                     | <span data-ttu-id="8f59e-130">无内容</span><span class="sxs-lookup"><span data-stu-id="8f59e-130">No Content</span></span> | <span data-ttu-id="8f59e-131">从 list 中删除项。</span><span class="sxs-lookup"><span data-stu-id="8f59e-131">Removes an item from a list.</span></span>
| <span data-ttu-id="8f59e-132">[Update][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-132">[Update][]</span></span>                     | <span data-ttu-id="8f59e-133">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-133">[fieldValueSet][]</span></span>| <span data-ttu-id="8f59e-134">更新 listItem 上的属性。</span><span class="sxs-lookup"><span data-stu-id="8f59e-134">Update the properties on a listItem.</span></span>
| <span data-ttu-id="8f59e-135">[更新列值][Update]</span><span class="sxs-lookup"><span data-stu-id="8f59e-135">[Update column values][Update]</span></span> | <span data-ttu-id="8f59e-136">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-136">[fieldValueSet][]</span></span>| <span data-ttu-id="8f59e-137">更新 listItem 上的列值。</span><span class="sxs-lookup"><span data-stu-id="8f59e-137">Update column values on a listItem.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8f59e-146">属性</span><span class="sxs-lookup"><span data-stu-id="8f59e-146">Properties</span></span>

<span data-ttu-id="8f59e-147">**listItem** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="8f59e-147">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="8f59e-148">属性名称</span><span class="sxs-lookup"><span data-stu-id="8f59e-148">Property name</span></span> | <span data-ttu-id="8f59e-149">类型</span><span class="sxs-lookup"><span data-stu-id="8f59e-149">Type</span></span>                | <span data-ttu-id="8f59e-150">说明</span><span class="sxs-lookup"><span data-stu-id="8f59e-150">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="8f59e-151">contentType</span><span class="sxs-lookup"><span data-stu-id="8f59e-151">contentType</span></span>   | <span data-ttu-id="8f59e-152">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-152">[contentTypeInfo][]</span></span> | <span data-ttu-id="8f59e-153">此列表项的内容类型</span><span class="sxs-lookup"><span data-stu-id="8f59e-153">The content type of this list item</span></span>

<span data-ttu-id="8f59e-154">以下属性继承自 **[baseItem][]**。</span><span class="sxs-lookup"><span data-stu-id="8f59e-154">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="8f59e-155">属性名称</span><span class="sxs-lookup"><span data-stu-id="8f59e-155">Property name</span></span>        | <span data-ttu-id="8f59e-156">类型</span><span class="sxs-lookup"><span data-stu-id="8f59e-156">Type</span></span>              | <span data-ttu-id="8f59e-157">说明</span><span class="sxs-lookup"><span data-stu-id="8f59e-157">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="8f59e-158">id</span><span class="sxs-lookup"><span data-stu-id="8f59e-158">id</span></span>                   | <span data-ttu-id="8f59e-159">string</span><span class="sxs-lookup"><span data-stu-id="8f59e-159">string</span></span>            | <span data-ttu-id="8f59e-p102">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="8f59e-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="8f59e-162">name</span><span class="sxs-lookup"><span data-stu-id="8f59e-162">name</span></span>                 | <span data-ttu-id="8f59e-163">string</span><span class="sxs-lookup"><span data-stu-id="8f59e-163">string</span></span>            | <span data-ttu-id="8f59e-164">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="8f59e-164">The name / title of the item.</span></span>
| <span data-ttu-id="8f59e-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="8f59e-165">createdBy</span></span>            | <span data-ttu-id="8f59e-166">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-166">[identitySet][]</span></span>   | <span data-ttu-id="8f59e-167">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="8f59e-167">Identity of the creator of this item.</span></span> <span data-ttu-id="8f59e-168">只读。</span><span class="sxs-lookup"><span data-stu-id="8f59e-168">Read-only.</span></span>
| <span data-ttu-id="8f59e-169">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f59e-169">createdDateTime</span></span>      | <span data-ttu-id="8f59e-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f59e-170">DateTimeOffset</span></span>    | <span data-ttu-id="8f59e-p104">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="8f59e-p104">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="8f59e-173">说明</span><span class="sxs-lookup"><span data-stu-id="8f59e-173">description</span></span>          | <span data-ttu-id="8f59e-174">string</span><span class="sxs-lookup"><span data-stu-id="8f59e-174">string</span></span>            | <span data-ttu-id="8f59e-175">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="8f59e-175">The descriptive text for the item.</span></span>
| <span data-ttu-id="8f59e-176">eTag</span><span class="sxs-lookup"><span data-stu-id="8f59e-176">eTag</span></span>                 | <span data-ttu-id="8f59e-177">字符串</span><span class="sxs-lookup"><span data-stu-id="8f59e-177">string</span></span>            | <span data-ttu-id="8f59e-p105">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="8f59e-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="8f59e-180">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8f59e-180">lastModifiedBy</span></span>       | <span data-ttu-id="8f59e-181">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-181">[identitySet][]</span></span>   | <span data-ttu-id="8f59e-182">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="8f59e-182">Identity of the last modifier of this item.</span></span> <span data-ttu-id="8f59e-183">只读。</span><span class="sxs-lookup"><span data-stu-id="8f59e-183">Read-only.</span></span>
| <span data-ttu-id="8f59e-184">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f59e-184">lastModifiedDateTime</span></span> | <span data-ttu-id="8f59e-185">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f59e-185">DateTimeOffset</span></span>    | <span data-ttu-id="8f59e-p107">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="8f59e-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="8f59e-188">parentReference</span><span class="sxs-lookup"><span data-stu-id="8f59e-188">parentReference</span></span>      | <span data-ttu-id="8f59e-189">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-189">[itemReference][]</span></span> | <span data-ttu-id="8f59e-p108">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="8f59e-p108">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="8f59e-192">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="8f59e-192">sharepointIds</span></span>        | <span data-ttu-id="8f59e-193">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-193">[sharepointIds][]</span></span> | <span data-ttu-id="8f59e-p109">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="8f59e-p109">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="8f59e-196">webUrl</span><span class="sxs-lookup"><span data-stu-id="8f59e-196">webUrl</span></span>               | <span data-ttu-id="8f59e-197">string (url)</span><span class="sxs-lookup"><span data-stu-id="8f59e-197">string (url)</span></span>      | <span data-ttu-id="8f59e-p110">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="8f59e-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="8f59e-200">关系</span><span class="sxs-lookup"><span data-stu-id="8f59e-200">Relationships</span></span>

 <span data-ttu-id="8f59e-201">**listItem** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="8f59e-201">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="8f59e-202">关系名称</span><span class="sxs-lookup"><span data-stu-id="8f59e-202">Relationship name</span></span> | <span data-ttu-id="8f59e-203">类型</span><span class="sxs-lookup"><span data-stu-id="8f59e-203">Type</span></span>                           | <span data-ttu-id="8f59e-204">说明</span><span class="sxs-lookup"><span data-stu-id="8f59e-204">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="8f59e-205">activities</span><span class="sxs-lookup"><span data-stu-id="8f59e-205">activities</span></span>        | <span data-ttu-id="8f59e-206">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="8f59e-206">[itemActivity][] collection</span></span>    | <span data-ttu-id="8f59e-207">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="8f59e-207">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="8f59e-208">分析</span><span class="sxs-lookup"><span data-stu-id="8f59e-208">analytics</span></span>         | <span data-ttu-id="8f59e-209">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="8f59e-209">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="8f59e-210">此项目上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="8f59e-210">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="8f59e-211">driveItem</span><span class="sxs-lookup"><span data-stu-id="8f59e-211">driveItem</span></span>         | <span data-ttu-id="8f59e-212">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-212">[driveItem][]</span></span>                  | <span data-ttu-id="8f59e-213">对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。</span><span class="sxs-lookup"><span data-stu-id="8f59e-213">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="8f59e-214">fields</span><span class="sxs-lookup"><span data-stu-id="8f59e-214">fields</span></span>            | <span data-ttu-id="8f59e-215">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="8f59e-215">[fieldValueSet][]</span></span>              | <span data-ttu-id="8f59e-216">在此列表项上设置的列的值。</span><span class="sxs-lookup"><span data-stu-id="8f59e-216">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="8f59e-217">版本</span><span class="sxs-lookup"><span data-stu-id="8f59e-217">versions</span></span>          | <span data-ttu-id="8f59e-218">[listItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="8f59e-218">[listItemVersion][] collection</span></span> | <span data-ttu-id="8f59e-219">先前版本的列表项的列表。</span><span class="sxs-lookup"><span data-stu-id="8f59e-219">The list of previous versions of the list item.</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="8f59e-231">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f59e-231">JSON representation</span></span>

<span data-ttu-id="8f59e-232">下面是 **listItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f59e-232">Here is a JSON representation of a **listItem** resource.</span></span>

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

