---
author: JeremyKelley
description: 此资源表示 SharePoint list 中的项目。
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 03f3dae851cf9a23dbe300f834846046dce4de74
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522944"
---
# <a name="listitem-resource"></a><span data-ttu-id="007a6-103">ListItem 资源</span><span class="sxs-lookup"><span data-stu-id="007a6-103">ListItem resource</span></span>

<span data-ttu-id="007a6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="007a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="007a6-105">此资源表示 SharePoint **[list][]** 中的项目。</span><span class="sxs-lookup"><span data-stu-id="007a6-105">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="007a6-106">该列表中的列值可通过 `fieldValueSet` 字典获得。</span><span class="sxs-lookup"><span data-stu-id="007a6-106">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="007a6-107">listItem 上的任务</span><span class="sxs-lookup"><span data-stu-id="007a6-107">Tasks on a listItem</span></span>

<span data-ttu-id="007a6-108">下列任务可用于 **listItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="007a6-108">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="007a6-109">下面的所有示例都与**[list][]** 相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`。</span><span class="sxs-lookup"><span data-stu-id="007a6-109">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="007a6-110">常见任务</span><span class="sxs-lookup"><span data-stu-id="007a6-110">Common task</span></span>                    | <span data-ttu-id="007a6-111">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="007a6-111">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="007a6-112">[获取][]</span><span class="sxs-lookup"><span data-stu-id="007a6-112">[Get][]</span></span>                        | <span data-ttu-id="007a6-113">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="007a6-113">GET /items/{item-id}</span></span>
| <span data-ttu-id="007a6-114">[获取列值][Get]</span><span class="sxs-lookup"><span data-stu-id="007a6-114">[Get column values][Get]</span></span>       | <span data-ttu-id="007a6-115">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="007a6-115">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="007a6-116">[获取分析结果][]</span><span class="sxs-lookup"><span data-stu-id="007a6-116">[Get analytics][]</span></span>              | <span data-ttu-id="007a6-117">获取/items/{item-id}/analytics</span><span class="sxs-lookup"><span data-stu-id="007a6-117">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="007a6-118">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="007a6-118">[Get activities by interval][]</span></span> | <span data-ttu-id="007a6-119">获取/items/{item-id}/getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="007a6-119">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="007a6-120">[创建][]</span><span class="sxs-lookup"><span data-stu-id="007a6-120">[Create][]</span></span>                     | <span data-ttu-id="007a6-121">POST /items</span><span class="sxs-lookup"><span data-stu-id="007a6-121">POST /items</span></span>
| <span data-ttu-id="007a6-122">[删除][]</span><span class="sxs-lookup"><span data-stu-id="007a6-122">[Delete][]</span></span>                     | <span data-ttu-id="007a6-123">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="007a6-123">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="007a6-124">[更新][]</span><span class="sxs-lookup"><span data-stu-id="007a6-124">[Update][]</span></span>                     | <span data-ttu-id="007a6-125">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="007a6-125">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="007a6-126">[更新列值][Update]</span><span class="sxs-lookup"><span data-stu-id="007a6-126">[Update column values][Update]</span></span> | <span data-ttu-id="007a6-127">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="007a6-127">PATCH /items/{item-id}/fields</span></span>

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

## <a name="json-representation"></a><span data-ttu-id="007a6-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="007a6-134">JSON representation</span></span>

<span data-ttu-id="007a6-135">下面是 **listItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="007a6-135">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="007a6-136">属性</span><span class="sxs-lookup"><span data-stu-id="007a6-136">Properties</span></span>

<span data-ttu-id="007a6-137">**listItem** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="007a6-137">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="007a6-138">属性名称</span><span class="sxs-lookup"><span data-stu-id="007a6-138">Property name</span></span> | <span data-ttu-id="007a6-139">类型</span><span class="sxs-lookup"><span data-stu-id="007a6-139">Type</span></span>                | <span data-ttu-id="007a6-140">说明</span><span class="sxs-lookup"><span data-stu-id="007a6-140">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="007a6-141">contentType</span><span class="sxs-lookup"><span data-stu-id="007a6-141">contentType</span></span>   | <span data-ttu-id="007a6-142">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="007a6-142">[contentTypeInfo][]</span></span> | <span data-ttu-id="007a6-143">此列表项的内容类型</span><span class="sxs-lookup"><span data-stu-id="007a6-143">The content type of this list item</span></span>

<span data-ttu-id="007a6-144">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="007a6-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="007a6-145">属性名称</span><span class="sxs-lookup"><span data-stu-id="007a6-145">Property name</span></span>        | <span data-ttu-id="007a6-146">类型</span><span class="sxs-lookup"><span data-stu-id="007a6-146">Type</span></span>              | <span data-ttu-id="007a6-147">说明</span><span class="sxs-lookup"><span data-stu-id="007a6-147">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="007a6-148">id</span><span class="sxs-lookup"><span data-stu-id="007a6-148">id</span></span>                   | <span data-ttu-id="007a6-149">string</span><span class="sxs-lookup"><span data-stu-id="007a6-149">string</span></span>            | <span data-ttu-id="007a6-p103">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="007a6-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="007a6-152">name</span><span class="sxs-lookup"><span data-stu-id="007a6-152">name</span></span>                 | <span data-ttu-id="007a6-153">string</span><span class="sxs-lookup"><span data-stu-id="007a6-153">string</span></span>            | <span data-ttu-id="007a6-154">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="007a6-154">The name / title of the item.</span></span>
| <span data-ttu-id="007a6-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="007a6-155">createdBy</span></span>            | <span data-ttu-id="007a6-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="007a6-156">[identitySet][]</span></span>   | <span data-ttu-id="007a6-157">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="007a6-157">Identity of the creator of this item.</span></span> <span data-ttu-id="007a6-158">只读。</span><span class="sxs-lookup"><span data-stu-id="007a6-158">Read-only.</span></span>
| <span data-ttu-id="007a6-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="007a6-159">createdDateTime</span></span>      | <span data-ttu-id="007a6-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="007a6-160">DateTimeOffset</span></span>    | <span data-ttu-id="007a6-p105">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="007a6-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="007a6-163">说明</span><span class="sxs-lookup"><span data-stu-id="007a6-163">description</span></span>          | <span data-ttu-id="007a6-164">string</span><span class="sxs-lookup"><span data-stu-id="007a6-164">string</span></span>            | <span data-ttu-id="007a6-165">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="007a6-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="007a6-166">eTag</span><span class="sxs-lookup"><span data-stu-id="007a6-166">eTag</span></span>                 | <span data-ttu-id="007a6-167">字符串</span><span class="sxs-lookup"><span data-stu-id="007a6-167">string</span></span>            | <span data-ttu-id="007a6-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="007a6-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="007a6-170">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="007a6-170">lastModifiedBy</span></span>       | <span data-ttu-id="007a6-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="007a6-171">[identitySet][]</span></span>   | <span data-ttu-id="007a6-172">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="007a6-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="007a6-173">只读。</span><span class="sxs-lookup"><span data-stu-id="007a6-173">Read-only.</span></span>
| <span data-ttu-id="007a6-174">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="007a6-174">lastModifiedDateTime</span></span> | <span data-ttu-id="007a6-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="007a6-175">DateTimeOffset</span></span>    | <span data-ttu-id="007a6-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="007a6-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="007a6-178">parentReference</span><span class="sxs-lookup"><span data-stu-id="007a6-178">parentReference</span></span>      | <span data-ttu-id="007a6-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="007a6-179">[itemReference][]</span></span> | <span data-ttu-id="007a6-p109">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="007a6-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="007a6-182">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="007a6-182">sharepointIds</span></span>        | <span data-ttu-id="007a6-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="007a6-183">[sharepointIds][]</span></span> | <span data-ttu-id="007a6-p110">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="007a6-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="007a6-186">webUrl</span><span class="sxs-lookup"><span data-stu-id="007a6-186">webUrl</span></span>               | <span data-ttu-id="007a6-187">string (url)</span><span class="sxs-lookup"><span data-stu-id="007a6-187">string (url)</span></span>      | <span data-ttu-id="007a6-p111">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="007a6-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="007a6-190">关系</span><span class="sxs-lookup"><span data-stu-id="007a6-190">Relationships</span></span>

 <span data-ttu-id="007a6-191">**listItem** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="007a6-191">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="007a6-192">关系名称</span><span class="sxs-lookup"><span data-stu-id="007a6-192">Relationship name</span></span> | <span data-ttu-id="007a6-193">类型</span><span class="sxs-lookup"><span data-stu-id="007a6-193">Type</span></span>                           | <span data-ttu-id="007a6-194">说明</span><span class="sxs-lookup"><span data-stu-id="007a6-194">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="007a6-195">activities</span><span class="sxs-lookup"><span data-stu-id="007a6-195">activities</span></span>        | <span data-ttu-id="007a6-196">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="007a6-196">[itemActivity][] collection</span></span>    | <span data-ttu-id="007a6-197">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="007a6-197">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="007a6-198">分析</span><span class="sxs-lookup"><span data-stu-id="007a6-198">analytics</span></span>         | <span data-ttu-id="007a6-199">[itemAnalytics][] 资源</span><span class="sxs-lookup"><span data-stu-id="007a6-199">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="007a6-200">此项目上发生的查看活动的相关分析。</span><span class="sxs-lookup"><span data-stu-id="007a6-200">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="007a6-201">driveItem</span><span class="sxs-lookup"><span data-stu-id="007a6-201">driveItem</span></span>         | <span data-ttu-id="007a6-202">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="007a6-202">[driveItem][]</span></span>                  | <span data-ttu-id="007a6-203">对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。</span><span class="sxs-lookup"><span data-stu-id="007a6-203">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="007a6-204">fields</span><span class="sxs-lookup"><span data-stu-id="007a6-204">fields</span></span>            | <span data-ttu-id="007a6-205">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="007a6-205">[fieldValueSet][]</span></span>              | <span data-ttu-id="007a6-206">在此列表项上设置的列的值。</span><span class="sxs-lookup"><span data-stu-id="007a6-206">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="007a6-207">版本</span><span class="sxs-lookup"><span data-stu-id="007a6-207">versions</span></span>          | <span data-ttu-id="007a6-208">[listItemVersion][] 集合</span><span class="sxs-lookup"><span data-stu-id="007a6-208">[listItemVersion][] collection</span></span> | <span data-ttu-id="007a6-209">先前版本的列表项的列表。</span><span class="sxs-lookup"><span data-stu-id="007a6-209">The list of previous versions of the list item.</span></span>

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
