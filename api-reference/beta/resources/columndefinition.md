---
author: JeremyKelley
description: 下面是 columnDefinition 资源的 JSON 表示形式。
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7f60d33f8fbfe76c9dfd0ca02c98df96ca6ab380
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973291"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="18d92-103">columnDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="18d92-103">columnDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="18d92-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18d92-104">JSON representation</span></span>

<span data-ttu-id="18d92-105">下面是 columnDefinition 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18d92-105">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="18d92-106">属性</span><span class="sxs-lookup"><span data-stu-id="18d92-106">Properties</span></span>

<span data-ttu-id="18d92-107">列可以包含各种类型的数据。</span><span class="sxs-lookup"><span data-stu-id="18d92-107">Columns can hold data of various types.</span></span>
<span data-ttu-id="18d92-108">以下属性表示列存储的数据类型以及该数据的其他设置。</span><span class="sxs-lookup"><span data-stu-id="18d92-108">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="18d92-109">与类型相关的属性 (boolean、计算、choice、currency、dateTime、lookup、number、personOrGroup、text) 是相互排斥的--一个列只能有一个指定的属性。</span><span class="sxs-lookup"><span data-stu-id="18d92-109">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="18d92-110">属性名</span><span class="sxs-lookup"><span data-stu-id="18d92-110">Property name</span></span>           | <span data-ttu-id="18d92-111">类型</span><span class="sxs-lookup"><span data-stu-id="18d92-111">Type</span></span>    | <span data-ttu-id="18d92-112">说明</span><span class="sxs-lookup"><span data-stu-id="18d92-112">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="18d92-113">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="18d92-113">**columnGroup**</span></span>         | <span data-ttu-id="18d92-114">string</span><span class="sxs-lookup"><span data-stu-id="18d92-114">string</span></span>  | <span data-ttu-id="18d92-115">对于网站列，此列所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="18d92-115">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="18d92-116">可以帮助组织相关的列。</span><span class="sxs-lookup"><span data-stu-id="18d92-116">Helps organize related columns.</span></span>
| <span data-ttu-id="18d92-117">**说明**</span><span class="sxs-lookup"><span data-stu-id="18d92-117">**description**</span></span>         | <span data-ttu-id="18d92-118">string</span><span class="sxs-lookup"><span data-stu-id="18d92-118">string</span></span>  | <span data-ttu-id="18d92-119">面向用户的列描述。</span><span class="sxs-lookup"><span data-stu-id="18d92-119">The user-facing description of the column.</span></span>
| <span data-ttu-id="18d92-120">**displayName**</span><span class="sxs-lookup"><span data-stu-id="18d92-120">**displayName**</span></span>         | <span data-ttu-id="18d92-121">string</span><span class="sxs-lookup"><span data-stu-id="18d92-121">string</span></span>  | <span data-ttu-id="18d92-122">面向用户的列名称。</span><span class="sxs-lookup"><span data-stu-id="18d92-122">The user-facing name of the column.</span></span>
| <span data-ttu-id="18d92-123">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="18d92-123">**enforceUniqueValues**</span></span> | <span data-ttu-id="18d92-124">boolean</span><span class="sxs-lookup"><span data-stu-id="18d92-124">boolean</span></span> | <span data-ttu-id="18d92-125">如果为 true，则此列不能有两个列表项具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="18d92-125">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="18d92-126">**hidden**</span><span class="sxs-lookup"><span data-stu-id="18d92-126">**hidden**</span></span>              | <span data-ttu-id="18d92-127">boolean</span><span class="sxs-lookup"><span data-stu-id="18d92-127">boolean</span></span> | <span data-ttu-id="18d92-128">指定列是否显示在用户界面中。</span><span class="sxs-lookup"><span data-stu-id="18d92-128">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="18d92-129">**id**</span><span class="sxs-lookup"><span data-stu-id="18d92-129">**id**</span></span>                  | <span data-ttu-id="18d92-130">string</span><span class="sxs-lookup"><span data-stu-id="18d92-130">string</span></span>  | <span data-ttu-id="18d92-131">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="18d92-131">The unique identifier for the column.</span></span>
| <span data-ttu-id="18d92-132">**indexed**</span><span class="sxs-lookup"><span data-stu-id="18d92-132">**indexed**</span></span>             | <span data-ttu-id="18d92-133">boolean</span><span class="sxs-lookup"><span data-stu-id="18d92-133">boolean</span></span> | <span data-ttu-id="18d92-134">指定列值是否可用于排序和搜索。</span><span class="sxs-lookup"><span data-stu-id="18d92-134">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="18d92-135">**name**</span><span class="sxs-lookup"><span data-stu-id="18d92-135">**name**</span></span>                | <span data-ttu-id="18d92-136">string</span><span class="sxs-lookup"><span data-stu-id="18d92-136">string</span></span>  | <span data-ttu-id="18d92-137">在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。</span><span class="sxs-lookup"><span data-stu-id="18d92-137">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="18d92-138">对于面向用户的名称，请参阅 **displayName**。</span><span class="sxs-lookup"><span data-stu-id="18d92-138">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="18d92-139">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="18d92-139">**readOnly**</span></span>            | <span data-ttu-id="18d92-140">bool</span><span class="sxs-lookup"><span data-stu-id="18d92-140">bool</span></span>    | <span data-ttu-id="18d92-141">指定是否可以修改列值。</span><span class="sxs-lookup"><span data-stu-id="18d92-141">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="18d92-142">**required**</span><span class="sxs-lookup"><span data-stu-id="18d92-142">**required**</span></span>            | <span data-ttu-id="18d92-143">boolean</span><span class="sxs-lookup"><span data-stu-id="18d92-143">boolean</span></span> | <span data-ttu-id="18d92-144">指定列值是否不可选。</span><span class="sxs-lookup"><span data-stu-id="18d92-144">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="18d92-145">**boolean**</span><span class="sxs-lookup"><span data-stu-id="18d92-145">**boolean**</span></span>       | <span data-ttu-id="18d92-146">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="18d92-146">[booleanColumn][]</span></span>       | <span data-ttu-id="18d92-147">此列存储布尔值。</span><span class="sxs-lookup"><span data-stu-id="18d92-147">This column stores boolean values.</span></span>
| <span data-ttu-id="18d92-148">**calculated**</span><span class="sxs-lookup"><span data-stu-id="18d92-148">**calculated**</span></span>    | <span data-ttu-id="18d92-149">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="18d92-149">[calculatedColumn][]</span></span>    | <span data-ttu-id="18d92-150">根据其他列计算此列的数据。</span><span class="sxs-lookup"><span data-stu-id="18d92-150">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="18d92-151">**choice**</span><span class="sxs-lookup"><span data-stu-id="18d92-151">**choice**</span></span>        | <span data-ttu-id="18d92-152">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="18d92-152">[choiceColumn][]</span></span>        | <span data-ttu-id="18d92-153">此列存储所选列表中的数据。</span><span class="sxs-lookup"><span data-stu-id="18d92-153">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="18d92-154">**currency**</span><span class="sxs-lookup"><span data-stu-id="18d92-154">**currency**</span></span>      | <span data-ttu-id="18d92-155">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="18d92-155">[currencyColumn][]</span></span>      | <span data-ttu-id="18d92-156">此列存储货币值。</span><span class="sxs-lookup"><span data-stu-id="18d92-156">This column stores currency values.</span></span>
| <span data-ttu-id="18d92-157">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="18d92-157">**dateTime**</span></span>      | <span data-ttu-id="18d92-158">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="18d92-158">[dateTimeColumn][]</span></span>      | <span data-ttu-id="18d92-159">此列存储日期时间值。</span><span class="sxs-lookup"><span data-stu-id="18d92-159">This column stores DateTime values.</span></span>
| <span data-ttu-id="18d92-160">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="18d92-160">**defaultValue**</span></span>  | <span data-ttu-id="18d92-161">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="18d92-161">[defaultColumnValue][]</span></span>  | <span data-ttu-id="18d92-162">此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="18d92-162">The default value for this column.</span></span>
| <span data-ttu-id="18d92-163">**地理位置**</span><span class="sxs-lookup"><span data-stu-id="18d92-163">**geolocation**</span></span>   | <span data-ttu-id="18d92-164">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="18d92-164">[geolocationColumn][]</span></span>   | <span data-ttu-id="18d92-165">此列存储一个地理位置。</span><span class="sxs-lookup"><span data-stu-id="18d92-165">This column stores a geolocation.</span></span>
| <span data-ttu-id="18d92-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="18d92-166">**lookup**</span></span>        | <span data-ttu-id="18d92-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="18d92-167">[lookupColumn][]</span></span>        | <span data-ttu-id="18d92-168">从网站中的另一个源查找此列的数据。</span><span class="sxs-lookup"><span data-stu-id="18d92-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="18d92-169">**number**</span><span class="sxs-lookup"><span data-stu-id="18d92-169">**number**</span></span>        | <span data-ttu-id="18d92-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="18d92-170">[numberColumn][]</span></span>        | <span data-ttu-id="18d92-171">此列存储数值。</span><span class="sxs-lookup"><span data-stu-id="18d92-171">This column stores number values.</span></span>
| <span data-ttu-id="18d92-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="18d92-172">**personOrGroup**</span></span> | <span data-ttu-id="18d92-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="18d92-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="18d92-174">此列存储个人或组值。</span><span class="sxs-lookup"><span data-stu-id="18d92-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="18d92-175">**text**</span><span class="sxs-lookup"><span data-stu-id="18d92-175">**text**</span></span>          | <span data-ttu-id="18d92-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="18d92-176">[textColumn][]</span></span>          | <span data-ttu-id="18d92-177">此列存储文本值。</span><span class="sxs-lookup"><span data-stu-id="18d92-177">This column stores text values.</span></span>

><span data-ttu-id="18d92-178">**注意:** 这些属性对应于 SharePoint 的[SPFieldType][]枚举。</span><span class="sxs-lookup"><span data-stu-id="18d92-178">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="18d92-179">虽然在上表中表示的是最常见的字段类型, 但此 beta API 仍缺少一些。</span><span class="sxs-lookup"><span data-stu-id="18d92-179">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="18d92-180">在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。</span><span class="sxs-lookup"><span data-stu-id="18d92-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="18d92-181">备注</span><span class="sxs-lookup"><span data-stu-id="18d92-181">Remarks</span></span>

<span data-ttu-id="18d92-182">默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。</span><span class="sxs-lookup"><span data-stu-id="18d92-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="18d92-183">若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="18d92-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="18d92-184">若要在 [listItems][listItem] 上显示**字段**值时看到这些内容，请在 `$select` 语句中添加名称所需的列。</span><span class="sxs-lookup"><span data-stu-id="18d92-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

<span data-ttu-id="18d92-198">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="18d92-198">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

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
