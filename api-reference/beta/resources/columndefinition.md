---
author: JeremyKelley
description: 下面是 columnDefinition 资源的 JSON 表示形式。
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: cddab6ee01cea34902ee892e593e0e81b3cde8af
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961298"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="f5462-103">columnDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5462-103">columnDefinition resource type</span></span>

<span data-ttu-id="f5462-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5462-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5462-105">表示网站、[列表或][] [contentType][][中的][]列。</span><span class="sxs-lookup"><span data-stu-id="f5462-105">Represents a column in a [site][], [list][] or [contentType][].</span></span>

## <a name="methods"></a><span data-ttu-id="f5462-106">Methods</span><span class="sxs-lookup"><span data-stu-id="f5462-106">Methods</span></span>
|<span data-ttu-id="f5462-107">方法</span><span class="sxs-lookup"><span data-stu-id="f5462-107">Method</span></span>|<span data-ttu-id="f5462-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f5462-108">Return type</span></span>|<span data-ttu-id="f5462-109">说明</span><span class="sxs-lookup"><span data-stu-id="f5462-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f5462-110">列出网站中的列</span><span class="sxs-lookup"><span data-stu-id="f5462-110">List columns in a site</span></span>](../api/site-list-columns.md)|<span data-ttu-id="f5462-111">[columnDefinition](../resources/columndefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5462-111">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="f5462-112">获取网站中的 [columnDefinition](../resources/columndefinition.md) 对象及其属性 [的列表](../resources/site.md)。</span><span class="sxs-lookup"><span data-stu-id="f5462-112">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="f5462-113">列出列表中的列</span><span class="sxs-lookup"><span data-stu-id="f5462-113">List columns in a list</span></span>](../api/list-list-columns.md)|<span data-ttu-id="f5462-114">[columnDefinition](../resources/columndefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5462-114">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="f5462-115">在列表中获取 [columnDefinition](../resources/columndefinition.md) 对象及其属性 [的列表](../resources/list.md)。</span><span class="sxs-lookup"><span data-stu-id="f5462-115">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="f5462-116">列出内容类型中的列</span><span class="sxs-lookup"><span data-stu-id="f5462-116">List columns in a content type</span></span>](../api/contenttype-list-columns.md)|<span data-ttu-id="f5462-117">[columnDefinition](../resources/columndefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5462-117">[columnDefinition](../resources/columndefinition.md) collection</span></span>|<span data-ttu-id="f5462-118">获取内容类型中的 [columnDefinition](../resources/columndefinition.md) 对象及其 [属性的列表](../resources/contenttype.md)。</span><span class="sxs-lookup"><span data-stu-id="f5462-118">Get a list of the [columnDefinition](../resources/columndefinition.md) objects and their properties in a [content type](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="f5462-119">为网站创建 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="f5462-119">Create columnDefinition for a site</span></span>](../api/site-post-columns.md)|[<span data-ttu-id="f5462-120">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="f5462-120">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="f5462-121">在网站 [中创建新的 columnDefinition](../resources/columndefinition.md) [对象](../resources/site.md)。</span><span class="sxs-lookup"><span data-stu-id="f5462-121">Create a new [columnDefinition](../resources/columndefinition.md) object in a [site](../resources/site.md).</span></span>|
|[<span data-ttu-id="f5462-122">为列表创建 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="f5462-122">Create columnDefinition for a list</span></span>](../api/list-post-columns.md)|[<span data-ttu-id="f5462-123">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="f5462-123">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="f5462-124">在列表中 [创建新的 columnDefinition](../resources/columndefinition.md) [对象](../resources/list.md)。</span><span class="sxs-lookup"><span data-stu-id="f5462-124">Create a new [columnDefinition](../resources/columndefinition.md) object in a [list](../resources/list.md).</span></span>|
|[<span data-ttu-id="f5462-125">为内容类型创建 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="f5462-125">Create columnDefinition for a content type</span></span>](../api/contenttype-post-columns.md)|[<span data-ttu-id="f5462-126">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="f5462-126">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="f5462-127">在内容类型 [中创建新的 columnDefinition](../resources/columndefinition.md) [对象](../resources/contenttype.md)。</span><span class="sxs-lookup"><span data-stu-id="f5462-127">Create a new [columnDefinition](../resources/columndefinition.md) object in a [content type](../resources/contenttype.md).</span></span>|
|[<span data-ttu-id="f5462-128">获取 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="f5462-128">Get columnDefinition</span></span>](../api/columndefinition-get.md)|[<span data-ttu-id="f5462-129">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="f5462-129">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="f5462-130">读取 [columnDefinition 对象的属性和](../resources/columndefinition.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="f5462-130">Read the properties and relationships of a [columnDefinition](../resources/columndefinition.md) object.</span></span>|
|[<span data-ttu-id="f5462-131">更新 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="f5462-131">Update columnDefinition</span></span>](../api/columndefinition-update.md)|[<span data-ttu-id="f5462-132">columnDefinition</span><span class="sxs-lookup"><span data-stu-id="f5462-132">columnDefinition</span></span>](../resources/columndefinition.md)|<span data-ttu-id="f5462-133">更新 [columnDefinition 对象](../resources/columndefinition.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f5462-133">Update the properties of a [columnDefinition](../resources/columndefinition.md) object.</span></span>|
|[<span data-ttu-id="f5462-134">删除 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="f5462-134">Delete columnDefinition</span></span>](../api/columndefinition-delete.md)|<span data-ttu-id="f5462-135">无</span><span class="sxs-lookup"><span data-stu-id="f5462-135">None</span></span>|<span data-ttu-id="f5462-136">删除 [columnDefinition](../resources/columndefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5462-136">Deletes a [columnDefinition](../resources/columndefinition.md) object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5462-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5462-137">JSON representation</span></span>

<span data-ttu-id="f5462-138">下面是 columnDefinition 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5462-138">Here is a JSON representation of a columnDefinition resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnDefinition"
}-->

```json
{
  "columnGroup": "string",
  "description": "description",
  "displayName": "friendly name",
  "enforceUniqueValues": true,
  "hidden": false,
  "id": "string",
  "indexed": true,
  "name": "staticNameForApi",
  "readOnly": false,
  "required": false,
  "boolean": { "@odata.type": "microsoft.graph.booleanColumn" },
  "calculated": { "@odata.type": "microsoft.graph.calculatedColumn" },
  "choice": { "@odata.type": "microsoft.graph.choiceColumn" },
  "currency": { "@odata.type": "microsoft.graph.currencyColumn" },
  "dateTime": { "@odata.type": "microsoft.graph.dateTimeColumn" },
  "defaultValue": { "@odata.type": "microsoft.graph.defaultColumnValue" },
  "geolocation": { "@odata.type": "microsoft.graph.geolocationColumn" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" },
  "isDeletable" : false,
  "propagateChanges": false,
  "isReorderable": false,
  "isSealed": false,
  "validation": { "@odata.type": "microsoft.graph.columnValidation" },
  "hyperlinkOrPicture": { "@odata.type": "microsoft.graph.hyperlinkOrPictureColumn" },
  "term": { "@odata.type": "microsoft.graph.termColumn" },
  "sourceContentType": { "@odata.type": "microsoft.graph.contentTypeInfo" },
  "thumbnail": { "@odata.type": "microsoft.graph.thumbnailColumn" },
  "type": { "@odata.type": "microsoft.graph.columnTypes" },
  "contentApprovalStatus": { "@odata.type": "microsoft.graph.contentApprovalStatusColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="f5462-139">属性</span><span class="sxs-lookup"><span data-stu-id="f5462-139">Properties</span></span>

<span data-ttu-id="f5462-140">列可以包含各种类型的数据。</span><span class="sxs-lookup"><span data-stu-id="f5462-140">Columns can hold data of various types.</span></span>
<span data-ttu-id="f5462-141">以下属性表示列存储的数据类型以及该数据的其他设置。</span><span class="sxs-lookup"><span data-stu-id="f5462-141">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="f5462-142">与类型相关的属性 (布尔、计算、选项、货币、dateTime、lookup、number、personOrGroup、text) 是互斥的 -列只能指定其中一个。</span><span class="sxs-lookup"><span data-stu-id="f5462-142">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="f5462-143">属性名称</span><span class="sxs-lookup"><span data-stu-id="f5462-143">Property name</span></span>           | <span data-ttu-id="f5462-144">类型</span><span class="sxs-lookup"><span data-stu-id="f5462-144">Type</span></span>    | <span data-ttu-id="f5462-145">说明</span><span class="sxs-lookup"><span data-stu-id="f5462-145">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="f5462-146">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="f5462-146">**columnGroup**</span></span>         | <span data-ttu-id="f5462-147">string</span><span class="sxs-lookup"><span data-stu-id="f5462-147">string</span></span>  | <span data-ttu-id="f5462-148">对于网站列，此列所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="f5462-148">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="f5462-149">可以帮助组织相关的列。</span><span class="sxs-lookup"><span data-stu-id="f5462-149">Helps organize related columns.</span></span>
| <span data-ttu-id="f5462-150">**说明**</span><span class="sxs-lookup"><span data-stu-id="f5462-150">**description**</span></span>         | <span data-ttu-id="f5462-151">string</span><span class="sxs-lookup"><span data-stu-id="f5462-151">string</span></span>  | <span data-ttu-id="f5462-152">面向用户的列描述。</span><span class="sxs-lookup"><span data-stu-id="f5462-152">The user-facing description of the column.</span></span>
| <span data-ttu-id="f5462-153">**displayName**</span><span class="sxs-lookup"><span data-stu-id="f5462-153">**displayName**</span></span>         | <span data-ttu-id="f5462-154">string</span><span class="sxs-lookup"><span data-stu-id="f5462-154">string</span></span>  | <span data-ttu-id="f5462-155">面向用户的列名称。</span><span class="sxs-lookup"><span data-stu-id="f5462-155">The user-facing name of the column.</span></span>
| <span data-ttu-id="f5462-156">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="f5462-156">**enforceUniqueValues**</span></span> | <span data-ttu-id="f5462-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5462-157">Boolean</span></span> | <span data-ttu-id="f5462-158">如果为 true，则此列不能有两个列表项具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="f5462-158">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="f5462-159">**hidden**</span><span class="sxs-lookup"><span data-stu-id="f5462-159">**hidden**</span></span>              | <span data-ttu-id="f5462-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5462-160">Boolean</span></span> | <span data-ttu-id="f5462-161">指定列是否显示在用户界面中。</span><span class="sxs-lookup"><span data-stu-id="f5462-161">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="f5462-162">**id**</span><span class="sxs-lookup"><span data-stu-id="f5462-162">**id**</span></span>                  | <span data-ttu-id="f5462-163">string</span><span class="sxs-lookup"><span data-stu-id="f5462-163">string</span></span>  | <span data-ttu-id="f5462-164">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f5462-164">The unique identifier for the column.</span></span>
| <span data-ttu-id="f5462-165">**indexed**</span><span class="sxs-lookup"><span data-stu-id="f5462-165">**indexed**</span></span>             | <span data-ttu-id="f5462-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5462-166">Boolean</span></span> | <span data-ttu-id="f5462-167">指定列值是否可用于排序和搜索。</span><span class="sxs-lookup"><span data-stu-id="f5462-167">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="f5462-168">**名称**</span><span class="sxs-lookup"><span data-stu-id="f5462-168">**name**</span></span>                | <span data-ttu-id="f5462-169">string</span><span class="sxs-lookup"><span data-stu-id="f5462-169">string</span></span>  | <span data-ttu-id="f5462-170">在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。</span><span class="sxs-lookup"><span data-stu-id="f5462-170">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="f5462-171">对于面向用户的名称，请参阅 **displayName**。</span><span class="sxs-lookup"><span data-stu-id="f5462-171">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="f5462-172">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="f5462-172">**readOnly**</span></span>            | <span data-ttu-id="f5462-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5462-173">Boolean</span></span>    | <span data-ttu-id="f5462-174">指定是否可以修改列值。</span><span class="sxs-lookup"><span data-stu-id="f5462-174">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="f5462-175">**required**</span><span class="sxs-lookup"><span data-stu-id="f5462-175">**required**</span></span>            | <span data-ttu-id="f5462-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5462-176">Boolean</span></span> | <span data-ttu-id="f5462-177">指定列值是否不可选。</span><span class="sxs-lookup"><span data-stu-id="f5462-177">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="f5462-178">**boolean**</span><span class="sxs-lookup"><span data-stu-id="f5462-178">**boolean**</span></span>       | <span data-ttu-id="f5462-179">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-179">[booleanColumn][]</span></span>       | <span data-ttu-id="f5462-180">此列存储布尔值。</span><span class="sxs-lookup"><span data-stu-id="f5462-180">This column stores boolean values.</span></span>
| <span data-ttu-id="f5462-181">**calculated**</span><span class="sxs-lookup"><span data-stu-id="f5462-181">**calculated**</span></span>    | <span data-ttu-id="f5462-182">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-182">[calculatedColumn][]</span></span>    | <span data-ttu-id="f5462-183">根据其他列计算此列的数据。</span><span class="sxs-lookup"><span data-stu-id="f5462-183">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="f5462-184">**choice**</span><span class="sxs-lookup"><span data-stu-id="f5462-184">**choice**</span></span>        | <span data-ttu-id="f5462-185">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-185">[choiceColumn][]</span></span>        | <span data-ttu-id="f5462-186">此列存储所选列表中的数据。</span><span class="sxs-lookup"><span data-stu-id="f5462-186">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="f5462-187">**currency**</span><span class="sxs-lookup"><span data-stu-id="f5462-187">**currency**</span></span>      | <span data-ttu-id="f5462-188">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-188">[currencyColumn][]</span></span>      | <span data-ttu-id="f5462-189">此列存储货币值。</span><span class="sxs-lookup"><span data-stu-id="f5462-189">This column stores currency values.</span></span>
| <span data-ttu-id="f5462-190">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="f5462-190">**dateTime**</span></span>      | <span data-ttu-id="f5462-191">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-191">[dateTimeColumn][]</span></span>      | <span data-ttu-id="f5462-192">此列存储日期时间值。</span><span class="sxs-lookup"><span data-stu-id="f5462-192">This column stores DateTime values.</span></span>
| <span data-ttu-id="f5462-193">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="f5462-193">**defaultValue**</span></span>  | <span data-ttu-id="f5462-194">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="f5462-194">[defaultColumnValue][]</span></span>  | <span data-ttu-id="f5462-195">此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="f5462-195">The default value for this column.</span></span>
| <span data-ttu-id="f5462-196">**地理位置**</span><span class="sxs-lookup"><span data-stu-id="f5462-196">**geolocation**</span></span>   | <span data-ttu-id="f5462-197">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-197">[geolocationColumn][]</span></span>   | <span data-ttu-id="f5462-198">此列存储地理位置。</span><span class="sxs-lookup"><span data-stu-id="f5462-198">This column stores a geolocation.</span></span>
| <span data-ttu-id="f5462-199">**lookup**</span><span class="sxs-lookup"><span data-stu-id="f5462-199">**lookup**</span></span>        | <span data-ttu-id="f5462-200">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-200">[lookupColumn][]</span></span>        | <span data-ttu-id="f5462-201">从网站中的另一个源查找此列的数据。</span><span class="sxs-lookup"><span data-stu-id="f5462-201">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="f5462-202">**number**</span><span class="sxs-lookup"><span data-stu-id="f5462-202">**number**</span></span>        | <span data-ttu-id="f5462-203">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-203">[numberColumn][]</span></span>        | <span data-ttu-id="f5462-204">此列存储数值。</span><span class="sxs-lookup"><span data-stu-id="f5462-204">This column stores number values.</span></span>
| <span data-ttu-id="f5462-205">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="f5462-205">**personOrGroup**</span></span> | <span data-ttu-id="f5462-206">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-206">[personOrGroupColumn][]</span></span> | <span data-ttu-id="f5462-207">此列存储个人或组值。</span><span class="sxs-lookup"><span data-stu-id="f5462-207">This column stores Person or Group values.</span></span>
| <span data-ttu-id="f5462-208">**text**</span><span class="sxs-lookup"><span data-stu-id="f5462-208">**text**</span></span>          | <span data-ttu-id="f5462-209">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-209">[textColumn][]</span></span>          | <span data-ttu-id="f5462-210">此列存储文本值。</span><span class="sxs-lookup"><span data-stu-id="f5462-210">This column stores text values.</span></span>
| <span data-ttu-id="f5462-211">**isDeletable**</span><span class="sxs-lookup"><span data-stu-id="f5462-211">**isDeletable**</span></span>       | <span data-ttu-id="f5462-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5462-212">Boolean</span></span> | <span data-ttu-id="f5462-213">指示是否可以删除此列。</span><span class="sxs-lookup"><span data-stu-id="f5462-213">Indicates whether this column can be deleted.</span></span>
| <span data-ttu-id="f5462-214">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="f5462-214">**propagateChanges**</span></span>     | <span data-ttu-id="f5462-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5462-215">Boolean</span></span> | <span data-ttu-id="f5462-216">如果"True"，则对此列所做的更改将传播到实现该列的列表。</span><span class="sxs-lookup"><span data-stu-id="f5462-216">If 'True' changes to this column will be propagated to lists that implement the column.</span></span> 
| <span data-ttu-id="f5462-217">**isReorderable**</span><span class="sxs-lookup"><span data-stu-id="f5462-217">**isReorderable**</span></span>         | <span data-ttu-id="f5462-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5462-218">Boolean</span></span> | <span data-ttu-id="f5462-219">指示是否可以对列中的值进行重新排序。</span><span class="sxs-lookup"><span data-stu-id="f5462-219">Indicates whether values in the column can be reordered.</span></span> <span data-ttu-id="f5462-220">只读。</span><span class="sxs-lookup"><span data-stu-id="f5462-220">Read-only.</span></span>
| <span data-ttu-id="f5462-221">**isSealed**</span><span class="sxs-lookup"><span data-stu-id="f5462-221">**isSealed**</span></span>              | <span data-ttu-id="f5462-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5462-222">Boolean</span></span> | <span data-ttu-id="f5462-223">指定是否可以更改列。</span><span class="sxs-lookup"><span data-stu-id="f5462-223">Specifies whether column can be changed.</span></span>
| <span data-ttu-id="f5462-224">**validation**</span><span class="sxs-lookup"><span data-stu-id="f5462-224">**validation**</span></span>   |  <span data-ttu-id="f5462-225">[columnValidation][]</span><span class="sxs-lookup"><span data-stu-id="f5462-225">[columnValidation][]</span></span>    | <span data-ttu-id="f5462-226">此列存储该列的验证公式和消息。</span><span class="sxs-lookup"><span data-stu-id="f5462-226">This column stores validation formula and message for the column.</span></span> 
| <span data-ttu-id="f5462-227">**hyperlinkOrPicture**</span><span class="sxs-lookup"><span data-stu-id="f5462-227">**hyperlinkOrPicture**</span></span>  | <span data-ttu-id="f5462-228">[hyperlinkOrPictureColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-228">[hyperlinkOrPictureColumn][]</span></span> | <span data-ttu-id="f5462-229">此列存储超链接或图片值。</span><span class="sxs-lookup"><span data-stu-id="f5462-229">This column stores hyperlink or picture values.</span></span> 
| <span data-ttu-id="f5462-230">**term**</span><span class="sxs-lookup"><span data-stu-id="f5462-230">**term**</span></span>     | <span data-ttu-id="f5462-231">[termColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-231">[termColumn][]</span></span> | <span data-ttu-id="f5462-232">此列存储分类术语。</span><span class="sxs-lookup"><span data-stu-id="f5462-232">This column stores taxonomy terms.</span></span>
| <span data-ttu-id="f5462-233">**sourceContentType**</span><span class="sxs-lookup"><span data-stu-id="f5462-233">**sourceContentType**</span></span>   |<span data-ttu-id="f5462-234">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="f5462-234">[contentTypeInfo][]</span></span>  | <span data-ttu-id="f5462-235">从其继承此列的 ContentType。</span><span class="sxs-lookup"><span data-stu-id="f5462-235">ContentType from which this column is inherited from.</span></span> <span data-ttu-id="f5462-236">仅在提取 contentTypes 列时使用。</span><span class="sxs-lookup"><span data-stu-id="f5462-236">Used only while fetching contentTypes columns.</span></span>
| <span data-ttu-id="f5462-237">**thumbnail**</span><span class="sxs-lookup"><span data-stu-id="f5462-237">**thumbnail**</span></span>           |<span data-ttu-id="f5462-238">[thumbnailColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-238">[thumbnailColumn][]</span></span>      | <span data-ttu-id="f5462-239">此列存储缩略图值。</span><span class="sxs-lookup"><span data-stu-id="f5462-239">This column stores thumbnail values.</span></span>
| <span data-ttu-id="f5462-240">**类型**</span><span class="sxs-lookup"><span data-stu-id="f5462-240">**type**</span></span>         | <span data-ttu-id="f5462-241">columnTypes</span><span class="sxs-lookup"><span data-stu-id="f5462-241">columnTypes</span></span>  | <span data-ttu-id="f5462-242">对于网站栏，列的类型。</span><span class="sxs-lookup"><span data-stu-id="f5462-242">For site columns, the type of column.</span></span> <span data-ttu-id="f5462-243">只读</span><span class="sxs-lookup"><span data-stu-id="f5462-243">Read-only</span></span>
| <span data-ttu-id="f5462-244">**contentApprovalStatus**</span><span class="sxs-lookup"><span data-stu-id="f5462-244">**contentApprovalStatus**</span></span>| <span data-ttu-id="f5462-245">[contentApprovalStatusColumn][]</span><span class="sxs-lookup"><span data-stu-id="f5462-245">[contentApprovalStatusColumn][]</span></span>     | <span data-ttu-id="f5462-246">此列存储内容审批状态。</span><span class="sxs-lookup"><span data-stu-id="f5462-246">This column stores content approval status.</span></span>

## <a name="relationships"></a><span data-ttu-id="f5462-247">关系</span><span class="sxs-lookup"><span data-stu-id="f5462-247">Relationships</span></span>

| <span data-ttu-id="f5462-248">属性名称</span><span class="sxs-lookup"><span data-stu-id="f5462-248">Property name</span></span>   | <span data-ttu-id="f5462-249">类型</span><span class="sxs-lookup"><span data-stu-id="f5462-249">Type</span></span>                      | <span data-ttu-id="f5462-250">说明</span><span class="sxs-lookup"><span data-stu-id="f5462-250">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="f5462-251">**sourceColumn**</span><span class="sxs-lookup"><span data-stu-id="f5462-251">**sourceColumn**</span></span> | <span data-ttu-id="f5462-252">[columnDefinition][]</span><span class="sxs-lookup"><span data-stu-id="f5462-252">[columnDefinition][]</span></span> | <span data-ttu-id="f5462-253">内容类型列的源列。</span><span class="sxs-lookup"><span data-stu-id="f5462-253">The source column for content type column.</span></span>

><span data-ttu-id="f5462-254">**注意：** 这些属性对应于 SharePoint 的 [SPFieldType][] 枚举。</span><span class="sxs-lookup"><span data-stu-id="f5462-254">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="f5462-255">虽然上表中显示了最常见的字段类型，但此 beta API 仍缺少一些。</span><span class="sxs-lookup"><span data-stu-id="f5462-255">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="f5462-256">在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。</span><span class="sxs-lookup"><span data-stu-id="f5462-256">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="f5462-257">备注</span><span class="sxs-lookup"><span data-stu-id="f5462-257">Remarks</span></span>

<span data-ttu-id="f5462-258">默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。</span><span class="sxs-lookup"><span data-stu-id="f5462-258">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="f5462-259">若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="f5462-259">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="f5462-260">若要在 [listItems][listItem] 上显示 **字段** 值时看到这些内容，请在 `$select` 语句中添加名称所需的列。</span><span class="sxs-lookup"><span data-stu-id="f5462-260">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[columnDefinition]: columnDefinition.md
[contentType]: contenttype.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[列表]: list.md
[list]: list.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[site]: site.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md
[termColumn]: termColumn.md
[contentApprovalStatusColumn]: contentApprovalStatusColumn.md
[thumbnailColumn]: thumbnailColumn.md
[hyperlinkOrPictureColumn]: hyperlinkOrPictureColumn.md
[columnValidation]: columnValidation.md
[contentTypeInfo]: contentTypeInfo.md

<span data-ttu-id="f5462-284">
  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span><span class="sxs-lookup"><span data-stu-id="f5462-284">[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": []
}
-->