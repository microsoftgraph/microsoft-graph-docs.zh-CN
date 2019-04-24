---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: ddd6b3c6d3048bf7a6d3ab2dbc8ff7259651ee2f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460618"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="8c340-102">columnDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c340-102">columnDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="8c340-103">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c340-103">JSON representation</span></span>

<span data-ttu-id="8c340-104">下面是 columnDefinition 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c340-104">Here is a JSON representation of a columnDefinition resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8c340-105">属性</span><span class="sxs-lookup"><span data-stu-id="8c340-105">Properties</span></span>

<span data-ttu-id="8c340-106">列可以包含各种类型的数据。</span><span class="sxs-lookup"><span data-stu-id="8c340-106">Columns can hold data of various types.</span></span>
<span data-ttu-id="8c340-107">以下属性表示列存储的数据类型以及该数据的其他设置。</span><span class="sxs-lookup"><span data-stu-id="8c340-107">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="8c340-108">与类型相关的属性 (boolean、计算、choice、currency、dateTime、lookup、number、personOrGroup、text) 是相互排斥的--一个列只能有一个指定的属性。</span><span class="sxs-lookup"><span data-stu-id="8c340-108">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="8c340-109">属性名称</span><span class="sxs-lookup"><span data-stu-id="8c340-109">Property name</span></span>           | <span data-ttu-id="8c340-110">类型</span><span class="sxs-lookup"><span data-stu-id="8c340-110">Type</span></span>    | <span data-ttu-id="8c340-111">说明</span><span class="sxs-lookup"><span data-stu-id="8c340-111">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="8c340-112">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="8c340-112">**columnGroup**</span></span>         | <span data-ttu-id="8c340-113">字符串</span><span class="sxs-lookup"><span data-stu-id="8c340-113">string</span></span>  | <span data-ttu-id="8c340-114">对于网站列，此列所属的组的名称。</span><span class="sxs-lookup"><span data-stu-id="8c340-114">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="8c340-115">可以帮助组织相关的列。</span><span class="sxs-lookup"><span data-stu-id="8c340-115">Helps organize related columns.</span></span>
| <span data-ttu-id="8c340-116">**说明**</span><span class="sxs-lookup"><span data-stu-id="8c340-116">**description**</span></span>         | <span data-ttu-id="8c340-117">字符串</span><span class="sxs-lookup"><span data-stu-id="8c340-117">string</span></span>  | <span data-ttu-id="8c340-118">面向用户的列描述。</span><span class="sxs-lookup"><span data-stu-id="8c340-118">The user-facing description of the column.</span></span>
| <span data-ttu-id="8c340-119">**displayName**</span><span class="sxs-lookup"><span data-stu-id="8c340-119">**displayName**</span></span>         | <span data-ttu-id="8c340-120">string</span><span class="sxs-lookup"><span data-stu-id="8c340-120">string</span></span>  | <span data-ttu-id="8c340-121">面向用户的列名称。</span><span class="sxs-lookup"><span data-stu-id="8c340-121">The user-facing name of the column.</span></span>
| <span data-ttu-id="8c340-122">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="8c340-122">**enforceUniqueValues**</span></span> | <span data-ttu-id="8c340-123">布尔</span><span class="sxs-lookup"><span data-stu-id="8c340-123">boolean</span></span> | <span data-ttu-id="8c340-124">如果为 true，则此列不能有两个列表项具有相同的值。</span><span class="sxs-lookup"><span data-stu-id="8c340-124">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="8c340-125">**hidden**</span><span class="sxs-lookup"><span data-stu-id="8c340-125">**hidden**</span></span>              | <span data-ttu-id="8c340-126">布尔</span><span class="sxs-lookup"><span data-stu-id="8c340-126">boolean</span></span> | <span data-ttu-id="8c340-127">指定列是否显示在用户界面中。</span><span class="sxs-lookup"><span data-stu-id="8c340-127">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="8c340-128">**id**</span><span class="sxs-lookup"><span data-stu-id="8c340-128">**id**</span></span>                  | <span data-ttu-id="8c340-129">string</span><span class="sxs-lookup"><span data-stu-id="8c340-129">string</span></span>  | <span data-ttu-id="8c340-130">列的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8c340-130">The unique identifier for the column.</span></span>
| <span data-ttu-id="8c340-131">**indexed**</span><span class="sxs-lookup"><span data-stu-id="8c340-131">**indexed**</span></span>             | <span data-ttu-id="8c340-132">布尔</span><span class="sxs-lookup"><span data-stu-id="8c340-132">boolean</span></span> | <span data-ttu-id="8c340-133">指定列值是否可用于排序和搜索。</span><span class="sxs-lookup"><span data-stu-id="8c340-133">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="8c340-134">**name**</span><span class="sxs-lookup"><span data-stu-id="8c340-134">**name**</span></span>                | <span data-ttu-id="8c340-135">string</span><span class="sxs-lookup"><span data-stu-id="8c340-135">string</span></span>  | <span data-ttu-id="8c340-136">在 [listItem][] 上的 [fields][] 中显示的面向 API 的列名称。</span><span class="sxs-lookup"><span data-stu-id="8c340-136">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="8c340-137">对于面向用户的名称，请参阅 **displayName**。</span><span class="sxs-lookup"><span data-stu-id="8c340-137">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="8c340-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="8c340-138">**readOnly**</span></span>            | <span data-ttu-id="8c340-139">bool</span><span class="sxs-lookup"><span data-stu-id="8c340-139">bool</span></span>    | <span data-ttu-id="8c340-140">指定是否可以修改列值。</span><span class="sxs-lookup"><span data-stu-id="8c340-140">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="8c340-141">**required**</span><span class="sxs-lookup"><span data-stu-id="8c340-141">**required**</span></span>            | <span data-ttu-id="8c340-142">boolean</span><span class="sxs-lookup"><span data-stu-id="8c340-142">boolean</span></span> | <span data-ttu-id="8c340-143">指定列值是否不可选。</span><span class="sxs-lookup"><span data-stu-id="8c340-143">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="8c340-144">**boolean**</span><span class="sxs-lookup"><span data-stu-id="8c340-144">**boolean**</span></span>       | <span data-ttu-id="8c340-145">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="8c340-145">[booleanColumn][]</span></span>       | <span data-ttu-id="8c340-146">此列存储布尔值。</span><span class="sxs-lookup"><span data-stu-id="8c340-146">This column stores boolean values.</span></span>
| <span data-ttu-id="8c340-147">**calculated**</span><span class="sxs-lookup"><span data-stu-id="8c340-147">**calculated**</span></span>    | <span data-ttu-id="8c340-148">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="8c340-148">[calculatedColumn][]</span></span>    | <span data-ttu-id="8c340-149">根据其他列计算此列的数据。</span><span class="sxs-lookup"><span data-stu-id="8c340-149">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="8c340-150">**choice**</span><span class="sxs-lookup"><span data-stu-id="8c340-150">**choice**</span></span>        | <span data-ttu-id="8c340-151">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="8c340-151">[choiceColumn][]</span></span>        | <span data-ttu-id="8c340-152">此列存储所选列表中的数据。</span><span class="sxs-lookup"><span data-stu-id="8c340-152">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="8c340-153">**currency**</span><span class="sxs-lookup"><span data-stu-id="8c340-153">**currency**</span></span>      | <span data-ttu-id="8c340-154">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="8c340-154">[currencyColumn][]</span></span>      | <span data-ttu-id="8c340-155">此列存储货币值。</span><span class="sxs-lookup"><span data-stu-id="8c340-155">This column stores currency values.</span></span>
| <span data-ttu-id="8c340-156">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="8c340-156">**dateTime**</span></span>      | <span data-ttu-id="8c340-157">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="8c340-157">[dateTimeColumn][]</span></span>      | <span data-ttu-id="8c340-158">此列存储日期时间值。</span><span class="sxs-lookup"><span data-stu-id="8c340-158">This column stores DateTime values.</span></span>
| <span data-ttu-id="8c340-159">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="8c340-159">**defaultValue**</span></span>  | <span data-ttu-id="8c340-160">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="8c340-160">[defaultColumnValue][]</span></span>  | <span data-ttu-id="8c340-161">此列的默认值。</span><span class="sxs-lookup"><span data-stu-id="8c340-161">The default value for this column.</span></span>
| <span data-ttu-id="8c340-162">**地理位置**</span><span class="sxs-lookup"><span data-stu-id="8c340-162">**geolocation**</span></span>   | <span data-ttu-id="8c340-163">[geolocationColumn][]</span><span class="sxs-lookup"><span data-stu-id="8c340-163">[geolocationColumn][]</span></span>   | <span data-ttu-id="8c340-164">此列存储一个地理位置。</span><span class="sxs-lookup"><span data-stu-id="8c340-164">This column stores a geolocation.</span></span>
| <span data-ttu-id="8c340-165">**lookup**</span><span class="sxs-lookup"><span data-stu-id="8c340-165">**lookup**</span></span>        | <span data-ttu-id="8c340-166">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="8c340-166">[lookupColumn][]</span></span>        | <span data-ttu-id="8c340-167">从网站中的另一个源查找此列的数据。</span><span class="sxs-lookup"><span data-stu-id="8c340-167">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="8c340-168">**number**</span><span class="sxs-lookup"><span data-stu-id="8c340-168">**number**</span></span>        | <span data-ttu-id="8c340-169">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="8c340-169">[numberColumn][]</span></span>        | <span data-ttu-id="8c340-170">此列存储数值。</span><span class="sxs-lookup"><span data-stu-id="8c340-170">This column stores number values.</span></span>
| <span data-ttu-id="8c340-171">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="8c340-171">**personOrGroup**</span></span> | <span data-ttu-id="8c340-172">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="8c340-172">[personOrGroupColumn][]</span></span> | <span data-ttu-id="8c340-173">此列存储个人或组值。</span><span class="sxs-lookup"><span data-stu-id="8c340-173">This column stores Person or Group values.</span></span>
| <span data-ttu-id="8c340-174">**text**</span><span class="sxs-lookup"><span data-stu-id="8c340-174">**text**</span></span>          | <span data-ttu-id="8c340-175">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="8c340-175">[textColumn][]</span></span>          | <span data-ttu-id="8c340-176">此列存储文本值。</span><span class="sxs-lookup"><span data-stu-id="8c340-176">This column stores text values.</span></span>

