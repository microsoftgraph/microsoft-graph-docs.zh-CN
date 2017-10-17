---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: e5942ddee4b505243cb64121862ce9e89e52d245
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="columndefinition-resource"></a><span data-ttu-id="b5054-102">ColumnDefinition 资源</span><span class="sxs-lookup"><span data-stu-id="b5054-102">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5054-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5054-103">JSON representation</span></span>

<span data-ttu-id="b5054-104">下面是 ColumnDefinition 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5054-104">Here is a JSON representation of a {type} resource.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnDefinition",
       "keyProperty": "id", "optionalProperties": [ ] } -->

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

## <a name="properties"></a><span data-ttu-id="b5054-105">属性</span><span class="sxs-lookup"><span data-stu-id="b5054-105">Properties</span></span>

<span data-ttu-id="b5054-106">**columnDefinition** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="b5054-106">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="b5054-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="b5054-107">Property name</span></span>           | <span data-ttu-id="b5054-108">类型</span><span class="sxs-lookup"><span data-stu-id="b5054-108">Type</span></span>    | <span data-ttu-id="b5054-109">说明</span><span class="sxs-lookup"><span data-stu-id="b5054-109">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="b5054-110">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="b5054-110">**columnGroup**</span></span>         | <span data-ttu-id="b5054-111">string</span><span class="sxs-lookup"><span data-stu-id="b5054-111">string</span></span>  | <span data-ttu-id="b5054-112">对于网站列，此列所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="b5054-112">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="b5054-113">可以帮助组织相关的列。</span><span class="sxs-lookup"><span data-stu-id="b5054-113">Helps organize related columns.</span></span>
| <span data-ttu-id="b5054-114">**description**</span><span class="sxs-lookup"><span data-stu-id="b5054-114">**description**</span></span>         | <span data-ttu-id="b5054-115">string</span><span class="sxs-lookup"><span data-stu-id="b5054-115">string</span></span>  | <span data-ttu-id="b5054-116">面向用户的列描述。</span><span class="sxs-lookup"><span data-stu-id="b5054-116">The user-facing description of the column.</span></span>
| <span data-ttu-id="b5054-117">**displayName**</span><span class="sxs-lookup"><span data-stu-id="b5054-117">**displayName**</span></span>         | <span data-ttu-id="b5054-118">string</span><span class="sxs-lookup"><span data-stu-id="b5054-118">string</span></span>  | <span data-ttu-id="b5054-119">面向用户的列名称。</span><span class="sxs-lookup"><span data-stu-id="b5054-119">The user-facing name of the column.</span></span>
| <span data-ttu-id="b5054-120">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="b5054-120">**enforceUniqueValues**</span></span> | <span data-ttu-id="b5054-121">boolean</span><span class="sxs-lookup"><span data-stu-id="b5054-121">boolean</span></span> | <span data-ttu-id="b5054-122">如果为 true，则此列不能有两个列表项具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="b5054-122">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="b5054-123">**hidden**</span><span class="sxs-lookup"><span data-stu-id="b5054-123">**hidden**</span></span>              | <span data-ttu-id="b5054-124">boolean</span><span class="sxs-lookup"><span data-stu-id="b5054-124">boolean</span></span> | <span data-ttu-id="b5054-125">指定列是否显示在用户界面中。</span><span class="sxs-lookup"><span data-stu-id="b5054-125">Specifies the policy item name that is displayed in the oss14long user interface.</span></span>
| <span data-ttu-id="b5054-126">**id**</span><span class="sxs-lookup"><span data-stu-id="b5054-126">**id**</span></span>                  | <span data-ttu-id="b5054-127">string</span><span class="sxs-lookup"><span data-stu-id="b5054-127">string</span></span>  | <span data-ttu-id="b5054-128">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b5054-128">The unique identifier for the column.</span></span>
| <span data-ttu-id="b5054-129">**indexed**</span><span class="sxs-lookup"><span data-stu-id="b5054-129">**Indexed**</span></span>             | <span data-ttu-id="b5054-130">boolean</span><span class="sxs-lookup"><span data-stu-id="b5054-130">boolean</span></span> | <span data-ttu-id="b5054-131">指定列值是否可用于排序和搜索。</span><span class="sxs-lookup"><span data-stu-id="b5054-131">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="b5054-132">**name**</span><span class="sxs-lookup"><span data-stu-id="b5054-132">**name**</span></span>                | <span data-ttu-id="b5054-133">string</span><span class="sxs-lookup"><span data-stu-id="b5054-133">string</span></span>  | <span data-ttu-id="b5054-134">在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。</span><span class="sxs-lookup"><span data-stu-id="b5054-134">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="b5054-135">对于面向用户的名称，请参阅 **displayName**。</span><span class="sxs-lookup"><span data-stu-id="b5054-135">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="b5054-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="b5054-136">**Read-only.**</span></span>            | <span data-ttu-id="b5054-137">bool</span><span class="sxs-lookup"><span data-stu-id="b5054-137">bool</span></span>    | <span data-ttu-id="b5054-138">指定是否可以修改列值。</span><span class="sxs-lookup"><span data-stu-id="b5054-138">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="b5054-139">**required**</span><span class="sxs-lookup"><span data-stu-id="b5054-139">**Required**</span></span>            | <span data-ttu-id="b5054-140">boolean</span><span class="sxs-lookup"><span data-stu-id="b5054-140">boolean</span></span> | <span data-ttu-id="b5054-141">指定列值是否不可选。</span><span class="sxs-lookup"><span data-stu-id="b5054-141">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="b5054-142">列可以包含各种类型的数据。</span><span class="sxs-lookup"><span data-stu-id="b5054-142">Columns can hold data of various types.</span></span>
<span data-ttu-id="b5054-143">以下属性表示列存储的数据类型以及该数据的其他设置。</span><span class="sxs-lookup"><span data-stu-id="b5054-143">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="b5054-144">这些属性是互相排斥的 - 列只能指定其中一个。</span><span class="sxs-lookup"><span data-stu-id="b5054-144">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="b5054-145">属性名称</span><span class="sxs-lookup"><span data-stu-id="b5054-145">Property name</span></span>     | <span data-ttu-id="b5054-146">类型</span><span class="sxs-lookup"><span data-stu-id="b5054-146">Type</span></span>                    | <span data-ttu-id="b5054-147">说明</span><span class="sxs-lookup"><span data-stu-id="b5054-147">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="b5054-148">**boolean**</span><span class="sxs-lookup"><span data-stu-id="b5054-148">**Boolean**</span></span>       | <span data-ttu-id="b5054-149">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="b5054-149">[booleanColumn][]</span></span>       | <span data-ttu-id="b5054-150">此列存储布尔值。</span><span class="sxs-lookup"><span data-stu-id="b5054-150">This column stores boolean values.</span></span>
| <span data-ttu-id="b5054-151">**calculated**</span><span class="sxs-lookup"><span data-stu-id="b5054-151">**Calculated**</span></span>    | <span data-ttu-id="b5054-152">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="b5054-152">[calculatedColumn][]</span></span>    | <span data-ttu-id="b5054-153">根据其他列计算此列的数据。</span><span class="sxs-lookup"><span data-stu-id="b5054-153">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="b5054-154">**choice**</span><span class="sxs-lookup"><span data-stu-id="b5054-154">**Choice**</span></span>        | <span data-ttu-id="b5054-155">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="b5054-155">[choiceColumn][]</span></span>        | <span data-ttu-id="b5054-156">此列存储选项列表中的数据。</span><span class="sxs-lookup"><span data-stu-id="b5054-156">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="b5054-157">**currency**</span><span class="sxs-lookup"><span data-stu-id="b5054-157">**Currency**</span></span>      | <span data-ttu-id="b5054-158">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="b5054-158">[currencyColumn][]</span></span>      | <span data-ttu-id="b5054-159">此列存储货币值。</span><span class="sxs-lookup"><span data-stu-id="b5054-159">This column stores currency values.</span></span>
| <span data-ttu-id="b5054-160">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="b5054-160">**DateTime**</span></span>      | <span data-ttu-id="b5054-161">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="b5054-161">[dateTimeColumn][]</span></span>      | <span data-ttu-id="b5054-162">此列存储日期时间值。</span><span class="sxs-lookup"><span data-stu-id="b5054-162">This column stores DateTime values.</span></span>
| <span data-ttu-id="b5054-163">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="b5054-163">**DefaultValue**</span></span>  | <span data-ttu-id="b5054-164">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="b5054-164">[defaultColumnValue][]</span></span>  | <span data-ttu-id="b5054-165">此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="b5054-165">The default value for this column.</span></span>
| <span data-ttu-id="b5054-166">**lookup**</span><span class="sxs-lookup"><span data-stu-id="b5054-166">**Lookup**</span></span>        | <span data-ttu-id="b5054-167">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="b5054-167">[lookupColumn][]</span></span>        | <span data-ttu-id="b5054-168">从网站中的另一个源查找此列的数据。</span><span class="sxs-lookup"><span data-stu-id="b5054-168">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="b5054-169">**number**</span><span class="sxs-lookup"><span data-stu-id="b5054-169">**number**</span></span>        | <span data-ttu-id="b5054-170">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="b5054-170">[numberColumn][]</span></span>        | <span data-ttu-id="b5054-171">此列存储数值。</span><span class="sxs-lookup"><span data-stu-id="b5054-171">This column stores number values.</span></span>
| <span data-ttu-id="b5054-172">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="b5054-172">**personOrGroup**</span></span> | <span data-ttu-id="b5054-173">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="b5054-173">[personOrGroupColumn][]</span></span> | <span data-ttu-id="b5054-174">此列存储个人或组值。</span><span class="sxs-lookup"><span data-stu-id="b5054-174">This column stores Person or Group values.</span></span>
| <span data-ttu-id="b5054-175">**text**</span><span class="sxs-lookup"><span data-stu-id="b5054-175">**text**</span></span>          | <span data-ttu-id="b5054-176">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="b5054-176">[textColumn][]</span></span>          | <span data-ttu-id="b5054-177">此列存储文本值。</span><span class="sxs-lookup"><span data-stu-id="b5054-177">This column stores text values.</span></span>

