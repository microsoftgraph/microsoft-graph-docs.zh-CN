---
author: JeremyKelley
description: 下面是 columnDefinition 资源的 JSON 表示形式。
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: aab34ebe8a0cb7539775ba3e7b07e8ad7b3c357b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444334"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="2fc30-103">columnDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="2fc30-103">columnDefinition resource type</span></span>

<span data-ttu-id="2fc30-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fc30-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="2fc30-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2fc30-105">JSON representation</span></span>

<span data-ttu-id="2fc30-106">下面是 columnDefinition 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fc30-106">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="2fc30-107">属性</span><span class="sxs-lookup"><span data-stu-id="2fc30-107">Properties</span></span>

<span data-ttu-id="2fc30-108">列可以包含各种类型的数据。</span><span class="sxs-lookup"><span data-stu-id="2fc30-108">Columns can hold data of various types.</span></span>
<span data-ttu-id="2fc30-109">以下属性表示列存储的数据类型以及该数据的其他设置。</span><span class="sxs-lookup"><span data-stu-id="2fc30-109">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="2fc30-110">与类型相关的属性 (布尔、计算、选择、货币、dateTime、lookup、number、personOrGroup、text) 相互排斥 - 列只能指定其中一个。</span><span class="sxs-lookup"><span data-stu-id="2fc30-110">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="2fc30-111">属性名称</span><span class="sxs-lookup"><span data-stu-id="2fc30-111">Property name</span></span>           | <span data-ttu-id="2fc30-112">类型</span><span class="sxs-lookup"><span data-stu-id="2fc30-112">Type</span></span>    | <span data-ttu-id="2fc30-113">说明</span><span class="sxs-lookup"><span data-stu-id="2fc30-113">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="2fc30-114">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="2fc30-114">**columnGroup**</span></span>         | <span data-ttu-id="2fc30-115">string</span><span class="sxs-lookup"><span data-stu-id="2fc30-115">string</span></span>  | <span data-ttu-id="2fc30-116">对于网站列，此列所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="2fc30-116">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="2fc30-117">可以帮助组织相关的列。</span><span class="sxs-lookup"><span data-stu-id="2fc30-117">Helps organize related columns.</span></span>
| <span data-ttu-id="2fc30-118">**说明**</span><span class="sxs-lookup"><span data-stu-id="2fc30-118">**description**</span></span>         | <span data-ttu-id="2fc30-119">string</span><span class="sxs-lookup"><span data-stu-id="2fc30-119">string</span></span>  | <span data-ttu-id="2fc30-120">面向用户的列描述。</span><span class="sxs-lookup"><span data-stu-id="2fc30-120">The user-facing description of the column.</span></span>
| <span data-ttu-id="2fc30-121">**displayName**</span><span class="sxs-lookup"><span data-stu-id="2fc30-121">**displayName**</span></span>         | <span data-ttu-id="2fc30-122">string</span><span class="sxs-lookup"><span data-stu-id="2fc30-122">string</span></span>  | <span data-ttu-id="2fc30-123">面向用户的列名称。</span><span class="sxs-lookup"><span data-stu-id="2fc30-123">The user-facing name of the column.</span></span>
| <span data-ttu-id="2fc30-124">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="2fc30-124">**enforceUniqueValues**</span></span> | <span data-ttu-id="2fc30-125">布尔</span><span class="sxs-lookup"><span data-stu-id="2fc30-125">Boolean</span></span> | <span data-ttu-id="2fc30-126">如果为 true，则此列不能有两个列表项具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="2fc30-126">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="2fc30-127">**hidden**</span><span class="sxs-lookup"><span data-stu-id="2fc30-127">**hidden**</span></span>              | <span data-ttu-id="2fc30-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="2fc30-128">Boolean</span></span> | <span data-ttu-id="2fc30-129">指定列是否显示在用户界面中。</span><span class="sxs-lookup"><span data-stu-id="2fc30-129">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="2fc30-130">**id**</span><span class="sxs-lookup"><span data-stu-id="2fc30-130">**id**</span></span>                  | <span data-ttu-id="2fc30-131">string</span><span class="sxs-lookup"><span data-stu-id="2fc30-131">string</span></span>  | <span data-ttu-id="2fc30-132">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2fc30-132">The unique identifier for the column.</span></span>
| <span data-ttu-id="2fc30-133">**indexed**</span><span class="sxs-lookup"><span data-stu-id="2fc30-133">**indexed**</span></span>             | <span data-ttu-id="2fc30-134">布尔</span><span class="sxs-lookup"><span data-stu-id="2fc30-134">Boolean</span></span> | <span data-ttu-id="2fc30-135">指定列值是否可用于排序和搜索。</span><span class="sxs-lookup"><span data-stu-id="2fc30-135">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="2fc30-136">**名称**</span><span class="sxs-lookup"><span data-stu-id="2fc30-136">**name**</span></span>                | <span data-ttu-id="2fc30-137">string</span><span class="sxs-lookup"><span data-stu-id="2fc30-137">string</span></span>  | <span data-ttu-id="2fc30-138">在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。</span><span class="sxs-lookup"><span data-stu-id="2fc30-138">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="2fc30-139">对于面向用户的名称，请参阅 **displayName**。</span><span class="sxs-lookup"><span data-stu-id="2fc30-139">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="2fc30-140">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="2fc30-140">**readOnly**</span></span>            | <span data-ttu-id="2fc30-141">布尔</span><span class="sxs-lookup"><span data-stu-id="2fc30-141">Boolean</span></span>    | <span data-ttu-id="2fc30-142">指定是否可以修改列值。</span><span class="sxs-lookup"><span data-stu-id="2fc30-142">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="2fc30-143">**required**</span><span class="sxs-lookup"><span data-stu-id="2fc30-143">**required**</span></span>            | <span data-ttu-id="2fc30-144">布尔</span><span class="sxs-lookup"><span data-stu-id="2fc30-144">Boolean</span></span> | <span data-ttu-id="2fc30-145">指定列值是否不可选。</span><span class="sxs-lookup"><span data-stu-id="2fc30-145">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="2fc30-146">**boolean**</span><span class="sxs-lookup"><span data-stu-id="2fc30-146">**boolean**</span></span>       | <span data-ttu-id="2fc30-147">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-147">[booleanColumn][]</span></span>       | <span data-ttu-id="2fc30-148">此列存储布尔值。</span><span class="sxs-lookup"><span data-stu-id="2fc30-148">This column stores boolean values.</span></span>
| <span data-ttu-id="2fc30-149">**calculated**</span><span class="sxs-lookup"><span data-stu-id="2fc30-149">**calculated**</span></span>    | <span data-ttu-id="2fc30-150">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-150">[calculatedColumn][]</span></span>    | <span data-ttu-id="2fc30-151">根据其他列计算此列的数据。</span><span class="sxs-lookup"><span data-stu-id="2fc30-151">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="2fc30-152">**choice**</span><span class="sxs-lookup"><span data-stu-id="2fc30-152">**choice**</span></span>        | <span data-ttu-id="2fc30-153">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-153">[choiceColumn][]</span></span>        | <span data-ttu-id="2fc30-154">此列存储所选列表中的数据。</span><span class="sxs-lookup"><span data-stu-id="2fc30-154">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="2fc30-155">**currency**</span><span class="sxs-lookup"><span data-stu-id="2fc30-155">**currency**</span></span>      | <span data-ttu-id="2fc30-156">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-156">[currencyColumn][]</span></span>      | <span data-ttu-id="2fc30-157">此列存储货币值。</span><span class="sxs-lookup"><span data-stu-id="2fc30-157">This column stores currency values.</span></span>
| <span data-ttu-id="2fc30-158">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="2fc30-158">**dateTime**</span></span>      | <span data-ttu-id="2fc30-159">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-159">[dateTimeColumn][]</span></span>      | <span data-ttu-id="2fc30-160">此列存储日期时间值。</span><span class="sxs-lookup"><span data-stu-id="2fc30-160">This column stores DateTime values.</span></span>
| <span data-ttu-id="2fc30-161">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="2fc30-161">**defaultValue**</span></span>  | <span data-ttu-id="2fc30-162">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-162">[defaultColumnValue][]</span></span>  | <span data-ttu-id="2fc30-163">此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="2fc30-163">The default value for this column.</span></span>
| <span data-ttu-id="2fc30-164">**geolocation**</span><span class="sxs-lookup"><span data-stu-id="2fc30-164">**geolocation**</span></span>   | <span data-ttu-id="2fc30-165">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-165">[geolocationColumn][]</span></span>   | <span data-ttu-id="2fc30-166">此列存储地理位置。</span><span class="sxs-lookup"><span data-stu-id="2fc30-166">This column stores a geolocation.</span></span>
| <span data-ttu-id="2fc30-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="2fc30-167">**lookup**</span></span>        | <span data-ttu-id="2fc30-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-168">[lookupColumn][]</span></span>        | <span data-ttu-id="2fc30-169">从网站中的另一个源查找此列的数据。</span><span class="sxs-lookup"><span data-stu-id="2fc30-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="2fc30-170">**number**</span><span class="sxs-lookup"><span data-stu-id="2fc30-170">**number**</span></span>        | <span data-ttu-id="2fc30-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-171">[numberColumn][]</span></span>        | <span data-ttu-id="2fc30-172">此列存储数值。</span><span class="sxs-lookup"><span data-stu-id="2fc30-172">This column stores number values.</span></span>
| <span data-ttu-id="2fc30-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="2fc30-173">**personOrGroup**</span></span> | <span data-ttu-id="2fc30-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="2fc30-175">此列存储个人或组值。</span><span class="sxs-lookup"><span data-stu-id="2fc30-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="2fc30-176">**text**</span><span class="sxs-lookup"><span data-stu-id="2fc30-176">**text**</span></span>          | <span data-ttu-id="2fc30-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-177">[textColumn][]</span></span>          | <span data-ttu-id="2fc30-178">此列存储文本值。</span><span class="sxs-lookup"><span data-stu-id="2fc30-178">This column stores text values.</span></span>
| <span data-ttu-id="2fc30-179">**isDeletable**</span><span class="sxs-lookup"><span data-stu-id="2fc30-179">**isDeletable**</span></span>       | <span data-ttu-id="2fc30-180">布尔</span><span class="sxs-lookup"><span data-stu-id="2fc30-180">Boolean</span></span> | <span data-ttu-id="2fc30-181">指示是否可以删除此列。</span><span class="sxs-lookup"><span data-stu-id="2fc30-181">Indicates whether this column can be deleted.</span></span>
| <span data-ttu-id="2fc30-182">**propagateChanges**</span><span class="sxs-lookup"><span data-stu-id="2fc30-182">**propagateChanges**</span></span>     | <span data-ttu-id="2fc30-183">布尔</span><span class="sxs-lookup"><span data-stu-id="2fc30-183">Boolean</span></span> | <span data-ttu-id="2fc30-184">如果为"True"，则对此列所做的更改将传播到实现该列的列表。</span><span class="sxs-lookup"><span data-stu-id="2fc30-184">If 'True' changes to this column will be propagated to lists that implement the column.</span></span> 
| <span data-ttu-id="2fc30-185">**isReorderable**</span><span class="sxs-lookup"><span data-stu-id="2fc30-185">**isReorderable**</span></span>         | <span data-ttu-id="2fc30-186">布尔</span><span class="sxs-lookup"><span data-stu-id="2fc30-186">Boolean</span></span> | <span data-ttu-id="2fc30-187">指示是否可以对列中的值进行重新排序。</span><span class="sxs-lookup"><span data-stu-id="2fc30-187">Indicates whether values in the column can be reordered.</span></span> <span data-ttu-id="2fc30-188">只读。</span><span class="sxs-lookup"><span data-stu-id="2fc30-188">Read-only.</span></span>
| <span data-ttu-id="2fc30-189">**isSealed**</span><span class="sxs-lookup"><span data-stu-id="2fc30-189">**isSealed**</span></span>              | <span data-ttu-id="2fc30-190">布尔</span><span class="sxs-lookup"><span data-stu-id="2fc30-190">Boolean</span></span> | <span data-ttu-id="2fc30-191">指定是否可以更改列。</span><span class="sxs-lookup"><span data-stu-id="2fc30-191">Specifies whether column can be changed.</span></span>
| <span data-ttu-id="2fc30-192">**validation**</span><span class="sxs-lookup"><span data-stu-id="2fc30-192">**validation**</span></span>   |  <span data-ttu-id="2fc30-193">[columnValidation][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-193">[columnValidation][]</span></span>    | <span data-ttu-id="2fc30-194">此列存储该列的验证公式和消息。</span><span class="sxs-lookup"><span data-stu-id="2fc30-194">This column stores validation formula and message for the column.</span></span> 
| <span data-ttu-id="2fc30-195">**hyperlinkOrPicture**</span><span class="sxs-lookup"><span data-stu-id="2fc30-195">**hyperlinkOrPicture**</span></span>  | <span data-ttu-id="2fc30-196">[hyperlinkOrPictureColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-196">[hyperlinkOrPictureColumn][]</span></span> | <span data-ttu-id="2fc30-197">此列存储超链接或图片值。</span><span class="sxs-lookup"><span data-stu-id="2fc30-197">This column stores hyperlink or picture values.</span></span> 
| <span data-ttu-id="2fc30-198">**term**</span><span class="sxs-lookup"><span data-stu-id="2fc30-198">**term**</span></span>     | <span data-ttu-id="2fc30-199">[termColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-199">[termColumn][]</span></span> | <span data-ttu-id="2fc30-200">此列存储分类术语。</span><span class="sxs-lookup"><span data-stu-id="2fc30-200">This column stores taxonomy terms.</span></span>
| <span data-ttu-id="2fc30-201">**sourceContentType**</span><span class="sxs-lookup"><span data-stu-id="2fc30-201">**sourceContentType**</span></span>   |<span data-ttu-id="2fc30-202">[contentTypeInfo][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-202">[contentTypeInfo][]</span></span>  | <span data-ttu-id="2fc30-203">继承此列的 ContentType。</span><span class="sxs-lookup"><span data-stu-id="2fc30-203">ContentType from which this column is inherited from.</span></span> <span data-ttu-id="2fc30-204">仅在提取 contentTypes 列时使用。</span><span class="sxs-lookup"><span data-stu-id="2fc30-204">Used only while fetching contentTypes columns.</span></span>
| <span data-ttu-id="2fc30-205">**thumbnail**</span><span class="sxs-lookup"><span data-stu-id="2fc30-205">**thumbnail**</span></span>           |<span data-ttu-id="2fc30-206">[thumbnailColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-206">[thumbnailColumn][]</span></span>      | <span data-ttu-id="2fc30-207">此列存储缩略图值。</span><span class="sxs-lookup"><span data-stu-id="2fc30-207">This column stores thumbnail values.</span></span>
| <span data-ttu-id="2fc30-208">**type**</span><span class="sxs-lookup"><span data-stu-id="2fc30-208">**type**</span></span>         | <span data-ttu-id="2fc30-209">columnTypes</span><span class="sxs-lookup"><span data-stu-id="2fc30-209">columnTypes</span></span>  | <span data-ttu-id="2fc30-210">对于网站栏，列的类型。</span><span class="sxs-lookup"><span data-stu-id="2fc30-210">For site columns, the type of column.</span></span> <span data-ttu-id="2fc30-211">只读</span><span class="sxs-lookup"><span data-stu-id="2fc30-211">Read-only</span></span>
| <span data-ttu-id="2fc30-212">**contentApprovalStatus**</span><span class="sxs-lookup"><span data-stu-id="2fc30-212">**contentApprovalStatus**</span></span>| <span data-ttu-id="2fc30-213">[contentApprovalStatusColumn][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-213">[contentApprovalStatusColumn][]</span></span>     | <span data-ttu-id="2fc30-214">此列存储内容审批状态。</span><span class="sxs-lookup"><span data-stu-id="2fc30-214">This column stores content approval status.</span></span>

## <a name="relationships"></a><span data-ttu-id="2fc30-215">关系</span><span class="sxs-lookup"><span data-stu-id="2fc30-215">Relationships</span></span>

| <span data-ttu-id="2fc30-216">属性名称</span><span class="sxs-lookup"><span data-stu-id="2fc30-216">Property name</span></span>   | <span data-ttu-id="2fc30-217">类型</span><span class="sxs-lookup"><span data-stu-id="2fc30-217">Type</span></span>                      | <span data-ttu-id="2fc30-218">说明</span><span class="sxs-lookup"><span data-stu-id="2fc30-218">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="2fc30-219">**sourceColumn**</span><span class="sxs-lookup"><span data-stu-id="2fc30-219">**sourceColumn**</span></span> | <span data-ttu-id="2fc30-220">[columnDefinition][]</span><span class="sxs-lookup"><span data-stu-id="2fc30-220">[columnDefinition][]</span></span> | <span data-ttu-id="2fc30-221">内容类型列的源列。</span><span class="sxs-lookup"><span data-stu-id="2fc30-221">The source column for content type column.</span></span>

><span data-ttu-id="2fc30-222">**注意：** 这些属性对应于 SharePoint 的 [SPFieldType][] 枚举。</span><span class="sxs-lookup"><span data-stu-id="2fc30-222">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="2fc30-223">虽然上表中显示了最常见的字段类型，但此 beta API 仍缺少一些。</span><span class="sxs-lookup"><span data-stu-id="2fc30-223">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="2fc30-224">在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。</span><span class="sxs-lookup"><span data-stu-id="2fc30-224">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="2fc30-225">备注</span><span class="sxs-lookup"><span data-stu-id="2fc30-225">Remarks</span></span>

<span data-ttu-id="2fc30-226">默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。</span><span class="sxs-lookup"><span data-stu-id="2fc30-226">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="2fc30-227">若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="2fc30-227">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="2fc30-228">若要在 [listItems][listItem] 上显示 **字段** 值时看到这些内容，请在 `$select` 语句中添加名称所需的列。</span><span class="sxs-lookup"><span data-stu-id="2fc30-228">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[columnDefinition]: columnDefinition.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
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

<span data-ttu-id="2fc30-249">
  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span><span class="sxs-lookup"><span data-stu-id="2fc30-249">[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span></span>

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