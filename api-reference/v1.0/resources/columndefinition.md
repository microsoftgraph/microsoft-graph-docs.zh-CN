---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
description: 下面是 ColumnDefinition 资源的 JSON 表示形式。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: aae4b71055c7a6574cc4abbaa506fad8961991d9
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48581224"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="595ab-103">ColumnDefinition 资源</span><span class="sxs-lookup"><span data-stu-id="595ab-103">ColumnDefinition resource</span></span>

<span data-ttu-id="595ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="595ab-104">Namespace: microsoft.graph</span></span>

## <a name="json-representation"></a><span data-ttu-id="595ab-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="595ab-105">JSON representation</span></span>

<span data-ttu-id="595ab-106">下面是 ColumnDefinition 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="595ab-106">Here is a JSON representation of a ColumnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="595ab-107">属性</span><span class="sxs-lookup"><span data-stu-id="595ab-107">Properties</span></span>

<span data-ttu-id="595ab-108">**columnDefinition** 资源具有以下属性。</span><span class="sxs-lookup"><span data-stu-id="595ab-108">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="595ab-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="595ab-109">Property name</span></span>           | <span data-ttu-id="595ab-110">类型</span><span class="sxs-lookup"><span data-stu-id="595ab-110">Type</span></span>    | <span data-ttu-id="595ab-111">说明</span><span class="sxs-lookup"><span data-stu-id="595ab-111">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="595ab-112">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="595ab-112">**columnGroup**</span></span>         | <span data-ttu-id="595ab-113">string</span><span class="sxs-lookup"><span data-stu-id="595ab-113">string</span></span>  | <span data-ttu-id="595ab-114">对于网站列，此列所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="595ab-114">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="595ab-115">可以帮助组织相关的列。</span><span class="sxs-lookup"><span data-stu-id="595ab-115">Helps organize related columns.</span></span>
| <span data-ttu-id="595ab-116">**说明**</span><span class="sxs-lookup"><span data-stu-id="595ab-116">**description**</span></span>         | <span data-ttu-id="595ab-117">string</span><span class="sxs-lookup"><span data-stu-id="595ab-117">string</span></span>  | <span data-ttu-id="595ab-118">面向用户的列描述。</span><span class="sxs-lookup"><span data-stu-id="595ab-118">The user-facing description of the column.</span></span>
| <span data-ttu-id="595ab-119">**displayName**</span><span class="sxs-lookup"><span data-stu-id="595ab-119">**displayName**</span></span>         | <span data-ttu-id="595ab-120">string</span><span class="sxs-lookup"><span data-stu-id="595ab-120">string</span></span>  | <span data-ttu-id="595ab-121">面向用户的列名称。</span><span class="sxs-lookup"><span data-stu-id="595ab-121">The user-facing name of the column.</span></span>
| <span data-ttu-id="595ab-122">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="595ab-122">**enforceUniqueValues**</span></span> | <span data-ttu-id="595ab-123">boolean</span><span class="sxs-lookup"><span data-stu-id="595ab-123">boolean</span></span> | <span data-ttu-id="595ab-124">如果为 true，则此列不能有两个列表项具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="595ab-124">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="595ab-125">**hidden**</span><span class="sxs-lookup"><span data-stu-id="595ab-125">**hidden**</span></span>              | <span data-ttu-id="595ab-126">boolean</span><span class="sxs-lookup"><span data-stu-id="595ab-126">boolean</span></span> | <span data-ttu-id="595ab-127">指定列是否显示在用户界面中。</span><span class="sxs-lookup"><span data-stu-id="595ab-127">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="595ab-128">**id**</span><span class="sxs-lookup"><span data-stu-id="595ab-128">**id**</span></span>                  | <span data-ttu-id="595ab-129">string</span><span class="sxs-lookup"><span data-stu-id="595ab-129">string</span></span>  | <span data-ttu-id="595ab-130">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="595ab-130">The unique identifier for the column.</span></span>
| <span data-ttu-id="595ab-131">**indexed**</span><span class="sxs-lookup"><span data-stu-id="595ab-131">**indexed**</span></span>             | <span data-ttu-id="595ab-132">boolean</span><span class="sxs-lookup"><span data-stu-id="595ab-132">boolean</span></span> | <span data-ttu-id="595ab-133">指定列值是否可用于排序和搜索。</span><span class="sxs-lookup"><span data-stu-id="595ab-133">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="595ab-134">**name**</span><span class="sxs-lookup"><span data-stu-id="595ab-134">**name**</span></span>                | <span data-ttu-id="595ab-135">string</span><span class="sxs-lookup"><span data-stu-id="595ab-135">string</span></span>  | <span data-ttu-id="595ab-136">在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。</span><span class="sxs-lookup"><span data-stu-id="595ab-136">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="595ab-137">对于面向用户的名称，请参阅 **displayName**。</span><span class="sxs-lookup"><span data-stu-id="595ab-137">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="595ab-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="595ab-138">**readOnly**</span></span>            | <span data-ttu-id="595ab-139">bool</span><span class="sxs-lookup"><span data-stu-id="595ab-139">bool</span></span>    | <span data-ttu-id="595ab-140">指定是否可以修改列值。</span><span class="sxs-lookup"><span data-stu-id="595ab-140">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="595ab-141">**required**</span><span class="sxs-lookup"><span data-stu-id="595ab-141">**required**</span></span>            | <span data-ttu-id="595ab-142">boolean</span><span class="sxs-lookup"><span data-stu-id="595ab-142">boolean</span></span> | <span data-ttu-id="595ab-143">指定列值是否不可选。</span><span class="sxs-lookup"><span data-stu-id="595ab-143">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="595ab-144">列可以包含各种类型的数据。</span><span class="sxs-lookup"><span data-stu-id="595ab-144">Columns can hold data of various types.</span></span>
<span data-ttu-id="595ab-145">以下属性表示列存储的数据类型以及该数据的其他设置。</span><span class="sxs-lookup"><span data-stu-id="595ab-145">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="595ab-146">这些属性是互相排斥的 - 列只能指定其中一个。</span><span class="sxs-lookup"><span data-stu-id="595ab-146">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="595ab-147">属性名称</span><span class="sxs-lookup"><span data-stu-id="595ab-147">Property name</span></span>     | <span data-ttu-id="595ab-148">类型</span><span class="sxs-lookup"><span data-stu-id="595ab-148">Type</span></span>                    | <span data-ttu-id="595ab-149">说明</span><span class="sxs-lookup"><span data-stu-id="595ab-149">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="595ab-150">**boolean**</span><span class="sxs-lookup"><span data-stu-id="595ab-150">**boolean**</span></span>       | <span data-ttu-id="595ab-151">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="595ab-151">[booleanColumn][]</span></span>       | <span data-ttu-id="595ab-152">此列存储布尔值。</span><span class="sxs-lookup"><span data-stu-id="595ab-152">This column stores boolean values.</span></span>
| <span data-ttu-id="595ab-153">**calculated**</span><span class="sxs-lookup"><span data-stu-id="595ab-153">**calculated**</span></span>    | <span data-ttu-id="595ab-154">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="595ab-154">[calculatedColumn][]</span></span>    | <span data-ttu-id="595ab-155">根据其他列计算此列的数据。</span><span class="sxs-lookup"><span data-stu-id="595ab-155">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="595ab-156">**choice**</span><span class="sxs-lookup"><span data-stu-id="595ab-156">**choice**</span></span>        | <span data-ttu-id="595ab-157">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="595ab-157">[choiceColumn][]</span></span>        | <span data-ttu-id="595ab-158">此列存储所选列表中的数据。</span><span class="sxs-lookup"><span data-stu-id="595ab-158">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="595ab-159">**currency**</span><span class="sxs-lookup"><span data-stu-id="595ab-159">**currency**</span></span>      | <span data-ttu-id="595ab-160">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="595ab-160">[currencyColumn][]</span></span>      | <span data-ttu-id="595ab-161">此列存储货币值。</span><span class="sxs-lookup"><span data-stu-id="595ab-161">This column stores currency values.</span></span>
| <span data-ttu-id="595ab-162">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="595ab-162">**dateTime**</span></span>      | <span data-ttu-id="595ab-163">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="595ab-163">[dateTimeColumn][]</span></span>      | <span data-ttu-id="595ab-164">此列存储日期时间值。</span><span class="sxs-lookup"><span data-stu-id="595ab-164">This column stores DateTime values.</span></span>
| <span data-ttu-id="595ab-165">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="595ab-165">**defaultValue**</span></span>  | <span data-ttu-id="595ab-166">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="595ab-166">[defaultColumnValue][]</span></span>  | <span data-ttu-id="595ab-167">此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="595ab-167">The default value for this column.</span></span>
| <span data-ttu-id="595ab-168">**地理位置**</span><span class="sxs-lookup"><span data-stu-id="595ab-168">**geolocation**</span></span>   | <span data-ttu-id="595ab-169">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="595ab-169">[geolocationColumn][]</span></span>   | <span data-ttu-id="595ab-170">此列存储一个地理位置。</span><span class="sxs-lookup"><span data-stu-id="595ab-170">This column stores a geolocation.</span></span>
| <span data-ttu-id="595ab-171">**lookup**</span><span class="sxs-lookup"><span data-stu-id="595ab-171">**lookup**</span></span>        | <span data-ttu-id="595ab-172">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="595ab-172">[lookupColumn][]</span></span>        | <span data-ttu-id="595ab-173">从网站中的另一个源查找此列的数据。</span><span class="sxs-lookup"><span data-stu-id="595ab-173">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="595ab-174">**number**</span><span class="sxs-lookup"><span data-stu-id="595ab-174">**number**</span></span>        | <span data-ttu-id="595ab-175">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="595ab-175">[numberColumn][]</span></span>        | <span data-ttu-id="595ab-176">此列存储数值。</span><span class="sxs-lookup"><span data-stu-id="595ab-176">This column stores number values.</span></span>
| <span data-ttu-id="595ab-177">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="595ab-177">**personOrGroup**</span></span> | <span data-ttu-id="595ab-178">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="595ab-178">[personOrGroupColumn][]</span></span> | <span data-ttu-id="595ab-179">此列存储个人或组值。</span><span class="sxs-lookup"><span data-stu-id="595ab-179">This column stores Person or Group values.</span></span>
| <span data-ttu-id="595ab-180">**text**</span><span class="sxs-lookup"><span data-stu-id="595ab-180">**text**</span></span>          | <span data-ttu-id="595ab-181">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="595ab-181">[textColumn][]</span></span>          | <span data-ttu-id="595ab-182">此列存储文本值。</span><span class="sxs-lookup"><span data-stu-id="595ab-182">This column stores text values.</span></span>

<span data-ttu-id="595ab-183">注意：这些属性对应于 SharePoint 的 [SPFieldType][] 枚举。</span><span class="sxs-lookup"><span data-stu-id="595ab-183">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="595ab-184">虽然上面表示的是最常见的字段类型，但此 API 仍缺少一些。</span><span class="sxs-lookup"><span data-stu-id="595ab-184">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="595ab-185">在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。</span><span class="sxs-lookup"><span data-stu-id="595ab-185">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="595ab-186">备注</span><span class="sxs-lookup"><span data-stu-id="595ab-186">Remarks</span></span>

<span data-ttu-id="595ab-187">默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。</span><span class="sxs-lookup"><span data-stu-id="595ab-187">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="595ab-188">若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="595ab-188">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="595ab-189">若要在 [listItems][listItem] 上显示**字段**值时看到这些内容，请在 `$select` 语句中添加名称所需的列。</span><span class="sxs-lookup"><span data-stu-id="595ab-189">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

<span data-ttu-id="595ab-203">
  [SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span><span class="sxs-lookup"><span data-stu-id="595ab-203">[SPFieldType]: /previous-versions/office/sharepoint-server/ms428806(v=office.15)</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->