<span data-ttu-id="b5054-178">注意：这些属性对应于 SharePoint 的 [SPFieldType][] 枚举。</span><span class="sxs-lookup"><span data-stu-id="b5054-178">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="b5054-179">虽然上面体现了最常见的字段类型，但仍缺少一些此测试 API。</span><span class="sxs-lookup"><span data-stu-id="b5054-179">While the most common field types are represented above, this beta API is still missing some.</span></span>
<span data-ttu-id="b5054-180">在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。</span><span class="sxs-lookup"><span data-stu-id="b5054-180">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="b5054-181">备注</span><span class="sxs-lookup"><span data-stu-id="b5054-181">Remarks</span></span>

<span data-ttu-id="b5054-182">默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。</span><span class="sxs-lookup"><span data-stu-id="b5054-182">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="b5054-183">若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="b5054-183">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="b5054-184">若要在 [listItems][listItem] 上显示**字段**值时看到这些内容，请在 `$select` 语句中添加名称所需的列。</span><span class="sxs-lookup"><span data-stu-id="b5054-184">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleanColumn.md
[calculatedColumn]: calculatedColumn.md
[choiceColumn]: choiceColumn.md
[currencyColumn]: currencyColumn.md
[dateTimeColumn]: dateTimeColumn.md
[defaultColumnValue]: defaultColumnValue.md
[lookupColumn]: lookupColumn.md
[numberColumn]: numberColumn.md
[personOrGroupColumn]: personOrGroupColumn.md
[textColumn]: textColumn.md
[fieldValueSet]: fieldValueSet.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/en-us/library/microsoft.sharepoint.spfieldtype.aspx

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
