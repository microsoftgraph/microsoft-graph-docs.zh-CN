---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
localization_priority: Normal
ms.openlocfilehash: b2e151937d5e8db633edeb5d521d6e0c875b6d78
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866085"
---
# <a name="listitem-resource"></a><span data-ttu-id="ff1c0-102">ListItem 资源</span><span class="sxs-lookup"><span data-stu-id="ff1c0-102">ListItem resource</span></span>

> <span data-ttu-id="ff1c0-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff1c0-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff1c0-105">此资源表示 SharePoint **[list][]** 中的项目。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-105">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="ff1c0-106">该列表中的列值可通过 `fieldValueSet` 字典获得。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-106">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="ff1c0-107">listItem 上的任务</span><span class="sxs-lookup"><span data-stu-id="ff1c0-107">Tasks on a listItem</span></span>

<span data-ttu-id="ff1c0-108">下列任务可用于 **listItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-108">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="ff1c0-109">下面的所有示例都与**[list][]** 相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-109">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="ff1c0-110">常见任务</span><span class="sxs-lookup"><span data-stu-id="ff1c0-110">Common task</span></span>                    | <span data-ttu-id="ff1c0-111">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="ff1c0-111">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="ff1c0-112">[获取][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-112">[Get][]</span></span>                        | <span data-ttu-id="ff1c0-113">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ff1c0-113">GET /items/{item-id}</span></span>
| <span data-ttu-id="ff1c0-114">[获取列值][Get]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-114">[Get column values][Get]</span></span>       | <span data-ttu-id="ff1c0-115">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="ff1c0-115">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="ff1c0-116">[获取分析][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-116">[Get analytics][]</span></span>              | <span data-ttu-id="ff1c0-117">GET /items/ {项目-id} / 分析</span><span class="sxs-lookup"><span data-stu-id="ff1c0-117">GET /items/{item-id}/analytics</span></span>
| <span data-ttu-id="ff1c0-118">[按间隔获取活动][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-118">[Get activities by interval][]</span></span> | <span data-ttu-id="ff1c0-119">GET /items/ {项目-id} / getActivitiesByInterval</span><span class="sxs-lookup"><span data-stu-id="ff1c0-119">GET /items/{item-id}/getActivitiesByInterval</span></span>
| <span data-ttu-id="ff1c0-120">[创建][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-120">[Create][]</span></span>                     | <span data-ttu-id="ff1c0-121">POST /items</span><span class="sxs-lookup"><span data-stu-id="ff1c0-121">POST /items</span></span>
| <span data-ttu-id="ff1c0-122">[删除][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-122">[Delete][]</span></span>                     | <span data-ttu-id="ff1c0-123">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ff1c0-123">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="ff1c0-124">[更新][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-124">[Update][]</span></span>                     | <span data-ttu-id="ff1c0-125">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="ff1c0-125">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="ff1c0-126">[更新列值][Update]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-126">[Update column values][Update]</span></span> | <span data-ttu-id="ff1c0-127">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="ff1c0-127">PATCH /items/{item-id}/fields</span></span>

[获取]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[获取分析]: ../api/itemanalytics-get.md
[Get analytics]: ../api/itemanalytics-get.md
[按间隔获取活动]: ../api/itemactivity-getbyinterval.md
[Get activities by interval]: ../api/itemactivity-getbyinterval.md
[Create]: ../api/listitem-create.md
[删除]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[更新]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="ff1c0-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff1c0-134">JSON representation</span></span>

<span data-ttu-id="ff1c0-135">下面是 **listItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-135">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="ff1c0-136">属性</span><span class="sxs-lookup"><span data-stu-id="ff1c0-136">Properties</span></span>

<span data-ttu-id="ff1c0-137">**listItem** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-137">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="ff1c0-138">属性名称</span><span class="sxs-lookup"><span data-stu-id="ff1c0-138">Property name</span></span> | <span data-ttu-id="ff1c0-139">类型</span><span class="sxs-lookup"><span data-stu-id="ff1c0-139">Type</span></span>                | <span data-ttu-id="ff1c0-140">说明</span><span class="sxs-lookup"><span data-stu-id="ff1c0-140">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="ff1c0-141">contentType</span><span class="sxs-lookup"><span data-stu-id="ff1c0-141">contentType</span></span>   | <span data-ttu-id="ff1c0-142">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-142">[contentTypeInfo][]</span></span> | <span data-ttu-id="ff1c0-143">此列表项的内容类型</span><span class="sxs-lookup"><span data-stu-id="ff1c0-143">The content type of this list item</span></span>

<span data-ttu-id="ff1c0-144">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-144">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="ff1c0-145">属性名称</span><span class="sxs-lookup"><span data-stu-id="ff1c0-145">Property name</span></span>        | <span data-ttu-id="ff1c0-146">类型</span><span class="sxs-lookup"><span data-stu-id="ff1c0-146">Type</span></span>              | <span data-ttu-id="ff1c0-147">说明</span><span class="sxs-lookup"><span data-stu-id="ff1c0-147">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="ff1c0-148">ID</span><span class="sxs-lookup"><span data-stu-id="ff1c0-148">id</span></span>                   | <span data-ttu-id="ff1c0-149">string</span><span class="sxs-lookup"><span data-stu-id="ff1c0-149">string</span></span>            | <span data-ttu-id="ff1c0-p104">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-p104">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="ff1c0-152">name</span><span class="sxs-lookup"><span data-stu-id="ff1c0-152">name</span></span>                 | <span data-ttu-id="ff1c0-153">string</span><span class="sxs-lookup"><span data-stu-id="ff1c0-153">string</span></span>            | <span data-ttu-id="ff1c0-154">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-154">The name / title of the item.</span></span>
| <span data-ttu-id="ff1c0-155">createdBy</span><span class="sxs-lookup"><span data-stu-id="ff1c0-155">createdBy</span></span>            | <span data-ttu-id="ff1c0-156">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-156">[identitySet][]</span></span>   | <span data-ttu-id="ff1c0-157">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-157">Identity of the creator of this item.</span></span> <span data-ttu-id="ff1c0-158">只读。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-158">Read-only.</span></span>
| <span data-ttu-id="ff1c0-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff1c0-159">createdDateTime</span></span>      | <span data-ttu-id="ff1c0-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff1c0-160">DateTimeOffset</span></span>    | <span data-ttu-id="ff1c0-p106">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-p106">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="ff1c0-163">说明</span><span class="sxs-lookup"><span data-stu-id="ff1c0-163">description</span></span>          | <span data-ttu-id="ff1c0-164">string</span><span class="sxs-lookup"><span data-stu-id="ff1c0-164">string</span></span>            | <span data-ttu-id="ff1c0-165">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-165">The descriptive text for the item.</span></span>
| <span data-ttu-id="ff1c0-166">eTag</span><span class="sxs-lookup"><span data-stu-id="ff1c0-166">eTag</span></span>                 | <span data-ttu-id="ff1c0-167">string</span><span class="sxs-lookup"><span data-stu-id="ff1c0-167">string</span></span>            | <span data-ttu-id="ff1c0-p107">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-p107">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="ff1c0-170">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="ff1c0-170">lastModifiedBy</span></span>       | <span data-ttu-id="ff1c0-171">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-171">[identitySet][]</span></span>   | <span data-ttu-id="ff1c0-172">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-172">Identity of the last modifier of this item.</span></span> <span data-ttu-id="ff1c0-173">只读。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-173">Read-only.</span></span>
| <span data-ttu-id="ff1c0-174">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff1c0-174">lastModifiedDateTime</span></span> | <span data-ttu-id="ff1c0-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff1c0-175">DateTimeOffset</span></span>    | <span data-ttu-id="ff1c0-p109">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-p109">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="ff1c0-178">parentReference</span><span class="sxs-lookup"><span data-stu-id="ff1c0-178">parentReference</span></span>      | <span data-ttu-id="ff1c0-179">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-179">[itemReference][]</span></span> | <span data-ttu-id="ff1c0-p110">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-p110">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="ff1c0-182">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="ff1c0-182">sharepointIds</span></span>        | <span data-ttu-id="ff1c0-183">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-183">[sharepointIds][]</span></span> | <span data-ttu-id="ff1c0-p111">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-p111">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="ff1c0-186">WebUrl</span><span class="sxs-lookup"><span data-stu-id="ff1c0-186">webUrl</span></span>               | <span data-ttu-id="ff1c0-187">string (url)</span><span class="sxs-lookup"><span data-stu-id="ff1c0-187">string (url)</span></span>      | <span data-ttu-id="ff1c0-p112">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-p112">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="ff1c0-190">关系</span><span class="sxs-lookup"><span data-stu-id="ff1c0-190">Relationships</span></span>

 <span data-ttu-id="ff1c0-191">**listItem** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-191">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="ff1c0-192">关系名称</span><span class="sxs-lookup"><span data-stu-id="ff1c0-192">Relationship name</span></span> | <span data-ttu-id="ff1c0-193">类型</span><span class="sxs-lookup"><span data-stu-id="ff1c0-193">Type</span></span>                           | <span data-ttu-id="ff1c0-194">说明</span><span class="sxs-lookup"><span data-stu-id="ff1c0-194">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="ff1c0-195">activities</span><span class="sxs-lookup"><span data-stu-id="ff1c0-195">activities</span></span>        | <span data-ttu-id="ff1c0-196">[itemActivity][] 集合</span><span class="sxs-lookup"><span data-stu-id="ff1c0-196">[itemActivity][] collection</span></span>    | <span data-ttu-id="ff1c0-197">最近发生在此项上的活动的列表。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-197">The list of recent activities that took place on this item.</span></span>
| <span data-ttu-id="ff1c0-198">分析</span><span class="sxs-lookup"><span data-stu-id="ff1c0-198">analytics</span></span>         | <span data-ttu-id="ff1c0-199">[itemAnalytics][]资源</span><span class="sxs-lookup"><span data-stu-id="ff1c0-199">[itemAnalytics][] resource</span></span>     | <span data-ttu-id="ff1c0-200">有关此项发生查看活动的分析。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-200">Analytics about the view activities that took place on this item.</span></span>
| <span data-ttu-id="ff1c0-201">driveItem</span><span class="sxs-lookup"><span data-stu-id="ff1c0-201">driveItem</span></span>         | <span data-ttu-id="ff1c0-202">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-202">[driveItem][]</span></span>                  | <span data-ttu-id="ff1c0-203">对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-203">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="ff1c0-204">fields</span><span class="sxs-lookup"><span data-stu-id="ff1c0-204">fields</span></span>            | <span data-ttu-id="ff1c0-205">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="ff1c0-205">[fieldValueSet][]</span></span>              | <span data-ttu-id="ff1c0-206">在此列表项上设置的列的值。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-206">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="ff1c0-207">版本</span><span class="sxs-lookup"><span data-stu-id="ff1c0-207">versions</span></span>          | <span data-ttu-id="ff1c0-208">[listItemVersion][]集合</span><span class="sxs-lookup"><span data-stu-id="ff1c0-208">[listItemVersion][] collection</span></span> | <span data-ttu-id="ff1c0-209">早期版本的列表项的列表。</span><span class="sxs-lookup"><span data-stu-id="ff1c0-209">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemActivity]: itemactivity.md
[itemAnalytics]: itemanalytics.md
[itemReference]: itemreference.md
[列表]: list.md
[list]: list.md
[listItemVersion]: listitemversion.md
[sharepointIds]: sharepointids.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ListItem",
  "tocBookmarks": {
    "ListItem": "#"
  }
} -->
