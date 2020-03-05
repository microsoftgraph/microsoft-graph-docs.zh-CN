---
title: workbookRangeView 资源类型
description: RangeView 表示父范围的一组可见单元格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a8fb5810f43b415aee7a6151267bfd43e8644272
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519153"
---
# <a name="workbookrangeview-resource-type"></a><span data-ttu-id="3b65c-103">workbookRangeView 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b65c-103">workbookRangeView resource type</span></span>

<span data-ttu-id="3b65c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3b65c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b65c-105">RangeView 表示父范围的一组可见单元格。</span><span class="sxs-lookup"><span data-stu-id="3b65c-105">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="3b65c-106">方法</span><span class="sxs-lookup"><span data-stu-id="3b65c-106">Methods</span></span>

| <span data-ttu-id="3b65c-107">方法</span><span class="sxs-lookup"><span data-stu-id="3b65c-107">Method</span></span>           | <span data-ttu-id="3b65c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3b65c-108">Return Type</span></span>    |<span data-ttu-id="3b65c-109">说明</span><span class="sxs-lookup"><span data-stu-id="3b65c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3b65c-110">List rows</span><span class="sxs-lookup"><span data-stu-id="3b65c-110">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="3b65c-111">[workbookRangeView](workbookrangeview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b65c-111">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="3b65c-112">获取一组 workbookRangeView 对象。</span><span class="sxs-lookup"><span data-stu-id="3b65c-112">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="3b65c-113">Itemat</span><span class="sxs-lookup"><span data-stu-id="3b65c-113">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="3b65c-114">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="3b65c-114">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="3b65c-115">按索引获取范围视图项。</span><span class="sxs-lookup"><span data-stu-id="3b65c-115">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="3b65c-116">Range</span><span class="sxs-lookup"><span data-stu-id="3b65c-116">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="3b65c-117">workbookRange</span><span class="sxs-lookup"><span data-stu-id="3b65c-117">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="3b65c-118">返回与范围视图相关联的范围对象</span><span class="sxs-lookup"><span data-stu-id="3b65c-118">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="3b65c-119">属性</span><span class="sxs-lookup"><span data-stu-id="3b65c-119">Properties</span></span>
| <span data-ttu-id="3b65c-120">属性</span><span class="sxs-lookup"><span data-stu-id="3b65c-120">Property</span></span>     | <span data-ttu-id="3b65c-121">类型</span><span class="sxs-lookup"><span data-stu-id="3b65c-121">Type</span></span>   |<span data-ttu-id="3b65c-122">说明</span><span class="sxs-lookup"><span data-stu-id="3b65c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b65c-123">columnCount</span><span class="sxs-lookup"><span data-stu-id="3b65c-123">columnCount</span></span>|<span data-ttu-id="3b65c-124">Int32</span><span class="sxs-lookup"><span data-stu-id="3b65c-124">Int32</span></span>|<span data-ttu-id="3b65c-p101">返回可见列数。只读。</span><span class="sxs-lookup"><span data-stu-id="3b65c-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="3b65c-127">formulas</span><span class="sxs-lookup"><span data-stu-id="3b65c-127">formulas</span></span>|<span data-ttu-id="3b65c-128">Json</span><span class="sxs-lookup"><span data-stu-id="3b65c-128">Json</span></span>|<span data-ttu-id="3b65c-129">表示采用 A1 表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="3b65c-129">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="3b65c-130">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="3b65c-130">formulasLocal</span></span>|<span data-ttu-id="3b65c-131">Json</span><span class="sxs-lookup"><span data-stu-id="3b65c-131">Json</span></span>|<span data-ttu-id="3b65c-p102">表示采用 A1 表示法的公式，使用用户语言和数字格式区域设置。例如，英语中的公式 "=SUM(A1, 1.5)" 在德语中变为 "=SUMME(A1; 1,5)"。</span><span class="sxs-lookup"><span data-stu-id="3b65c-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="3b65c-134">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="3b65c-134">formulasR1C1</span></span>|<span data-ttu-id="3b65c-135">Json</span><span class="sxs-lookup"><span data-stu-id="3b65c-135">Json</span></span>|<span data-ttu-id="3b65c-136">表示采用 R1C1 样式表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="3b65c-136">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="3b65c-137">index</span><span class="sxs-lookup"><span data-stu-id="3b65c-137">index</span></span>|<span data-ttu-id="3b65c-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3b65c-138">Int32</span></span>|<span data-ttu-id="3b65c-139">范围的索引。</span><span class="sxs-lookup"><span data-stu-id="3b65c-139">Index of the range.</span></span>|
|<span data-ttu-id="3b65c-140">numberFormat</span><span class="sxs-lookup"><span data-stu-id="3b65c-140">numberFormat</span></span>|<span data-ttu-id="3b65c-141">Json</span><span class="sxs-lookup"><span data-stu-id="3b65c-141">Json</span></span>|<span data-ttu-id="3b65c-p103">表示 Excel 中指定单元格的数字格式代码。只读。</span><span class="sxs-lookup"><span data-stu-id="3b65c-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="3b65c-144">rowCount</span><span class="sxs-lookup"><span data-stu-id="3b65c-144">rowCount</span></span>|<span data-ttu-id="3b65c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="3b65c-145">Int32</span></span>|<span data-ttu-id="3b65c-p104">返回可见行数。只读。</span><span class="sxs-lookup"><span data-stu-id="3b65c-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="3b65c-148">text</span><span class="sxs-lookup"><span data-stu-id="3b65c-148">text</span></span>|<span data-ttu-id="3b65c-149">Json</span><span class="sxs-lookup"><span data-stu-id="3b65c-149">Json</span></span>|<span data-ttu-id="3b65c-p105">指定区域的文本值。文本值与单元格宽度无关。在 Excel UI 中替代 # 符号不会影响 API 返回的文本值。只读。</span><span class="sxs-lookup"><span data-stu-id="3b65c-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="3b65c-154">valueTypes</span><span class="sxs-lookup"><span data-stu-id="3b65c-154">valueTypes</span></span>|<span data-ttu-id="3b65c-155">Json</span><span class="sxs-lookup"><span data-stu-id="3b65c-155">Json</span></span>|<span data-ttu-id="3b65c-p106">表示每个单元格的数据类型。只读。可能的值是：Unknown、Empty、String、Integer、Double、Boolean、Error。</span><span class="sxs-lookup"><span data-stu-id="3b65c-p106">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="3b65c-159">values</span><span class="sxs-lookup"><span data-stu-id="3b65c-159">values</span></span>|<span data-ttu-id="3b65c-160">Json</span><span class="sxs-lookup"><span data-stu-id="3b65c-160">Json</span></span>|<span data-ttu-id="3b65c-p107">表示指定的 RangeView 的原始值。返回的数据可能是字符串、数字，也可能是布尔值。包含错误的单元格将返回错误字符串。</span><span class="sxs-lookup"><span data-stu-id="3b65c-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="3b65c-164">关系</span><span class="sxs-lookup"><span data-stu-id="3b65c-164">Relationships</span></span>
| <span data-ttu-id="3b65c-165">关系</span><span class="sxs-lookup"><span data-stu-id="3b65c-165">Relationship</span></span> | <span data-ttu-id="3b65c-166">类型</span><span class="sxs-lookup"><span data-stu-id="3b65c-166">Type</span></span>   |<span data-ttu-id="3b65c-167">说明</span><span class="sxs-lookup"><span data-stu-id="3b65c-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3b65c-168">rows</span><span class="sxs-lookup"><span data-stu-id="3b65c-168">rows</span></span>|<span data-ttu-id="3b65c-169">[workbookRangeView](workbookrangeview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b65c-169">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="3b65c-p108">表示一组与范围相关联的范围视图。只读。  只读。</span><span class="sxs-lookup"><span data-stu-id="3b65c-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3b65c-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b65c-173">JSON representation</span></span>
<span data-ttu-id="3b65c-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b65c-174">Here is a JSON representation of the resource.</span></span>
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
