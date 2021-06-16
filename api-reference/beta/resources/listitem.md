---
author: JeremyKelley
description: 此资源表示 SharePoint list 中的项目。
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ad1e278f31bbeb0bc079f1ad2a6345d9b260cdec
ms.sourcegitcommit: e4461c7eb8c3d265fc1aa766125e81b58c6e1099
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2021
ms.locfileid: "52941464"
---
# <a name="listitem-resource"></a><span data-ttu-id="8cc02-103">ListItem 资源</span><span class="sxs-lookup"><span data-stu-id="8cc02-103">ListItem resource</span></span>

<span data-ttu-id="8cc02-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cc02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cc02-105">表示 SharePoint [列表][]中的项目。</span><span class="sxs-lookup"><span data-stu-id="8cc02-105">Represents an item in a SharePoint [list][].</span></span>

<span data-ttu-id="8cc02-106">SharePoint 文档库中的所有项目可以表示为 **listItem** 或 [driveItem][] 资源。</span><span class="sxs-lookup"><span data-stu-id="8cc02-106">All items in a SharePoint document library can be represented as a **listItem** or [driveItem][] resource.</span></span>

<span data-ttu-id="8cc02-107">该列表中的列值可通过 `fieldValueSet` 字典获得。</span><span class="sxs-lookup"><span data-stu-id="8cc02-107">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="8cc02-108">listItem 上的任务</span><span class="sxs-lookup"><span data-stu-id="8cc02-108">Tasks on a listItem</span></span>

<span data-ttu-id="8cc02-109">下列任务可用于 **listItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="8cc02-109">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="8cc02-110">下面的所有示例都与 **[list][]** 相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`。</span><span class="sxs-lookup"><span data-stu-id="8cc02-110">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="8cc02-111">常见任务</span><span class="sxs-lookup"><span data-stu-id="8cc02-111">Common task</span></span>                    | <span data-ttu-id="8cc02-112">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="8cc02-112">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="8cc02-113">[获取][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-113">[Get][]</span></span>                        | <span data-ttu-id="8cc02-114">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="8cc02-114">GET /items/{item-id}</span></span>
| <span data-ttu-id="8cc02-115">[获取列值][Get]</span><span class="sxs-lookup"><span data-stu-id="8cc02-115">[Get column values][Get]</span></span>       | <span data-ttu-id="8cc02-116">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="8cc02-116">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="8cc02-117">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-117">[Get analytics][]</span></span>              | <span data-ttu-id="8cc02-118">GET /items/{item-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="8cc02-118">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="8cc02-119">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-119">[Get activities by interval][]</span></span> | <span data-ttu-id="8cc02-120">GET /items/{item-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="8cc02-120">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="8cc02-121">[创建][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-121">[Create][]</span></span>                     | <span data-ttu-id="8cc02-122">POST /items</span><span class="sxs-lookup"><span data-stu-id="8cc02-122">POST /items</span></span>
| <span data-ttu-id="8cc02-123">[删除][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-123">[Delete][]</span></span>                     | <span data-ttu-id="8cc02-124">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="8cc02-124">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="8cc02-125">[更新][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-125">[Update][]</span></span>                     | <span data-ttu-id="8cc02-126">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="8cc02-126">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="8cc02-127">[更新列值][Update]</span><span class="sxs-lookup"><span data-stu-id="8cc02-127">[Update column values][Update]</span></span> | <span data-ttu-id="8cc02-128">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="8cc02-128">PATCH /items/{item-id}/fields</span></span>
| <span data-ttu-id="8cc02-129">[createLink][CreateLink]</span><span class="sxs-lookup"><span data-stu-id="8cc02-129">[createLink][CreateLink]</span></span>       | <span data-ttu-id="8cc02-130">POST /items/{itemId}/createLink</span><span class="sxs-lookup"><span data-stu-id="8cc02-130">POST /items/{itemId}/createLink</span></span>

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
[CreateLink]: ../api/listitem-createlink.md

## <a name="json-representation"></a><span data-ttu-id="8cc02-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cc02-137">JSON representation</span></span>

<span data-ttu-id="8cc02-138">下面是 **listItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cc02-138">Here is a JSON representation of a **listItem** resource.</span></span>

<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.baseItem",
  "@odata.type&quot;: &quot;microsoft.graph.listItem"
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
  "webUrl&quot;: &quot;url"
}
```

