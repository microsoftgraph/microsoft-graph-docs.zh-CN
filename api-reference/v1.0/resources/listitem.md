---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: b7293398314ea91dcb5ac6985031f91d6531e78f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010875"
---
# <a name="listitem-resource"></a><span data-ttu-id="28e44-102">ListItem 资源</span><span class="sxs-lookup"><span data-stu-id="28e44-102">ListItem resource</span></span>

<span data-ttu-id="28e44-103">此资源表示 SharePoint **[list][]** 中的项目。</span><span class="sxs-lookup"><span data-stu-id="28e44-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="28e44-104">该列表中的列值可通过 `fieldValueSet` 字典获得。</span><span class="sxs-lookup"><span data-stu-id="28e44-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="28e44-105">listItem 上的任务</span><span class="sxs-lookup"><span data-stu-id="28e44-105">Tasks on a listItem</span></span>

<span data-ttu-id="28e44-106">下列任务可用于 **listItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="28e44-106">The following tasks are available for **listItem** resources.</span></span>
<span data-ttu-id="28e44-107">下面的所有示例都与**[list][]** 相关，例如：`https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`。</span><span class="sxs-lookup"><span data-stu-id="28e44-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="28e44-108">常见任务</span><span class="sxs-lookup"><span data-stu-id="28e44-108">Common task</span></span>                    | <span data-ttu-id="28e44-109">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="28e44-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="28e44-110">[获取][]</span><span class="sxs-lookup"><span data-stu-id="28e44-110">[Get][]</span></span>                        | <span data-ttu-id="28e44-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="28e44-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="28e44-112">[获取列值][Get]</span><span class="sxs-lookup"><span data-stu-id="28e44-112">[Get column values][Get]</span></span>       | <span data-ttu-id="28e44-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="28e44-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="28e44-114">[创建][]</span><span class="sxs-lookup"><span data-stu-id="28e44-114">[Create][]</span></span>                     | <span data-ttu-id="28e44-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="28e44-115">POST /items</span></span>
| <span data-ttu-id="28e44-116">[删除][]</span><span class="sxs-lookup"><span data-stu-id="28e44-116">[Delete][]</span></span>                     | <span data-ttu-id="28e44-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="28e44-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="28e44-118">[更新][]</span><span class="sxs-lookup"><span data-stu-id="28e44-118">[Update][]</span></span>                     | <span data-ttu-id="28e44-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="28e44-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="28e44-120">[更新列值][Update]</span><span class="sxs-lookup"><span data-stu-id="28e44-120">[Update column values][Update]</span></span> | <span data-ttu-id="28e44-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="28e44-121">PATCH /items/{item-id}/fields</span></span>

[获取]: ../api/listitem-get.md
[Get]: ../api/listitem-get.md
[创建]: ../api/listitem-create.md
[Create]: ../api/listitem-create.md
[删除]: ../api/listitem-delete.md
[Delete]: ../api/listitem-delete.md
[更新]: ../api/listitem-update.md
[Update]: ../api/listitem-update.md

## <a name="json-representation"></a><span data-ttu-id="28e44-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28e44-126">JSON representation</span></span>

<span data-ttu-id="28e44-127">下面是 **listItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28e44-127">Here is a JSON representation of a **listItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="28e44-128">属性</span><span class="sxs-lookup"><span data-stu-id="28e44-128">Properties</span></span>

<span data-ttu-id="28e44-129">**listItem** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="28e44-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="28e44-130">属性名称</span><span class="sxs-lookup"><span data-stu-id="28e44-130">Property name</span></span> | <span data-ttu-id="28e44-131">类型</span><span class="sxs-lookup"><span data-stu-id="28e44-131">Type</span></span>                | <span data-ttu-id="28e44-132">说明</span><span class="sxs-lookup"><span data-stu-id="28e44-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="28e44-133">contentType</span><span class="sxs-lookup"><span data-stu-id="28e44-133">contentType</span></span>   | <span data-ttu-id="28e44-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="28e44-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="28e44-135">此列表项的内容类型</span><span class="sxs-lookup"><span data-stu-id="28e44-135">The content type of this list item</span></span>

