---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 96587cc1b3badf2d5fcc90bc7c1d2b1cfb710f6b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008497"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="8b5eb-102">ColumnDefinition 资源</span><span class="sxs-lookup"><span data-stu-id="8b5eb-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b5eb-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b5eb-103">JSON representation</span></span>

<span data-ttu-id="8b5eb-104">下面是 ColumnDefinition 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-104">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8b5eb-105">属性</span><span class="sxs-lookup"><span data-stu-id="8b5eb-105">Properties</span></span>

<span data-ttu-id="8b5eb-106">**columnDefinition** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="8b5eb-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="8b5eb-107">Property name</span></span>           | <span data-ttu-id="8b5eb-108">类型</span><span class="sxs-lookup"><span data-stu-id="8b5eb-108">Type</span></span>    | <span data-ttu-id="8b5eb-109">说明</span><span class="sxs-lookup"><span data-stu-id="8b5eb-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="8b5eb-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-110">**columnGroup**</span></span>         | <span data-ttu-id="8b5eb-111">string</span><span class="sxs-lookup"><span data-stu-id="8b5eb-111">string</span></span>  | <span data-ttu-id="8b5eb-112">对于网站列，此列所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="8b5eb-113">可以帮助组织相关的列。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-113">Helps organize related columns.</span></span>
| <span data-ttu-id="8b5eb-114">**description**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-114">**description**</span></span>         | <span data-ttu-id="8b5eb-115">string</span><span class="sxs-lookup"><span data-stu-id="8b5eb-115">string</span></span>  | <span data-ttu-id="8b5eb-116">面向用户的列描述。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="8b5eb-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-117">**displayName**</span></span>         | <span data-ttu-id="8b5eb-118">string</span><span class="sxs-lookup"><span data-stu-id="8b5eb-118">string</span></span>  | <span data-ttu-id="8b5eb-119">面向用户的列名称。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="8b5eb-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="8b5eb-121">boolean</span><span class="sxs-lookup"><span data-stu-id="8b5eb-121">boolean</span></span> | <span data-ttu-id="8b5eb-122">如果为 true，则此列不能有两个列表项具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="8b5eb-123">**hidden**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-123">**hidden**</span></span>              | <span data-ttu-id="8b5eb-124">boolean</span><span class="sxs-lookup"><span data-stu-id="8b5eb-124">boolean</span></span> | <span data-ttu-id="8b5eb-125">指定列是否显示在用户界面中。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-125">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="8b5eb-126">**id**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-126">**id**</span></span>                  | <span data-ttu-id="8b5eb-127">string</span><span class="sxs-lookup"><span data-stu-id="8b5eb-127">string</span></span>  | <span data-ttu-id="8b5eb-128">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="8b5eb-129">**indexed**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-129">**indexed**</span></span>             | <span data-ttu-id="8b5eb-130">boolean</span><span class="sxs-lookup"><span data-stu-id="8b5eb-130">boolean</span></span> | <span data-ttu-id="8b5eb-131">指定列值是否可用于排序和搜索。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="8b5eb-132">**name**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-132">**name**</span></span>                | <span data-ttu-id="8b5eb-133">string</span><span class="sxs-lookup"><span data-stu-id="8b5eb-133">string</span></span>  | <span data-ttu-id="8b5eb-134">在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="8b5eb-135">对于面向用户的名称，请参阅 **displayName**。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="8b5eb-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-136">**readOnly**</span></span>            | <span data-ttu-id="8b5eb-137">bool</span><span class="sxs-lookup"><span data-stu-id="8b5eb-137">bool</span></span>    | <span data-ttu-id="8b5eb-138">指定是否可以修改列值。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="8b5eb-139">**required**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-139">**required**</span></span>            | <span data-ttu-id="8b5eb-140">boolean</span><span class="sxs-lookup"><span data-stu-id="8b5eb-140">boolean</span></span> | <span data-ttu-id="8b5eb-141">指定列值是否不可选。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="8b5eb-142">列可以包含各种类型的数据。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="8b5eb-143">以下属性表示列存储的数据类型以及该数据的其他设置。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="8b5eb-144">这些属性是互相排斥的 - 列只能指定其中一个。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="8b5eb-145">属性名称</span><span class="sxs-lookup"><span data-stu-id="8b5eb-145">Property name</span></span>     | <span data-ttu-id="8b5eb-146">类型</span><span class="sxs-lookup"><span data-stu-id="8b5eb-146">Type</span></span>                    | <span data-ttu-id="8b5eb-147">说明</span><span class="sxs-lookup"><span data-stu-id="8b5eb-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="8b5eb-148">**boolean**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-148">**boolean**</span></span>       | <span data-ttu-id="8b5eb-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="8b5eb-149">[booleanColumn][]</span></span>       | <span data-ttu-id="8b5eb-150">此列存储布尔值。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-150">This column stores boolean values.</span></span>
| <span data-ttu-id="8b5eb-151">**calculated**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-151">**calculated**</span></span>    | <span data-ttu-id="8b5eb-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="8b5eb-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="8b5eb-153">根据其他列计算此列的数据。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="8b5eb-154">**choice**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-154">**choice**</span></span>        | <span data-ttu-id="8b5eb-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="8b5eb-155">[choiceColumn][]</span></span>        | <span data-ttu-id="8b5eb-156">此列存储所选列表中的数据。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="8b5eb-157">**currency**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-157">**currency**</span></span>      | <span data-ttu-id="8b5eb-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="8b5eb-158">[currencyColumn][]</span></span>      | <span data-ttu-id="8b5eb-159">此列存储货币值。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-159">This column stores currency values.</span></span>
| <span data-ttu-id="8b5eb-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-160">**dateTime**</span></span>      | <span data-ttu-id="8b5eb-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="8b5eb-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="8b5eb-162">此列存储日期时间值。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="8b5eb-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-163">**defaultValue**</span></span>  | <span data-ttu-id="8b5eb-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="8b5eb-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="8b5eb-165">此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-165">The default value for this column.</span></span>
| <span data-ttu-id="8b5eb-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-166">**lookup**</span></span>        | <span data-ttu-id="8b5eb-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="8b5eb-167">[lookupColumn][]</span></span>        | <span data-ttu-id="8b5eb-168">从网站中的另一个源查找此列的数据。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="8b5eb-169">**number**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-169">**number**</span></span>        | <span data-ttu-id="8b5eb-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="8b5eb-170">[numberColumn][]</span></span>        | <span data-ttu-id="8b5eb-171">此列存储数值。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-171">This column stores number values.</span></span>
| <span data-ttu-id="8b5eb-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-172">**personOrGroup**</span></span> | <span data-ttu-id="8b5eb-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="8b5eb-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="8b5eb-174">此列存储个人或组值。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="8b5eb-175">**text**</span><span class="sxs-lookup"><span data-stu-id="8b5eb-175">**text**</span></span>          | <span data-ttu-id="8b5eb-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="8b5eb-176">[textColumn][]</span></span>          | <span data-ttu-id="8b5eb-177">此列存储文本值。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-177">This column stores text values.</span></span>

<span data-ttu-id="8b5eb-178">注意：这些属性对应于 SharePoint 的 [SPFieldType][] 枚举。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="8b5eb-179">时的最常见的字段类型表示上方，此 API 仍然缺少一些。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-179">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="8b5eb-180">在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="8b5eb-181">备注</span><span class="sxs-lookup"><span data-stu-id="8b5eb-181">Remarks</span></span>

<span data-ttu-id="8b5eb-182">默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="8b5eb-183">若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="8b5eb-184">若要在 [listItems][listItem] 上显示**字段**值时看到这些内容，请在 `$select` 语句中添加名称所需的列。</span><span class="sxs-lookup"><span data-stu-id="8b5eb-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

<span data-ttu-id="8b5eb-197">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="8b5eb-197">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
