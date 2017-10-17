---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListItem
ms.openlocfilehash: eabb88eb6ad2eee7a032b2486555aa26c557ba1a
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="listitem-resource"></a><span data-ttu-id="b7e69-102">ListItem 资源</span><span class="sxs-lookup"><span data-stu-id="b7e69-102">ListItem resource</span></span>

<span data-ttu-id="b7e69-103">此资源表示 SharePoint **[列表][]**中的项目。</span><span class="sxs-lookup"><span data-stu-id="b7e69-103">This resource represents an item in a SharePoint **[list][]**.</span></span>
<span data-ttu-id="b7e69-104">该列表中的列值可通过 `fieldValueSet` 字典获得。</span><span class="sxs-lookup"><span data-stu-id="b7e69-104">Column values in the list are available through the `fieldValueSet` dictionary.</span></span>

## <a name="tasks-on-a-listitem"></a><span data-ttu-id="b7e69-105">listItem 上的任务</span><span class="sxs-lookup"><span data-stu-id="b7e69-105">Tasks on a listItem</span></span>

<span data-ttu-id="b7e69-106">下列任务可用于 **listItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="b7e69-106">The following tasks are available for {type} resources.</span></span>
<span data-ttu-id="b7e69-107">下面的所有示例都与**[列表][]**相关，例如：`https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`。</span><span class="sxs-lookup"><span data-stu-id="b7e69-107">All examples below are relative to a **[list][]**, eg: `https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}`.</span></span>

| <span data-ttu-id="b7e69-108">常见任务</span><span class="sxs-lookup"><span data-stu-id="b7e69-108">Common task</span></span>                    | <span data-ttu-id="b7e69-109">HTTP 方法</span><span class="sxs-lookup"><span data-stu-id="b7e69-109">HTTP method</span></span>
|:-------------------------------|:------------------------
| <span data-ttu-id="b7e69-110">[获取][]</span><span class="sxs-lookup"><span data-stu-id="b7e69-110">[Get][]</span></span>                        | <span data-ttu-id="b7e69-111">GET /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b7e69-111">GET /items/{item-id}</span></span>
| <span data-ttu-id="b7e69-112">[获取列值][获取]</span><span class="sxs-lookup"><span data-stu-id="b7e69-112">[Get column values][Get]</span></span>       | <span data-ttu-id="b7e69-113">GET /items/{item-id}?expand=fields</span><span class="sxs-lookup"><span data-stu-id="b7e69-113">GET /items/{item-id}?expand=fields</span></span>
| <span data-ttu-id="b7e69-114">[创建][]</span><span class="sxs-lookup"><span data-stu-id="b7e69-114">[Create][]</span></span>                     | <span data-ttu-id="b7e69-115">POST /items</span><span class="sxs-lookup"><span data-stu-id="b7e69-115">POST /items</span></span>
| <span data-ttu-id="b7e69-116">[删除][]</span><span class="sxs-lookup"><span data-stu-id="b7e69-116">[Delete][]</span></span>                     | <span data-ttu-id="b7e69-117">DELETE /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b7e69-117">DELETE /items/{item-id}</span></span>
| <span data-ttu-id="b7e69-118">[更新][]</span><span class="sxs-lookup"><span data-stu-id="b7e69-118">[Update][]</span></span>                     | <span data-ttu-id="b7e69-119">PATCH /items/{item-id}</span><span class="sxs-lookup"><span data-stu-id="b7e69-119">PATCH /items/{item-id}</span></span>
| <span data-ttu-id="b7e69-120">[更新列值][更新]</span><span class="sxs-lookup"><span data-stu-id="b7e69-120">[Update column values][Update]</span></span> | <span data-ttu-id="b7e69-121">PATCH /items/{item-id}/fields</span><span class="sxs-lookup"><span data-stu-id="b7e69-121">PATCH /items/{item-id}/fields</span></span>

[获取]: ../api/listItem_get.md
[创建]: ../api/listItem_create.md
[删除]: ../api/listItem_delete.md
[更新]: ../api/listItem_update.md

## <a name="json-representation"></a><span data-ttu-id="b7e69-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7e69-126">JSON representation</span></span>

