---
title: workbookRangeView 资源类型
description: RangeView 表示父范围的一组可见单元格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b71f6eadcf110c2942cf02f43b3aa8b5db2db4cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007086"
---
# <a name="workbookrangeview-resource-type"></a><span data-ttu-id="6d5b8-103">workbookRangeView 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d5b8-103">workbookRangeView resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d5b8-104">RangeView 表示父范围的一组可见单元格。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="6d5b8-105">方法</span><span class="sxs-lookup"><span data-stu-id="6d5b8-105">Methods</span></span>

| <span data-ttu-id="6d5b8-106">方法</span><span class="sxs-lookup"><span data-stu-id="6d5b8-106">Method</span></span>           | <span data-ttu-id="6d5b8-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="6d5b8-107">Return Type</span></span>    |<span data-ttu-id="6d5b8-108">说明</span><span class="sxs-lookup"><span data-stu-id="6d5b8-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6d5b8-109">List rows</span><span class="sxs-lookup"><span data-stu-id="6d5b8-109">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="6d5b8-110">[workbookRangeView](workbookrangeview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6d5b8-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="6d5b8-111">获取一组 workbookRangeView 对象。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="6d5b8-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="6d5b8-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="6d5b8-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="6d5b8-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="6d5b8-114">按索引获取范围视图项。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="6d5b8-115">Range</span><span class="sxs-lookup"><span data-stu-id="6d5b8-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="6d5b8-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="6d5b8-116">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="6d5b8-117">返回与范围视图相关联的范围对象</span><span class="sxs-lookup"><span data-stu-id="6d5b8-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="6d5b8-118">属性</span><span class="sxs-lookup"><span data-stu-id="6d5b8-118">Properties</span></span>
| <span data-ttu-id="6d5b8-119">属性</span><span class="sxs-lookup"><span data-stu-id="6d5b8-119">Property</span></span>     | <span data-ttu-id="6d5b8-120">类型</span><span class="sxs-lookup"><span data-stu-id="6d5b8-120">Type</span></span>   |<span data-ttu-id="6d5b8-121">说明</span><span class="sxs-lookup"><span data-stu-id="6d5b8-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d5b8-122">columnCount</span><span class="sxs-lookup"><span data-stu-id="6d5b8-122">columnCount</span></span>|<span data-ttu-id="6d5b8-123">Int32</span><span class="sxs-lookup"><span data-stu-id="6d5b8-123">Int32</span></span>|<span data-ttu-id="6d5b8-p101">返回可见列数。只读。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="6d5b8-126">formulas</span><span class="sxs-lookup"><span data-stu-id="6d5b8-126">formulas</span></span>|<span data-ttu-id="6d5b8-127">Json</span><span class="sxs-lookup"><span data-stu-id="6d5b8-127">Json</span></span>|<span data-ttu-id="6d5b8-128">表示采用 A1 表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-128">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="6d5b8-129">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="6d5b8-129">formulasLocal</span></span>|<span data-ttu-id="6d5b8-130">Json</span><span class="sxs-lookup"><span data-stu-id="6d5b8-130">Json</span></span>|<span data-ttu-id="6d5b8-p102">表示采用 A1 表示法的公式，使用用户语言和数字格式区域设置。例如，英语中的公式 "=SUM(A1, 1.5)" 在德语中变为 "=SUMME(A1; 1,5)"。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="6d5b8-133">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="6d5b8-133">formulasR1C1</span></span>|<span data-ttu-id="6d5b8-134">Json</span><span class="sxs-lookup"><span data-stu-id="6d5b8-134">Json</span></span>|<span data-ttu-id="6d5b8-135">表示采用 R1C1 样式表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-135">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="6d5b8-136">index</span><span class="sxs-lookup"><span data-stu-id="6d5b8-136">index</span></span>|<span data-ttu-id="6d5b8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6d5b8-137">Int32</span></span>|<span data-ttu-id="6d5b8-138">范围的索引。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-138">Index of the range.</span></span>|
|<span data-ttu-id="6d5b8-139">numberFormat</span><span class="sxs-lookup"><span data-stu-id="6d5b8-139">numberFormat</span></span>|<span data-ttu-id="6d5b8-140">Json</span><span class="sxs-lookup"><span data-stu-id="6d5b8-140">Json</span></span>|<span data-ttu-id="6d5b8-p103">表示 Excel 中指定单元格的数字格式代码。只读。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="6d5b8-143">rowCount</span><span class="sxs-lookup"><span data-stu-id="6d5b8-143">rowCount</span></span>|<span data-ttu-id="6d5b8-144">Int32</span><span class="sxs-lookup"><span data-stu-id="6d5b8-144">Int32</span></span>|<span data-ttu-id="6d5b8-p104">返回可见行数。只读。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="6d5b8-147">text</span><span class="sxs-lookup"><span data-stu-id="6d5b8-147">text</span></span>|<span data-ttu-id="6d5b8-148">Json</span><span class="sxs-lookup"><span data-stu-id="6d5b8-148">Json</span></span>|<span data-ttu-id="6d5b8-p105">指定区域的文本值。文本值与单元格宽度无关。在 Excel UI 中替代 # 符号不会影响 API 返回的文本值。只读。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="6d5b8-153">valueTypes</span><span class="sxs-lookup"><span data-stu-id="6d5b8-153">valueTypes</span></span>|<span data-ttu-id="6d5b8-154">Json</span><span class="sxs-lookup"><span data-stu-id="6d5b8-154">Json</span></span>|<span data-ttu-id="6d5b8-p106">表示每个单元格的数据类型。只读。可能的值是：Unknown、Empty、String、Integer、Double、Boolean、Error。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-p106">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="6d5b8-158">values</span><span class="sxs-lookup"><span data-stu-id="6d5b8-158">values</span></span>|<span data-ttu-id="6d5b8-159">Json</span><span class="sxs-lookup"><span data-stu-id="6d5b8-159">Json</span></span>|<span data-ttu-id="6d5b8-p107">表示指定的 RangeView 的原始值。返回的数据可能是字符串、数字，也可能是布尔值。包含错误的单元格将返回错误字符串。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="6d5b8-163">关系</span><span class="sxs-lookup"><span data-stu-id="6d5b8-163">Relationships</span></span>
| <span data-ttu-id="6d5b8-164">关系</span><span class="sxs-lookup"><span data-stu-id="6d5b8-164">Relationship</span></span> | <span data-ttu-id="6d5b8-165">类型</span><span class="sxs-lookup"><span data-stu-id="6d5b8-165">Type</span></span>   |<span data-ttu-id="6d5b8-166">说明</span><span class="sxs-lookup"><span data-stu-id="6d5b8-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6d5b8-167">rows</span><span class="sxs-lookup"><span data-stu-id="6d5b8-167">rows</span></span>|<span data-ttu-id="6d5b8-168">[workbookRangeView](workbookrangeview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6d5b8-168">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="6d5b8-p108">表示一组与范围相关联的范围视图。只读。  只读。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6d5b8-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d5b8-172">JSON representation</span></span>
<span data-ttu-id="6d5b8-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d5b8-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "id": "String (identifier)",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
