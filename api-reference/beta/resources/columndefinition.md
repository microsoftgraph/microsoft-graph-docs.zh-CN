---
author: JeremyKelley
description: 下面是 columnDefinition 资源的 JSON 表示形式。
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6b21ae8b85044ea1c0b9fef16c1bb7dd57487040
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033998"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="11eb1-103">columnDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="11eb1-103">columnDefinition resource type</span></span>

<span data-ttu-id="11eb1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11eb1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="11eb1-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11eb1-105">JSON representation</span></span>

<span data-ttu-id="11eb1-106">下面是 columnDefinition 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11eb1-106">Here is a JSON representation of a columnDefinition resource.</span></span>

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
  "enforceUniqueValues": "true",
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
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="11eb1-107">属性</span><span class="sxs-lookup"><span data-stu-id="11eb1-107">Properties</span></span>

<span data-ttu-id="11eb1-108">列可以包含各种类型的数据。</span><span class="sxs-lookup"><span data-stu-id="11eb1-108">Columns can hold data of various types.</span></span>
<span data-ttu-id="11eb1-109">以下属性表示列存储的数据类型以及该数据的其他设置。</span><span class="sxs-lookup"><span data-stu-id="11eb1-109">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="11eb1-110">与类型相关的属性 (boolean、计算、选择、货币、dateTime、lookup、number、personOrGroup、text) 相互排斥--列只能指定其中一个。</span><span class="sxs-lookup"><span data-stu-id="11eb1-110">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="11eb1-111">属性名</span><span class="sxs-lookup"><span data-stu-id="11eb1-111">Property name</span></span>           | <span data-ttu-id="11eb1-112">类型</span><span class="sxs-lookup"><span data-stu-id="11eb1-112">Type</span></span>    | <span data-ttu-id="11eb1-113">说明</span><span class="sxs-lookup"><span data-stu-id="11eb1-113">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="11eb1-114">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="11eb1-114">**columnGroup**</span></span>         | <span data-ttu-id="11eb1-115">string</span><span class="sxs-lookup"><span data-stu-id="11eb1-115">string</span></span>  | <span data-ttu-id="11eb1-116">对于网站列，此列所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="11eb1-116">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="11eb1-117">可以帮助组织相关的列。</span><span class="sxs-lookup"><span data-stu-id="11eb1-117">Helps organize related columns.</span></span>
| <span data-ttu-id="11eb1-118">**说明**</span><span class="sxs-lookup"><span data-stu-id="11eb1-118">**description**</span></span>         | <span data-ttu-id="11eb1-119">string</span><span class="sxs-lookup"><span data-stu-id="11eb1-119">string</span></span>  | <span data-ttu-id="11eb1-120">面向用户的列描述。</span><span class="sxs-lookup"><span data-stu-id="11eb1-120">The user-facing description of the column.</span></span>
| <span data-ttu-id="11eb1-121">**displayName**</span><span class="sxs-lookup"><span data-stu-id="11eb1-121">**displayName**</span></span>         | <span data-ttu-id="11eb1-122">string</span><span class="sxs-lookup"><span data-stu-id="11eb1-122">string</span></span>  | <span data-ttu-id="11eb1-123">面向用户的列名称。</span><span class="sxs-lookup"><span data-stu-id="11eb1-123">The user-facing name of the column.</span></span>
| <span data-ttu-id="11eb1-124">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="11eb1-124">**enforceUniqueValues**</span></span> | <span data-ttu-id="11eb1-125">boolean</span><span class="sxs-lookup"><span data-stu-id="11eb1-125">boolean</span></span> | <span data-ttu-id="11eb1-126">如果为 true，则此列不能有两个列表项具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="11eb1-126">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="11eb1-127">**hidden**</span><span class="sxs-lookup"><span data-stu-id="11eb1-127">**hidden**</span></span>              | <span data-ttu-id="11eb1-128">boolean</span><span class="sxs-lookup"><span data-stu-id="11eb1-128">boolean</span></span> | <span data-ttu-id="11eb1-129">指定列是否显示在用户界面中。</span><span class="sxs-lookup"><span data-stu-id="11eb1-129">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="11eb1-130">**id**</span><span class="sxs-lookup"><span data-stu-id="11eb1-130">**id**</span></span>                  | <span data-ttu-id="11eb1-131">string</span><span class="sxs-lookup"><span data-stu-id="11eb1-131">string</span></span>  | <span data-ttu-id="11eb1-132">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="11eb1-132">The unique identifier for the column.</span></span>
| <span data-ttu-id="11eb1-133">**indexed**</span><span class="sxs-lookup"><span data-stu-id="11eb1-133">**indexed**</span></span>             | <span data-ttu-id="11eb1-134">boolean</span><span class="sxs-lookup"><span data-stu-id="11eb1-134">boolean</span></span> | <span data-ttu-id="11eb1-135">指定列值是否可用于排序和搜索。</span><span class="sxs-lookup"><span data-stu-id="11eb1-135">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="11eb1-136">**name**</span><span class="sxs-lookup"><span data-stu-id="11eb1-136">**name**</span></span>                | <span data-ttu-id="11eb1-137">string</span><span class="sxs-lookup"><span data-stu-id="11eb1-137">string</span></span>  | <span data-ttu-id="11eb1-138">在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。</span><span class="sxs-lookup"><span data-stu-id="11eb1-138">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="11eb1-139">对于面向用户的名称，请参阅 **displayName**。</span><span class="sxs-lookup"><span data-stu-id="11eb1-139">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="11eb1-140">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="11eb1-140">**readOnly**</span></span>            | <span data-ttu-id="11eb1-141">bool</span><span class="sxs-lookup"><span data-stu-id="11eb1-141">bool</span></span>    | <span data-ttu-id="11eb1-142">指定是否可以修改列值。</span><span class="sxs-lookup"><span data-stu-id="11eb1-142">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="11eb1-143">**required**</span><span class="sxs-lookup"><span data-stu-id="11eb1-143">**required**</span></span>            | <span data-ttu-id="11eb1-144">boolean</span><span class="sxs-lookup"><span data-stu-id="11eb1-144">boolean</span></span> | <span data-ttu-id="11eb1-145">指定列值是否不可选。</span><span class="sxs-lookup"><span data-stu-id="11eb1-145">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="11eb1-146">**boolean**</span><span class="sxs-lookup"><span data-stu-id="11eb1-146">**boolean**</span></span>       | <span data-ttu-id="11eb1-147">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="11eb1-147">[booleanColumn][]</span></span>       | <span data-ttu-id="11eb1-148">此列存储布尔值。</span><span class="sxs-lookup"><span data-stu-id="11eb1-148">This column stores boolean values.</span></span>
| <span data-ttu-id="11eb1-149">**calculated**</span><span class="sxs-lookup"><span data-stu-id="11eb1-149">**calculated**</span></span>    | <span data-ttu-id="11eb1-150">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="11eb1-150">[calculatedColumn][]</span></span>    | <span data-ttu-id="11eb1-151">根据其他列计算此列的数据。</span><span class="sxs-lookup"><span data-stu-id="11eb1-151">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="11eb1-152">**choice**</span><span class="sxs-lookup"><span data-stu-id="11eb1-152">**choice**</span></span>        | <span data-ttu-id="11eb1-153">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="11eb1-153">[choiceColumn][]</span></span>        | <span data-ttu-id="11eb1-154">此列存储所选列表中的数据。</span><span class="sxs-lookup"><span data-stu-id="11eb1-154">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="11eb1-155">**currency**</span><span class="sxs-lookup"><span data-stu-id="11eb1-155">**currency**</span></span>      | <span data-ttu-id="11eb1-156">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="11eb1-156">[currencyColumn][]</span></span>      | <span data-ttu-id="11eb1-157">此列存储货币值。</span><span class="sxs-lookup"><span data-stu-id="11eb1-157">This column stores currency values.</span></span>
| <span data-ttu-id="11eb1-158">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="11eb1-158">**dateTime**</span></span>      | <span data-ttu-id="11eb1-159">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="11eb1-159">[dateTimeColumn][]</span></span>      | <span data-ttu-id="11eb1-160">此列存储日期时间值。</span><span class="sxs-lookup"><span data-stu-id="11eb1-160">This column stores DateTime values.</span></span>
| <span data-ttu-id="11eb1-161">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="11eb1-161">**defaultValue**</span></span>  | <span data-ttu-id="11eb1-162">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="11eb1-162">[defaultColumnValue][]</span></span>  | <span data-ttu-id="11eb1-163">此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="11eb1-163">The default value for this column.</span></span>
| <span data-ttu-id="11eb1-164">**地理位置**</span><span class="sxs-lookup"><span data-stu-id="11eb1-164">**geolocation**</span></span>   | <span data-ttu-id="11eb1-165">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="11eb1-165">[geolocationColumn][]</span></span>   | <span data-ttu-id="11eb1-166">此列存储一个地理位置。</span><span class="sxs-lookup"><span data-stu-id="11eb1-166">This column stores a geolocation.</span></span>
| <span data-ttu-id="11eb1-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="11eb1-167">**lookup**</span></span>        | <span data-ttu-id="11eb1-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="11eb1-168">[lookupColumn][]</span></span>        | <span data-ttu-id="11eb1-169">从网站中的另一个源查找此列的数据。</span><span class="sxs-lookup"><span data-stu-id="11eb1-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="11eb1-170">**number**</span><span class="sxs-lookup"><span data-stu-id="11eb1-170">**number**</span></span>        | <span data-ttu-id="11eb1-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="11eb1-171">[numberColumn][]</span></span>        | <span data-ttu-id="11eb1-172">此列存储数值。</span><span class="sxs-lookup"><span data-stu-id="11eb1-172">This column stores number values.</span></span>
| <span data-ttu-id="11eb1-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="11eb1-173">**personOrGroup**</span></span> | <span data-ttu-id="11eb1-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="11eb1-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="11eb1-175">此列存储个人或组值。</span><span class="sxs-lookup"><span data-stu-id="11eb1-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="11eb1-176">**text**</span><span class="sxs-lookup"><span data-stu-id="11eb1-176">**text**</span></span>          | <span data-ttu-id="11eb1-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="11eb1-177">[textColumn][]</span></span>          | <span data-ttu-id="11eb1-178">此列存储文本值。</span><span class="sxs-lookup"><span data-stu-id="11eb1-178">This column stores text values.</span></span>

><span data-ttu-id="11eb1-179">**注意：** 这些属性对应于 SharePoint 的 [SPFieldType][] 枚举。</span><span class="sxs-lookup"><span data-stu-id="11eb1-179">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="11eb1-180">虽然在上表中表示的是最常见的字段类型，但此 beta API 仍缺少一些。</span><span class="sxs-lookup"><span data-stu-id="11eb1-180">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="11eb1-181">在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。</span><span class="sxs-lookup"><span data-stu-id="11eb1-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="11eb1-182">备注</span><span class="sxs-lookup"><span data-stu-id="11eb1-182">Remarks</span></span>

<span data-ttu-id="11eb1-183">默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。</span><span class="sxs-lookup"><span data-stu-id="11eb1-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="11eb1-184">若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="11eb1-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="11eb1-185">若要在 [listItems][listItem] 上显示**字段**值时看到这些内容，请在 `$select` 语句中添加名称所需的列。</span><span class="sxs-lookup"><span data-stu-id="11eb1-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
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

<span data-ttu-id="11eb1-199">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="11eb1-199">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

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


