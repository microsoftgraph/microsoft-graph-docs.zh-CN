---
author: JeremyKelley
description: 此资源表示 SharePoint list 中的项目。
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 226213d1361c78f592f92ddfe9b6f52c4f3defd0
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714296"
---
# <a name="listitem-resource"></a><span data-ttu-id="b320e-103">ListItem 资源</span><span class="sxs-lookup"><span data-stu-id="b320e-103">ListItem resource</span></span>

<span data-ttu-id="b320e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b320e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b320e-105">表示 SharePoint [列表][]中的项目。</span><span class="sxs-lookup"><span data-stu-id="b320e-105">Represents an item in a SharePoint [list][].</span></span>

<span data-ttu-id="b320e-106">SharePoint 文档库中的所有项目都可以表示为 **listItem** 或 [driveItem][] 资源。</span><span class="sxs-lookup"><span data-stu-id="b320e-106">All items in a SharePoint document library can be represented as a **listItem** or [driveItem][] resource.</span></span>

<span data-ttu-id="b320e-107">该列表中的列值可通过 `fieldValueSet` 字典获得。</span><span class="sxs-lookup"><span data-stu-id="b320e-107">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="b320e-108">listItem 上的任务</span><span class="sxs-lookup"><span data-stu-id="b320e-108">Tasks on a listItem</span></span>