<span data-ttu-id="b7e69-127">下面是 **listItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7e69-127">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.listItem",
       "keyProperty": "id" } -->

```json
{
  "contentType": { "@odata.type": "microsoft.graph.contentType" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },

  /* relationships */
  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },

  /* inherited from baseItem */
  "id": "string",
  "name": "name of resource",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "timestamp",
  "description": "description of resource",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "timestamp",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="b7e69-128">属性</span><span class="sxs-lookup"><span data-stu-id="b7e69-128">Properties</span></span>

<span data-ttu-id="b7e69-129">**listItem** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="b7e69-129">The **listItem** resource has the following properties.</span></span>

| <span data-ttu-id="b7e69-130">属性名称</span><span class="sxs-lookup"><span data-stu-id="b7e69-130">Property name</span></span> | <span data-ttu-id="b7e69-131">类型</span><span class="sxs-lookup"><span data-stu-id="b7e69-131">Type</span></span>                | <span data-ttu-id="b7e69-132">说明</span><span class="sxs-lookup"><span data-stu-id="b7e69-132">Description</span></span>
|:--------------|:--------------------|:-------------------------------
| <span data-ttu-id="b7e69-133">contentType</span><span class="sxs-lookup"><span data-stu-id="b7e69-133">contentType</span></span>   | <span data-ttu-id="b7e69-134">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="b7e69-134">[contentTypeInfo][]</span></span> | <span data-ttu-id="b7e69-135">此列表项的内容类型</span><span class="sxs-lookup"><span data-stu-id="b7e69-135">The content type of this list item</span></span>
| <span data-ttu-id="b7e69-136">fields</span><span class="sxs-lookup"><span data-stu-id="b7e69-136">fields</span></span>        | <span data-ttu-id="b7e69-137">[fieldValueSet][]</span><span class="sxs-lookup"><span data-stu-id="b7e69-137">[fieldValueSet][]</span></span>   | <span data-ttu-id="b7e69-138">在此列表项上设置的列的值。</span><span class="sxs-lookup"><span data-stu-id="b7e69-138">The values of the columns set on this list item.</span></span>

<span data-ttu-id="b7e69-139">以下属性继承自 ** [baseItem][]**。</span><span class="sxs-lookup"><span data-stu-id="b7e69-139">The following properties are inherited from **[baseItem][]**.</span></span>

| <span data-ttu-id="b7e69-140">属性名称</span><span class="sxs-lookup"><span data-stu-id="b7e69-140">Property name</span></span>        | <span data-ttu-id="b7e69-141">类型</span><span class="sxs-lookup"><span data-stu-id="b7e69-141">Type</span></span>             | <span data-ttu-id="b7e69-142">说明</span><span class="sxs-lookup"><span data-stu-id="b7e69-142">Description</span></span>
|:---------------------|:-----------------|:-----------------------------------
| <span data-ttu-id="b7e69-143">id</span><span class="sxs-lookup"><span data-stu-id="b7e69-143">id</span></span>                   | <span data-ttu-id="b7e69-144">string</span><span class="sxs-lookup"><span data-stu-id="b7e69-144">string</span></span>           | <span data-ttu-id="b7e69-p103">项的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="b7e69-p103">The unique identifier of the item. Read-only.</span></span>
| <span data-ttu-id="b7e69-147">name</span><span class="sxs-lookup"><span data-stu-id="b7e69-147">name</span></span>                 | <span data-ttu-id="b7e69-148">string</span><span class="sxs-lookup"><span data-stu-id="b7e69-148">string</span></span>           | <span data-ttu-id="b7e69-149">项目名称/标题。</span><span class="sxs-lookup"><span data-stu-id="b7e69-149">The name / title of the item.</span></span>
| <span data-ttu-id="b7e69-150">createdBy</span><span class="sxs-lookup"><span data-stu-id="b7e69-150">createdBy</span></span>            | <span data-ttu-id="b7e69-151">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b7e69-151">[identitySet][]</span></span>  | <span data-ttu-id="b7e69-152">此项的创建者的标识。</span><span class="sxs-lookup"><span data-stu-id="b7e69-152">Identity of the creator of this item.</span></span> <span data-ttu-id="b7e69-153">只读。</span><span class="sxs-lookup"><span data-stu-id="b7e69-153">Read-only.</span></span>
| <span data-ttu-id="b7e69-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7e69-154">createdDateTime</span></span>      | <span data-ttu-id="b7e69-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7e69-155">DateTimeOffset</span></span>   | <span data-ttu-id="b7e69-p105">创建项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="b7e69-p105">The date and time the item was created. Read-only.</span></span>
| <span data-ttu-id="b7e69-158">description</span><span class="sxs-lookup"><span data-stu-id="b7e69-158">description</span></span>          | <span data-ttu-id="b7e69-159">string</span><span class="sxs-lookup"><span data-stu-id="b7e69-159">string</span></span>           | <span data-ttu-id="b7e69-160">项目的描述性文本。</span><span class="sxs-lookup"><span data-stu-id="b7e69-160">The descriptive text for the site.</span></span>
| <span data-ttu-id="b7e69-161">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b7e69-161">lastModifiedBy</span></span>       | <span data-ttu-id="b7e69-162">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b7e69-162">[identitySet][]</span></span>  | <span data-ttu-id="b7e69-163">此项的最后一个修饰符的标识。</span><span class="sxs-lookup"><span data-stu-id="b7e69-163">Identity of the last modifier of this item.</span></span> <span data-ttu-id="b7e69-164">只读。</span><span class="sxs-lookup"><span data-stu-id="b7e69-164">Read-only.</span></span>
| <span data-ttu-id="b7e69-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7e69-165">lastModifiedDateTime</span></span> | <span data-ttu-id="b7e69-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7e69-166">DateTimeOffset</span></span>   | <span data-ttu-id="b7e69-p107">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="b7e69-p107">The date and time the item was last modified. Read-only.</span></span>
| <span data-ttu-id="b7e69-169">WebUrl</span><span class="sxs-lookup"><span data-stu-id="b7e69-169">webUrl</span></span>               | <span data-ttu-id="b7e69-170">string (url)</span><span class="sxs-lookup"><span data-stu-id="b7e69-170">string (url)</span></span>     | <span data-ttu-id="b7e69-p108">在浏览器中显示此项目的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="b7e69-p108">URL that displays the item in the browser. Read-only.</span></span>

## <a name="relationships"></a><span data-ttu-id="b7e69-173">关系</span><span class="sxs-lookup"><span data-stu-id="b7e69-173">Relationships</span></span>

 <span data-ttu-id="b7e69-174">**listItem** 资源与其他资源具有以下关系。</span><span class="sxs-lookup"><span data-stu-id="b7e69-174">The **listItem** resource has the following relationships to other resources.</span></span>

| <span data-ttu-id="b7e69-175">关系名称</span><span class="sxs-lookup"><span data-stu-id="b7e69-175">Relationship name</span></span> | <span data-ttu-id="b7e69-176">类型</span><span class="sxs-lookup"><span data-stu-id="b7e69-176">Type</span></span>                        | <span data-ttu-id="b7e69-177">说明</span><span class="sxs-lookup"><span data-stu-id="b7e69-177">Description</span></span>
|:------------------|:----------------------------|:-------------------------------
| <span data-ttu-id="b7e69-178">driveItem</span><span class="sxs-lookup"><span data-stu-id="b7e69-178">driveItem</span></span>         | <span data-ttu-id="b7e69-179">[driveItem][]</span><span class="sxs-lookup"><span data-stu-id="b7e69-179">[driveItem][]</span></span>               | <span data-ttu-id="b7e69-180">对于文档库，**driveItem** 关系将 **listItem[ 显示为 ][]driveItem**。</span><span class="sxs-lookup"><span data-stu-id="b7e69-180">For document libraries, the **driveItem** relationship exposes the listItem as a **[driveItem][]**</span></span>

[baseItem]: baseItem.md
[contentTypeInfo]: contentTypeInfo.md
[driveItem]: driveItem.md
[fieldValueSet]: fieldValueSet.md
[identitySet]: identitySet.md
[list]: list.md

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
