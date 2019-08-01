---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
description: 下面是 ColumnDefinition 资源的 JSON 表示形式。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3a02721c5289b1d49077e1b2d9fa1017f0c53021
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032870"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="1d116-103">ColumnDefinition 资源</span><span class="sxs-lookup"><span data-stu-id="1d116-103">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d116-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d116-104">JSON representation</span></span>

<span data-ttu-id="1d116-105">下面是 ColumnDefinition 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d116-105">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="1d116-106">属性</span><span class="sxs-lookup"><span data-stu-id="1d116-106">Properties</span></span>

<span data-ttu-id="1d116-107">**columnDefinition** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="1d116-107">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="1d116-108">属性名</span><span class="sxs-lookup"><span data-stu-id="1d116-108">Property name</span></span>           | <span data-ttu-id="1d116-109">类型</span><span class="sxs-lookup"><span data-stu-id="1d116-109">Type</span></span>    | <span data-ttu-id="1d116-110">说明</span><span class="sxs-lookup"><span data-stu-id="1d116-110">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="1d116-111">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="1d116-111">**columnGroup**</span></span>         | <span data-ttu-id="1d116-112">string</span><span class="sxs-lookup"><span data-stu-id="1d116-112">string</span></span>  | <span data-ttu-id="1d116-113">对于网站列，此列所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="1d116-113">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="1d116-114">可以帮助组织相关的列。</span><span class="sxs-lookup"><span data-stu-id="1d116-114">Helps organize related columns.</span></span>
| <span data-ttu-id="1d116-115">**说明**</span><span class="sxs-lookup"><span data-stu-id="1d116-115">**description**</span></span>         | <span data-ttu-id="1d116-116">string</span><span class="sxs-lookup"><span data-stu-id="1d116-116">string</span></span>  | <span data-ttu-id="1d116-117">面向用户的列描述。</span><span class="sxs-lookup"><span data-stu-id="1d116-117">The user-facing description of the column.</span></span>
| <span data-ttu-id="1d116-118">**displayName**</span><span class="sxs-lookup"><span data-stu-id="1d116-118">**displayName**</span></span>         | <span data-ttu-id="1d116-119">string</span><span class="sxs-lookup"><span data-stu-id="1d116-119">string</span></span>  | <span data-ttu-id="1d116-120">面向用户的列名称。</span><span class="sxs-lookup"><span data-stu-id="1d116-120">The user-facing name of the column.</span></span>
| <span data-ttu-id="1d116-121">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="1d116-121">**enforceUniqueValues**</span></span> | <span data-ttu-id="1d116-122">boolean</span><span class="sxs-lookup"><span data-stu-id="1d116-122">boolean</span></span> | <span data-ttu-id="1d116-123">如果为 true，则此列不能有两个列表项具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="1d116-123">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="1d116-124">**hidden**</span><span class="sxs-lookup"><span data-stu-id="1d116-124">**hidden**</span></span>              | <span data-ttu-id="1d116-125">boolean</span><span class="sxs-lookup"><span data-stu-id="1d116-125">boolean</span></span> | <span data-ttu-id="1d116-126">指定列是否显示在用户界面中。</span><span class="sxs-lookup"><span data-stu-id="1d116-126">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="1d116-127">**id**</span><span class="sxs-lookup"><span data-stu-id="1d116-127">**id**</span></span>                  | <span data-ttu-id="1d116-128">string</span><span class="sxs-lookup"><span data-stu-id="1d116-128">string</span></span>  | <span data-ttu-id="1d116-129">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1d116-129">The unique identifier for the column.</span></span>
| <span data-ttu-id="1d116-130">**indexed**</span><span class="sxs-lookup"><span data-stu-id="1d116-130">**indexed**</span></span>             | <span data-ttu-id="1d116-131">boolean</span><span class="sxs-lookup"><span data-stu-id="1d116-131">boolean</span></span> | <span data-ttu-id="1d116-132">指定列值是否可用于排序和搜索。</span><span class="sxs-lookup"><span data-stu-id="1d116-132">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="1d116-133">**name**</span><span class="sxs-lookup"><span data-stu-id="1d116-133">**name**</span></span>                | <span data-ttu-id="1d116-134">string</span><span class="sxs-lookup"><span data-stu-id="1d116-134">string</span></span>  | <span data-ttu-id="1d116-135">在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。</span><span class="sxs-lookup"><span data-stu-id="1d116-135">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="1d116-136">对于面向用户的名称，请参阅 **displayName**。</span><span class="sxs-lookup"><span data-stu-id="1d116-136">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="1d116-137">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="1d116-137">**readOnly**</span></span>            | <span data-ttu-id="1d116-138">bool</span><span class="sxs-lookup"><span data-stu-id="1d116-138">bool</span></span>    | <span data-ttu-id="1d116-139">指定是否可以修改列值。</span><span class="sxs-lookup"><span data-stu-id="1d116-139">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="1d116-140">**required**</span><span class="sxs-lookup"><span data-stu-id="1d116-140">**required**</span></span>            | <span data-ttu-id="1d116-141">boolean</span><span class="sxs-lookup"><span data-stu-id="1d116-141">boolean</span></span> | <span data-ttu-id="1d116-142">指定列值是否不可选。</span><span class="sxs-lookup"><span data-stu-id="1d116-142">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="1d116-143">列可以包含各种类型的数据。</span><span class="sxs-lookup"><span data-stu-id="1d116-143">Columns can hold data of various types.</span></span>
<span data-ttu-id="1d116-144">以下属性表示列存储的数据类型以及该数据的其他设置。</span><span class="sxs-lookup"><span data-stu-id="1d116-144">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="1d116-145">这些属性是互相排斥的 - 列只能指定其中一个。</span><span class="sxs-lookup"><span data-stu-id="1d116-145">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="1d116-146">属性名</span><span class="sxs-lookup"><span data-stu-id="1d116-146">Property name</span></span>     | <span data-ttu-id="1d116-147">类型</span><span class="sxs-lookup"><span data-stu-id="1d116-147">Type</span></span>                    | <span data-ttu-id="1d116-148">说明</span><span class="sxs-lookup"><span data-stu-id="1d116-148">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="1d116-149">**boolean**</span><span class="sxs-lookup"><span data-stu-id="1d116-149">**boolean**</span></span>       | <span data-ttu-id="1d116-150">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="1d116-150">[booleanColumn][]</span></span>       | <span data-ttu-id="1d116-151">此列存储布尔值。</span><span class="sxs-lookup"><span data-stu-id="1d116-151">This column stores boolean values.</span></span>
| <span data-ttu-id="1d116-152">**calculated**</span><span class="sxs-lookup"><span data-stu-id="1d116-152">**calculated**</span></span>    | <span data-ttu-id="1d116-153">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="1d116-153">[calculatedColumn][]</span></span>    | <span data-ttu-id="1d116-154">根据其他列计算此列的数据。</span><span class="sxs-lookup"><span data-stu-id="1d116-154">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="1d116-155">**choice**</span><span class="sxs-lookup"><span data-stu-id="1d116-155">**choice**</span></span>        | <span data-ttu-id="1d116-156">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="1d116-156">[choiceColumn][]</span></span>        | <span data-ttu-id="1d116-157">此列存储所选列表中的数据。</span><span class="sxs-lookup"><span data-stu-id="1d116-157">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="1d116-158">**currency**</span><span class="sxs-lookup"><span data-stu-id="1d116-158">**currency**</span></span>      | <span data-ttu-id="1d116-159">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="1d116-159">[currencyColumn][]</span></span>      | <span data-ttu-id="1d116-160">此列存储货币值。</span><span class="sxs-lookup"><span data-stu-id="1d116-160">This column stores currency values.</span></span>
| <span data-ttu-id="1d116-161">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="1d116-161">**dateTime**</span></span>      | <span data-ttu-id="1d116-162">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="1d116-162">[dateTimeColumn][]</span></span>      | <span data-ttu-id="1d116-163">此列存储日期时间值。</span><span class="sxs-lookup"><span data-stu-id="1d116-163">This column stores DateTime values.</span></span>
| <span data-ttu-id="1d116-164">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="1d116-164">**defaultValue**</span></span>  | <span data-ttu-id="1d116-165">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="1d116-165">[defaultColumnValue][]</span></span>  | <span data-ttu-id="1d116-166">此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="1d116-166">The default value for this column.</span></span>
| <span data-ttu-id="1d116-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="1d116-167">**lookup**</span></span>        | <span data-ttu-id="1d116-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="1d116-168">[lookupColumn][]</span></span>        | <span data-ttu-id="1d116-169">从网站中的另一个源查找此列的数据。</span><span class="sxs-lookup"><span data-stu-id="1d116-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="1d116-170">**number**</span><span class="sxs-lookup"><span data-stu-id="1d116-170">**number**</span></span>        | <span data-ttu-id="1d116-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="1d116-171">[numberColumn][]</span></span>        | <span data-ttu-id="1d116-172">此列存储数值。</span><span class="sxs-lookup"><span data-stu-id="1d116-172">This column stores number values.</span></span>
| <span data-ttu-id="1d116-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="1d116-173">**personOrGroup**</span></span> | <span data-ttu-id="1d116-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="1d116-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="1d116-175">此列存储个人或组值。</span><span class="sxs-lookup"><span data-stu-id="1d116-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="1d116-176">**text**</span><span class="sxs-lookup"><span data-stu-id="1d116-176">**text**</span></span>          | <span data-ttu-id="1d116-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="1d116-177">[textColumn][]</span></span>          | <span data-ttu-id="1d116-178">此列存储文本值。</span><span class="sxs-lookup"><span data-stu-id="1d116-178">This column stores text values.</span></span>

<span data-ttu-id="1d116-179">注意：这些属性对应于 SharePoint 的 [SPFieldType][] 枚举。</span><span class="sxs-lookup"><span data-stu-id="1d116-179">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="1d116-180">虽然上面表示的是最常见的字段类型, 但此 API 仍缺少一些。</span><span class="sxs-lookup"><span data-stu-id="1d116-180">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="1d116-181">在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。</span><span class="sxs-lookup"><span data-stu-id="1d116-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="1d116-182">备注</span><span class="sxs-lookup"><span data-stu-id="1d116-182">Remarks</span></span>

<span data-ttu-id="1d116-183">默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。</span><span class="sxs-lookup"><span data-stu-id="1d116-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="1d116-184">若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="1d116-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="1d116-185">若要在 [listItems][listItem] 上显示**字段**值时看到这些内容，请在 `$select` 语句中添加名称所需的列。</span><span class="sxs-lookup"><span data-stu-id="1d116-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

<span data-ttu-id="1d116-198">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="1d116-198">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