## <a name="properties"></a><span data-ttu-id="8cc02-139">属性</span><span class="sxs-lookup"><span data-stu-id="8cc02-139">Properties</span></span>

<span data-ttu-id="8cc02-140">**listItem** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="8cc02-140">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="8cc02-141">属性名称</span><span class="sxs-lookup"><span data-stu-id="8cc02-141">Property name</span></span> | <span data-ttu-id="8cc02-142">类型</span><span class="sxs-lookup"><span data-stu-id="8cc02-142">Type</span></span>                | <span data-ttu-id="8cc02-143">说明</span><span class="sxs-lookup"><span data-stu-id="8cc02-143">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="8cc02-144">contentType</span><span class="sxs-lookup"><span data-stu-id="8cc02-144">contentType</span></span>   | <span data-ttu-id="8cc02-145">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-145">[contentTypeInfo][]</span></span> | <span data-ttu-id="8cc02-146">此列表项的内容类型</span><span class="sxs-lookup"><span data-stu-id="8cc02-146">The content type of this list item</span></span>

<span data-ttu-id="8cc02-147">以下属性继承自 **[baseItem][]**。</span><span class="sxs-lookup"><span data-stu-id="8cc02-147">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="8cc02-148">属性名称</span><span class="sxs-lookup"><span data-stu-id="8cc02-148">Property name</span></span>        | <span data-ttu-id="8cc02-149">类型</span><span class="sxs-lookup"><span data-stu-id="8cc02-149">Type</span></span>              | <span data-ttu-id="8cc02-150">说明</span><span class="sxs-lookup"><span data-stu-id="8cc02-150">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="8cc02-151">id</span><span class="sxs-lookup"><span data-stu-id="8cc02-151">id</span></span>                   | <span data-ttu-id="8cc02-152">string</span><span class="sxs-lookup"><span data-stu-id="8cc02-152">string</span></span>            | <span data-ttu-id="8cc02-p102">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="8cc02-p102">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="8cc02-155">name</span><span class="sxs-lookup"><span data-stu-id="8cc02-155">name</span></span>                 | <span data-ttu-id="8cc02-156">string</span><span class="sxs-lookup"><span data-stu-id="8cc02-156">string</span></span>            | <span data-ttu-id="8cc02-157">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="8cc02-157">The name / title of the item.</span></span>
| <span data-ttu-id="8cc02-158">createdBy</span><span class="sxs-lookup"><span data-stu-id="8cc02-158">createdBy</span></span>            | <span data-ttu-id="8cc02-159">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-159">[identitySet][]</span></span>   | <span data-ttu-id="8cc02-160">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="8cc02-160">Identity of the creator of this item.</span></span> <span data-ttu-id="8cc02-161">只读。</span><span class="sxs-lookup"><span data-stu-id="8cc02-161">Read-only.</span></span>
| <span data-ttu-id="8cc02-162">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc02-162">createdDateTime</span></span>      | <span data-ttu-id="8cc02-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc02-163">DateTimeOffset</span></span>    | <span data-ttu-id="8cc02-p104">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="8cc02-p104">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="8cc02-166">说明</span><span class="sxs-lookup"><span data-stu-id="8cc02-166">description</span></span>          | <span data-ttu-id="8cc02-167">string</span><span class="sxs-lookup"><span data-stu-id="8cc02-167">string</span></span>            | <span data-ttu-id="8cc02-168">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="8cc02-168">The descriptive text for the item.</span></span>
| <span data-ttu-id="8cc02-169">eTag</span><span class="sxs-lookup"><span data-stu-id="8cc02-169">eTag</span></span>                 | <span data-ttu-id="8cc02-170">字符串</span><span class="sxs-lookup"><span data-stu-id="8cc02-170">string</span></span>            | <span data-ttu-id="8cc02-p105">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="8cc02-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="8cc02-173">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8cc02-173">lastModifiedBy</span></span>       | <span data-ttu-id="8cc02-174">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-174">[identitySet][]</span></span>   | <span data-ttu-id="8cc02-175">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="8cc02-175">Identity of the last modifier of this item.</span></span> <span data-ttu-id="8cc02-176">只读。</span><span class="sxs-lookup"><span data-stu-id="8cc02-176">Read-only.</span></span>
| <span data-ttu-id="8cc02-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cc02-177">lastModifiedDateTime</span></span> | <span data-ttu-id="8cc02-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cc02-178">DateTimeOffset</span></span>    | <span data-ttu-id="8cc02-p107">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="8cc02-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="8cc02-181">parentReference</span><span class="sxs-lookup"><span data-stu-id="8cc02-181">parentReference</span></span>      | <span data-ttu-id="8cc02-182">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-182">[itemReference][]</span></span> | <span data-ttu-id="8cc02-p108">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="8cc02-p108">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="8cc02-185">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="8cc02-185">sharepointIds</span></span>        | <span data-ttu-id="8cc02-186">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-186">[sharepointIds][]</span></span> | <span data-ttu-id="8cc02-p109">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="8cc02-p109">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="8cc02-189">webUrl</span><span class="sxs-lookup"><span data-stu-id="8cc02-189">webUrl</span></span>               | <span data-ttu-id="8cc02-190">string (url)</span><span class="sxs-lookup"><span data-stu-id="8cc02-190">string (url)</span></span>      | <span data-ttu-id="8cc02-p110">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="8cc02-p110">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="8cc02-193">关系</span><span class="sxs-lookup"><span data-stu-id="8cc02-193">Relationships</span></span>

 <span data-ttu-id="8cc02-194">**listItem** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="8cc02-194">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="8cc02-195">关系名称</span><span class="sxs-lookup"><span data-stu-id="8cc02-195">Relationship name</span></span> | <span data-ttu-id="8cc02-196">类型</span><span class="sxs-lookup"><span data-stu-id="8cc02-196">Type</span></span>                           | <span data-ttu-id="8cc02-197">说明</span><span class="sxs-lookup"><span data-stu-id="8cc02-197">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="8cc02-198">activities</span><span class="sxs-lookup"><span data-stu-id="8cc02-198">activities</span></span>        | <span data-ttu-id="8cc02-199">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="8cc02-199">[itemActivity][] collection</span></span>    | <span data-ttu-id="8cc02-200">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="8cc02-200">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="8cc02-201">分析</span><span class="sxs-lookup"><span data-stu-id="8cc02-201">analytics</span></span>         | <span data-ttu-id="8cc02-202">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="8cc02-202">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="8cc02-203">此项目上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="8cc02-203">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="8cc02-204">driveItem</span><span class="sxs-lookup"><span data-stu-id="8cc02-204">driveItem</span></span>         | <span data-ttu-id="8cc02-205">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-205">[driveItem][]</span></span>                  | <span data-ttu-id="8cc02-206">对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。</span><span class="sxs-lookup"><span data-stu-id="8cc02-206">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="8cc02-207">fields</span><span class="sxs-lookup"><span data-stu-id="8cc02-207">fields</span></span>            | <span data-ttu-id="8cc02-208">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="8cc02-208">[fieldValueSet][]</span></span>              | <span data-ttu-id="8cc02-209">在此列表项上设置的列的值。</span><span class="sxs-lookup"><span data-stu-id="8cc02-209">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="8cc02-210">版本</span><span class="sxs-lookup"><span data-stu-id="8cc02-210">versions</span></span>          | <span data-ttu-id="8cc02-211">[listItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="8cc02-211">[listItemVersion][] collection</span></span> | <span data-ttu-id="8cc02-212">先前版本的列表项的列表。</span><span class="sxs-lookup"><span data-stu-id="8cc02-212">The list of previous versions of the list item.</span></span>

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
    "ListItem&quot;: &quot;#"
  },
  "suppressions": []
}
-->