<span data-ttu-id="28e44-136">以下属性继承自 \*\* [baseItem][]\*\*。</span><span class="sxs-lookup"><span data-stu-id="28e44-136">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="28e44-137">属性名称</span><span class="sxs-lookup"><span data-stu-id="28e44-137">Property name</span></span>        | <span data-ttu-id="28e44-138">类型</span><span class="sxs-lookup"><span data-stu-id="28e44-138">Type</span></span>              | <span data-ttu-id="28e44-139">说明</span><span class="sxs-lookup"><span data-stu-id="28e44-139">Description</span></span>
|:---------------------|:------------------|:----------------------------------
| <span data-ttu-id="28e44-140">ID</span><span class="sxs-lookup"><span data-stu-id="28e44-140">id</span></span>                   | <span data-ttu-id="28e44-141">string</span><span class="sxs-lookup"><span data-stu-id="28e44-141">string</span></span>            | <span data-ttu-id="28e44-p103">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="28e44-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="28e44-144">name</span><span class="sxs-lookup"><span data-stu-id="28e44-144">name</span></span>                 | <span data-ttu-id="28e44-145">string</span><span class="sxs-lookup"><span data-stu-id="28e44-145">string</span></span>            | <span data-ttu-id="28e44-146">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="28e44-146">The name / title of the item.</span></span>
| <span data-ttu-id="28e44-147">createdBy</span><span class="sxs-lookup"><span data-stu-id="28e44-147">createdBy</span></span>            | <span data-ttu-id="28e44-148">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="28e44-148">[identitySet][]</span></span>   | <span data-ttu-id="28e44-149">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="28e44-149">Identity of the creator of this item.</span></span> <span data-ttu-id="28e44-150">只读。</span><span class="sxs-lookup"><span data-stu-id="28e44-150">Read-only.</span></span>
| <span data-ttu-id="28e44-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28e44-151">createdDateTime</span></span>      | <span data-ttu-id="28e44-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28e44-152">DateTimeOffset</span></span>    | <span data-ttu-id="28e44-p105">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="28e44-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="28e44-155">说明</span><span class="sxs-lookup"><span data-stu-id="28e44-155">description</span></span>          | <span data-ttu-id="28e44-156">string</span><span class="sxs-lookup"><span data-stu-id="28e44-156">string</span></span>            | <span data-ttu-id="28e44-157">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="28e44-157">The descriptive text for the item.</span></span>
| <span data-ttu-id="28e44-158">eTag</span><span class="sxs-lookup"><span data-stu-id="28e44-158">eTag</span></span>                 | <span data-ttu-id="28e44-159">string</span><span class="sxs-lookup"><span data-stu-id="28e44-159">string</span></span>            | <span data-ttu-id="28e44-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="28e44-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="28e44-162">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="28e44-162">lastModifiedBy</span></span>       | <span data-ttu-id="28e44-163">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="28e44-163">[identitySet][]</span></span>   | <span data-ttu-id="28e44-164">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="28e44-164">Identity of the last modifier of this item.</span></span> <span data-ttu-id="28e44-165">只读。</span><span class="sxs-lookup"><span data-stu-id="28e44-165">Read-only.</span></span>
| <span data-ttu-id="28e44-166">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28e44-166">lastModifiedDateTime</span></span> | <span data-ttu-id="28e44-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28e44-167">DateTimeOffset</span></span>    | <span data-ttu-id="28e44-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="28e44-p108">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="28e44-170">parentReference</span><span class="sxs-lookup"><span data-stu-id="28e44-170">parentReference</span></span>      | <span data-ttu-id="28e44-171">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="28e44-171">[itemReference][]</span></span> | <span data-ttu-id="28e44-p109">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="28e44-p109">Parent information, if the item has a parent. Read-write.</span></span>
| <span data-ttu-id="28e44-174">sharepointIds</span><span class="sxs-lookup"><span data-stu-id="28e44-174">sharepointIds</span></span>        | <span data-ttu-id="28e44-175">[sharepointIds][]</span><span class="sxs-lookup"><span data-stu-id="28e44-175">[sharepointIds][]</span></span> | <span data-ttu-id="28e44-p110">返回对 SharePoint REST 兼容性有用的标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="28e44-p110">Returns identifiers useful for SharePoint REST compatibility. Read-only.</span></span>
| <span data-ttu-id="28e44-178">WebUrl</span><span class="sxs-lookup"><span data-stu-id="28e44-178">webUrl</span></span>               | <span data-ttu-id="28e44-179">string (url)</span><span class="sxs-lookup"><span data-stu-id="28e44-179">string (url)</span></span>      | <span data-ttu-id="28e44-p111">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="28e44-p111">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="28e44-182">关系</span><span class="sxs-lookup"><span data-stu-id="28e44-182">Relationships</span></span>

 <span data-ttu-id="28e44-183">**listItem** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="28e44-183">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="28e44-184">关系名称</span><span class="sxs-lookup"><span data-stu-id="28e44-184">Relationship name</span></span> | <span data-ttu-id="28e44-185">类型</span><span class="sxs-lookup"><span data-stu-id="28e44-185">Type</span></span>                           | <span data-ttu-id="28e44-186">说明</span><span class="sxs-lookup"><span data-stu-id="28e44-186">Description</span></span>
|:------------------|:-------------------------------|:-------------------------------
| <span data-ttu-id="28e44-187">driveItem</span><span class="sxs-lookup"><span data-stu-id="28e44-187">driveItem</span></span>         | <span data-ttu-id="28e44-188">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="28e44-188">[driveItem][]</span></span>                  | <span data-ttu-id="28e44-189">对于文档库，**driveItem** 关系将 listItem 显示为 **[driveItem][]**。</span><span class="sxs-lookup"><span data-stu-id="28e44-189">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>
| <span data-ttu-id="28e44-190">fields</span><span class="sxs-lookup"><span data-stu-id="28e44-190">fields</span></span>            | <span data-ttu-id="28e44-191">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="28e44-191">[fieldValueSet][]</span></span>              | <span data-ttu-id="28e44-192">在此列表项上设置的列的值。</span><span class="sxs-lookup"><span data-stu-id="28e44-192">The values of the columns set on this list item.</span></span>
| <span data-ttu-id="28e44-193">版本</span><span class="sxs-lookup"><span data-stu-id="28e44-193">versions</span></span>          | <span data-ttu-id="28e44-194">[listItemVersion][]集合</span><span class="sxs-lookup"><span data-stu-id="28e44-194">[listItemVersion][] collection</span></span> | <span data-ttu-id="28e44-195">早期版本的列表项的列表。</span><span class="sxs-lookup"><span data-stu-id="28e44-195">The list of previous versions of the list item.</span></span>

[baseItem]: baseitem.md
[contentTypeInfo]: contenttypeinfo.md
[driveItem]: driveitem.md
[fieldValueSet]: fieldvalueset.md
[identitySet]: identityset.md
[itemReference]: itemreference.md
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