><span data-ttu-id="8c340-177">**注意:** 这些属性对应于 SharePoint 的[SPFieldType][]枚举。</span><span class="sxs-lookup"><span data-stu-id="8c340-177">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="8c340-178">虽然在上表中表示的是最常见的字段类型, 但此 beta API 仍缺少一些。</span><span class="sxs-lookup"><span data-stu-id="8c340-178">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="8c340-179">在这些情况下，不会填充列类型 facet，列将仅具有其基本属性。</span><span class="sxs-lookup"><span data-stu-id="8c340-179">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="8c340-180">备注</span><span class="sxs-lookup"><span data-stu-id="8c340-180">Remarks</span></span>

<span data-ttu-id="8c340-181">默认情况下，不显示 `hidden` 列的 ColumnDefinitions 和字段值。</span><span class="sxs-lookup"><span data-stu-id="8c340-181">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="8c340-182">若要在列出 **columnDefinitions** 时看到这些内容，请在 `$select` 语句中添加 `hidden`。</span><span class="sxs-lookup"><span data-stu-id="8c340-182">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="8c340-183">若要在 [listItems][listItem] 上显示**字段**值时看到这些内容，请在 `$select` 语句中添加名称所需的列。</span><span class="sxs-lookup"><span data-stu-id="8c340-183">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

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

<span data-ttu-id="8c340-197">
  [SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span><span class="sxs-lookup"><span data-stu-id="8c340-197">[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": [
    "Error: /api-reference/beta/resources/columndefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
