---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 9b99abe78b009786d489ec7f0c0fdce1e2945b1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041609"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="177c9-102">columnDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="177c9-102">columnDefinition resource type</span></span>

> <span data-ttu-id="177c9-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="177c9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="177c9-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="177c9-104">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="177c9-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="177c9-105">JSON representation</span></span>

<span data-ttu-id="177c9-106">下面是 columnDefinition 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="177c9-106">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="177c9-107">属性</span><span class="sxs-lookup"><span data-stu-id="177c9-107">Properties</span></span>

<span data-ttu-id="177c9-108">列可以包含各种类型的数据。</span><span class="sxs-lookup"><span data-stu-id="177c9-108">Columns can hold data of various types.</span></span>
<span data-ttu-id="177c9-109">以下属性表示列存储的数据类型以及该数据的其他设置。</span><span class="sxs-lookup"><span data-stu-id="177c9-109">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="177c9-110">（布尔值、 计算，选择、 货币、 日期时间、 查找、 数量、 personOrGroup、 文本） 与类型相关的属性都是互斥的--列可以仅具有指定两者之一。</span><span class="sxs-lookup"><span data-stu-id="177c9-110">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="177c9-111">属性名</span><span class="sxs-lookup"><span data-stu-id="177c9-111">Property name</span></span>           | <span data-ttu-id="177c9-112">类型</span><span class="sxs-lookup"><span data-stu-id="177c9-112">Type</span></span>    | <span data-ttu-id="177c9-113">说明</span><span class="sxs-lookup"><span data-stu-id="177c9-113">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="177c9-114">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="177c9-114">**columnGroup**</span></span>         | <span data-ttu-id="177c9-115">string</span><span class="sxs-lookup"><span data-stu-id="177c9-115">string</span></span>  | <span data-ttu-id="177c9-116">对于网站列，此列所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="177c9-116">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="177c9-117">可以帮助组织相关的列。</span><span class="sxs-lookup"><span data-stu-id="177c9-117">Helps organize related columns.</span></span>
| <span data-ttu-id="177c9-118">**说明**</span><span class="sxs-lookup"><span data-stu-id="177c9-118">**description**</span></span>         | <span data-ttu-id="177c9-119">string</span><span class="sxs-lookup"><span data-stu-id="177c9-119">string</span></span>  | <span data-ttu-id="177c9-120">面向用户的列描述。</span><span class="sxs-lookup"><span data-stu-id="177c9-120">The user-facing description of the column.</span></span>
| <span data-ttu-id="177c9-121">**displayName**</span><span class="sxs-lookup"><span data-stu-id="177c9-121">**displayName**</span></span>         | <span data-ttu-id="177c9-122">string</span><span class="sxs-lookup"><span data-stu-id="177c9-122">string</span></span>  | <span data-ttu-id="177c9-123">面向用户的列名称。</span><span class="sxs-lookup"><span data-stu-id="177c9-123">The user-facing name of the column.</span></span>
| <span data-ttu-id="177c9-124">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="177c9-124">**enforceUniqueValues**</span></span> | <span data-ttu-id="177c9-125">boolean</span><span class="sxs-lookup"><span data-stu-id="177c9-125">boolean</span></span> | <span data-ttu-id="177c9-126">如果为 true，则此列不能有两个列表项具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="177c9-126">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="177c9-127">**hidden**</span><span class="sxs-lookup"><span data-stu-id="177c9-127">**hidden**</span></span>              | <span data-ttu-id="177c9-128">boolean</span><span class="sxs-lookup"><span data-stu-id="177c9-128">boolean</span></span> | <span data-ttu-id="177c9-129">指定列是否显示在用户界面中。</span><span class="sxs-lookup"><span data-stu-id="177c9-129">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="177c9-130">**id**</span><span class="sxs-lookup"><span data-stu-id="177c9-130">**id**</span></span>                  | <span data-ttu-id="177c9-131">string</span><span class="sxs-lookup"><span data-stu-id="177c9-131">string</span></span>  | <span data-ttu-id="177c9-132">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="177c9-132">The unique identifier for the column.</span></span>
| <span data-ttu-id="177c9-133">**indexed**</span><span class="sxs-lookup"><span data-stu-id="177c9-133">**indexed**</span></span>             | <span data-ttu-id="177c9-134">boolean</span><span class="sxs-lookup"><span data-stu-id="177c9-134">boolean</span></span> | <span data-ttu-id="177c9-135">指定列值是否可用于排序和搜索。</span><span class="sxs-lookup"><span data-stu-id="177c9-135">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="177c9-136">**name**</span><span class="sxs-lookup"><span data-stu-id="177c9-136">**name**</span></span>                | <span data-ttu-id="177c9-137">string</span><span class="sxs-lookup"><span data-stu-id="177c9-137">string</span></span>  | <span data-ttu-id="177c9-138">在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。</span><span class="sxs-lookup"><span data-stu-id="177c9-138">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="177c9-139">对于面向用户的名称，请参阅 **displayName**。</span><span class="sxs-lookup"><span data-stu-id="177c9-139">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="177c9-140">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="177c9-140">**readOnly**</span></span>            | <span data-ttu-id="177c9-141">bool</span><span class="sxs-lookup"><span data-stu-id="177c9-141">bool</span></span>    | <span data-ttu-id="177c9-142">指定是否可以修改列值。</span><span class="sxs-lookup"><span data-stu-id="177c9-142">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="177c9-143">**required**</span><span class="sxs-lookup"><span data-stu-id="177c9-143">**required**</span></span>            | <span data-ttu-id="177c9-144">boolean</span><span class="sxs-lookup"><span data-stu-id="177c9-144">boolean</span></span> | <span data-ttu-id="177c9-145">指定列值是否不可选。</span><span class="sxs-lookup"><span data-stu-id="177c9-145">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="177c9-146">**boolean**</span><span class="sxs-lookup"><span data-stu-id="177c9-146">**boolean**</span></span>       | <span data-ttu-id="177c9-147">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="177c9-147">[booleanColumn][]</span></span>       | <span data-ttu-id="177c9-148">此列存储布尔值。</span><span class="sxs-lookup"><span data-stu-id="177c9-148">This column stores boolean values.</span></span>
| <span data-ttu-id="177c9-149">**calculated**</span><span class="sxs-lookup"><span data-stu-id="177c9-149">**calculated**</span></span>    | <span data-ttu-id="177c9-150">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="177c9-150">[calculatedColumn][]</span></span>    | <span data-ttu-id="177c9-151">根据其他列计算此列的数据。</span><span class="sxs-lookup"><span data-stu-id="177c9-151">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="177c9-152">**choice**</span><span class="sxs-lookup"><span data-stu-id="177c9-152">**choice**</span></span>        | <span data-ttu-id="177c9-153">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="177c9-153">[choiceColumn][]</span></span>        | <span data-ttu-id="177c9-154">此列存储所选列表中的数据。</span><span class="sxs-lookup"><span data-stu-id="177c9-154">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="177c9-155">**currency**</span><span class="sxs-lookup"><span data-stu-id="177c9-155">**currency**</span></span>      | <span data-ttu-id="177c9-156">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="177c9-156">[currencyColumn][]</span></span>      | <span data-ttu-id="177c9-157">此列存储货币值。</span><span class="sxs-lookup"><span data-stu-id="177c9-157">This column stores currency values.</span></span>
| <span data-ttu-id="177c9-158">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="177c9-158">**dateTime**</span></span>      | <span data-ttu-id="177c9-159">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="177c9-159">[dateTimeColumn][]</span></span>      | <span data-ttu-id="177c9-160">此列存储日期时间值。</span><span class="sxs-lookup"><span data-stu-id="177c9-160">This column stores DateTime values.</span></span>
| <span data-ttu-id="177c9-161">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="177c9-161">**defaultValue**</span></span>  | <span data-ttu-id="177c9-162">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="177c9-162">[defaultColumnValue][]</span></span>  | <span data-ttu-id="177c9-163">此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="177c9-163">The default value for this column.</span></span>
| <span data-ttu-id="177c9-164">**地理位置**</span><span class="sxs-lookup"><span data-stu-id="177c9-164">**geolocation**</span></span>   | <span data-ttu-id="177c9-165">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="177c9-165">[geolocationColumn][]</span></span>   | <span data-ttu-id="177c9-166">此列存储地理位置。</span><span class="sxs-lookup"><span data-stu-id="177c9-166">This column stores a geolocation.</span></span>
| <span data-ttu-id="177c9-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="177c9-167">**lookup**</span></span>        | <span data-ttu-id="177c9-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="177c9-168">[lookupColumn][]</span></span>        | <span data-ttu-id="177c9-169">从网站中的另一个源查找此列的数据。</span><span class="sxs-lookup"><span data-stu-id="177c9-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="177c9-170">**number**</span><span class="sxs-lookup"><span data-stu-id="177c9-170">**number**</span></span>        | <span data-ttu-id="177c9-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="177c9-171">[numberColumn][]</span></span>        | <span data-ttu-id="177c9-172">此列存储数值。</span><span class="sxs-lookup"><span data-stu-id="177c9-172">This column stores number values.</span></span>
| <span data-ttu-id="177c9-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="177c9-173">**personOrGroup**</span></span> | <span data-ttu-id="177c9-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="177c9-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="177c9-175">此列存储个人或组值。</span><span class="sxs-lookup"><span data-stu-id="177c9-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="177c9-176">**text**</span><span class="sxs-lookup"><span data-stu-id="177c9-176">**text**</span></span>          | <span data-ttu-id="177c9-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="177c9-177">[textColumn][]</span></span>          | <span data-ttu-id="177c9-178">此列存储文本值。</span><span class="sxs-lookup"><span data-stu-id="177c9-178">This column stores text values.</span></span>

><span data-ttu-id="177c9-179">**注意：** 这些属性对应于 SharePoint 的[SPFieldType][]枚举。</span><span class="sxs-lookup"><span data-stu-id="177c9-179">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="177c9-180">时的最常见的字段类型表示上表中，此 beta API 仍然缺少一些。</span><span class="sxs-lookup"><span data-stu-id="177c9-180">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="177c9-181">在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。</span><span class="sxs-lookup"><span data-stu-id="177c9-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="177c9-182">备注</span><span class="sxs-lookup"><span data-stu-id="177c9-182">Remarks</span></span>

<span data-ttu-id="177c9-183">默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。</span><span class="sxs-lookup"><span data-stu-id="177c9-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="177c9-184">若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="177c9-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="177c9-185">若要在 [listItems][listItem] 上显示**字段**值时看到这些内容，请在 `$select` 语句中添加名称所需的列。</span><span class="sxs-lookup"><span data-stu-id="177c9-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

<span data-ttu-id="177c9-199">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="177c9-199">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