<span data-ttu-id="b320e-109">下列任务可用于 **listItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="b320e-109">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="b320e-110">下面的所有示例都与 **[list][]** 相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`。</span><span class="sxs-lookup"><span data-stu-id="b320e-110">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="b320e-111">常见任务</span><span class="sxs-lookup"><span data-stu-id="b320e-111">Common task</span></span>                    | <span data-ttu-id="b320e-112">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="b320e-112">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="b320e-113">[获取][]</span><span class="sxs-lookup"><span data-stu-id="b320e-113">[Get][]</span></span>                        | <span data-ttu-id="b320e-114">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b320e-114">GET /items/{item-id}</span></span>
| <span data-ttu-id="b320e-115">[获取列值][Get]</span><span class="sxs-lookup"><span data-stu-id="b320e-115">[Get column values][Get]</span></span>       | <span data-ttu-id="b320e-116">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="b320e-116">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="b320e-117">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="b320e-117">[Get analytics][]</span></span>              | <span data-ttu-id="b320e-118">GET /items/{item-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="b320e-118">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="b320e-119">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="b320e-119">[Get activities by interval][]</span></span> | <span data-ttu-id="b320e-120">GET /items/{item-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="b320e-120">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="b320e-121">[创建][]</span><span class="sxs-lookup"><span data-stu-id="b320e-121">[Create][]</span></span>                     | <span data-ttu-id="b320e-122">POST /items</span><span class="sxs-lookup"><span data-stu-id="b320e-122">POST /items</span></span>
| <span data-ttu-id="b320e-123">[删除][]</span><span class="sxs-lookup"><span data-stu-id="b320e-123">[Delete][]</span></span>                     | <span data-ttu-id="b320e-124">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b320e-124">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="b320e-125">[更新][]</span><span class="sxs-lookup"><span data-stu-id="b320e-125">[Update][]</span></span>                     | <span data-ttu-id="b320e-126">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b320e-126">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="b320e-127">[更新列值][Update]</span><span class="sxs-lookup"><span data-stu-id="b320e-127">[Update column values][Update]</span></span> | <span data-ttu-id="b320e-128">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="b320e-128">PATCH /items/{item-id}/fields</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="b320e-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b320e-135">JSON representation</span></span>

<span data-ttu-id="b320e-136">下面是 **listItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b320e-136">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b320e-137">属性</span><span class="sxs-lookup"><span data-stu-id="b320e-137">Properties</span></span>

<span data-ttu-id="b320e-138">**listItem** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="b320e-138">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="b320e-139">属性名称</span><span class="sxs-lookup"><span data-stu-id="b320e-139">Property name</span></span> | <span data-ttu-id="b320e-140">类型</span><span class="sxs-lookup"><span data-stu-id="b320e-140">Type</span></span>                | <span data-ttu-id="b320e-141">说明</span><span class="sxs-lookup"><span data-stu-id="b320e-141">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="b320e-142">contentType</span><span class="sxs-lookup"><span data-stu-id="b320e-142">contentType</span></span>   | <span data-ttu-id="b320e-143">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="b320e-143">[contentTypeInfo][]</span></span> | <span data-ttu-id="b320e-144">此列表项的内容类型</span><span class="sxs-lookup"><span data-stu-id="b320e-144">The content type of this list item</span></span>

<span data-ttu-id="b320e-145">以下属性继承自 **[baseItem][]**。</span><span class="sxs-lookup"><span data-stu-id="b320e-145">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="b320e-146">属性名称</span><span class="sxs-lookup"><span data-stu-id="b320e-146">Property name</span></span>        | <span data-ttu-id="b320e-147">类型</span><span class="sxs-lookup"><span data-stu-id="b320e-147">Type</span></span>              | <span data-ttu-id="b320e-148">说明</span><span class="sxs-lookup"><span data-stu-id="b320e-148">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="b320e-149">id</span><span class="sxs-lookup"><span data-stu-id="b320e-149">id</span></span>                   | <span data-ttu-id="b320e-150">string</span><span class="sxs-lookup"><span data-stu-id="b320e-150">string</span></span>            | <span data-ttu-id="b320e-p102">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="b320e-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="b320e-153">name</span><span class="sxs-lookup"><span data-stu-id="b320e-153">name</span></span>                 | <span data-ttu-id="b320e-154">string</span><span class="sxs-lookup"><span data-stu-id="b320e-154">string</span></span>            | <span data-ttu-id="b320e-155">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="b320e-155">The name / title of the item.</span></span>
| <span data-ttu-id="b320e-156">createdBy</span><span class="sxs-lookup"><span data-stu-id="b320e-156">createdBy</span></span>            | <span data-ttu-id="b320e-157">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b320e-157">[identitySet][]</span></span>   | <span data-ttu-id="b320e-158">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="b320e-158">Identity of the creator of this item.</span></span> <span data-ttu-id="b320e-159">只读。</span><span class="sxs-lookup"><span data-stu-id="b320e-159">Read-only.</span></span>
| <span data-ttu-id="b320e-160">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b320e-160">createdDateTime</span></span>      | <span data-ttu-id="b320e-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b320e-161">DateTimeOffset</span></span>    | <span data-ttu-id="b320e-p104">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="b320e-p104">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="b320e-164">说明</span><span class="sxs-lookup"><span data-stu-id="b320e-164">description</span></span>          | <span data-ttu-id="b320e-165">string</span><span class="sxs-lookup"><span data-stu-id="b320e-165">string</span></span>            | <span data-ttu-id="b320e-166">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="b320e-166">The descriptive text for the item.</span></span>
| <span data-ttu-id="b320e-167">eTag</span><span class="sxs-lookup"><span data-stu-id="b320e-167">eTag</span></span>                 | <span data-ttu-id="b320e-168">字符串</span><span class="sxs-lookup"><span data-stu-id="b320e-168">string</span></span>            | <span data-ttu-id="b320e-p105">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="b320e-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="b320e-171">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b320e-171">lastModifiedBy</span></span>       | <span data-ttu-id="b320e-172">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b320e-172">[identitySet][]</span></span>   | <span data-ttu-id="b320e-173">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="b320e-173">Identity of the last modifier of this item.</span></span> <span data-ttu-id="b320e-174">只读。</span><span class="sxs-lookup"><span data-stu-id="b320e-174">Read-only.</span></span>
| <span data-ttu-id="b320e-175">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b320e-175">lastModifiedDateTime</span></span> | <span data-ttu-id="b320e-176">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b320e-176">DateTimeOffset</span></span>    | <span data-ttu-id="b320e-p107">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="b320e-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="b320e-179">parentReference</span><span class="sxs-lookup"><span data-stu-id="b320e-179">parentReference</span></span>      | <span data-ttu-id="b320e-180">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="b320e-180">[itemReference][]</span></span> | <span data-ttu-id="b320e-p108">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="b320e-p108">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="b320e-183">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="b320e-183">sharepointIds</span></span>        | <span data-ttu-id="b320e-184">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="b320e-184">[sharepointIds][]</span></span> | <span data-ttu-id="b320e-p109">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="b320e-p109">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="b320e-187">webUrl</span><span class="sxs-lookup"><span data-stu-id="b320e-187">webUrl</span></span>               | <span data-ttu-id="b320e-188">string (url)</span><span class="sxs-lookup"><span data-stu-id="b320e-188">string (url)</span></span>      | <span data-ttu-id="b320e-p110">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="b320e-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="b320e-191">关系</span><span class="sxs-lookup"><span data-stu-id="b320e-191">Relationships</span></span>

 <span data-ttu-id="b320e-192">**listItem** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="b320e-192">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="b320e-193">关系名称</span><span class="sxs-lookup"><span data-stu-id="b320e-193">Relationship name</span></span> | <span data-ttu-id="b320e-194">类型</span><span class="sxs-lookup"><span data-stu-id="b320e-194">Type</span></span>                           | <span data-ttu-id="b320e-195">说明</span><span class="sxs-lookup"><span data-stu-id="b320e-195">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="b320e-196">activities</span><span class="sxs-lookup"><span data-stu-id="b320e-196">activities</span></span>        | <span data-ttu-id="b320e-197">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="b320e-197">[itemActivity][] collection</span></span>    | <span data-ttu-id="b320e-198">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="b320e-198">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="b320e-199">分析</span><span class="sxs-lookup"><span data-stu-id="b320e-199">analytics</span></span>         | <span data-ttu-id="b320e-200">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="b320e-200">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="b320e-201">此项目上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="b320e-201">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="b320e-202">driveItem</span><span class="sxs-lookup"><span data-stu-id="b320e-202">driveItem</span></span>         | <span data-ttu-id="b320e-203">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="b320e-203">[driveItem][]</span></span>                  | <span data-ttu-id="b320e-204">对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。</span><span class="sxs-lookup"><span data-stu-id="b320e-204">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="b320e-205">fields</span><span class="sxs-lookup"><span data-stu-id="b320e-205">fields</span></span>            | <span data-ttu-id="b320e-206">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="b320e-206">[fieldValueSet][]</span></span>              | <span data-ttu-id="b320e-207">在此列表项上设置的列的值。</span><span class="sxs-lookup"><span data-stu-id="b320e-207">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="b320e-208">版本</span><span class="sxs-lookup"><span data-stu-id="b320e-208">versions</span></span>          | <span data-ttu-id="b320e-209">[listItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="b320e-209">[listItemVersion][] collection</span></span> | <span data-ttu-id="b320e-210">先前版本的列表项的列表。</span><span class="sxs-lookup"><span data-stu-id="b320e-210">The list of previous versions of the list item.</span></span>

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


