---
title: rangeView 资源类型
description: RangeView 表示父范围的一组可见单元格。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 0fae95999de35b5bac42716a4c9ec8b16a5b1158
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810078"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="8c962-103">rangeView 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c962-103">rangeView resource type</span></span>
<span data-ttu-id="8c962-104">RangeView 表示父范围的一组可见单元格。</span><span class="sxs-lookup"><span data-stu-id="8c962-104">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="8c962-105">方法</span><span class="sxs-lookup"><span data-stu-id="8c962-105">Methods</span></span>

| <span data-ttu-id="8c962-106">方法</span><span class="sxs-lookup"><span data-stu-id="8c962-106">Method</span></span>           | <span data-ttu-id="8c962-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="8c962-107">Return Type</span></span>    |<span data-ttu-id="8c962-108">说明</span><span class="sxs-lookup"><span data-stu-id="8c962-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8c962-109">List rows</span><span class="sxs-lookup"><span data-stu-id="8c962-109">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="8c962-110">[workbookRangeView](workbookrangeview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8c962-110">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="8c962-111">获取一组 workbookRangeView 对象。</span><span class="sxs-lookup"><span data-stu-id="8c962-111">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="8c962-112">Itemat</span><span class="sxs-lookup"><span data-stu-id="8c962-112">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="8c962-113">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="8c962-113">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="8c962-114">按索引获取范围视图项。</span><span class="sxs-lookup"><span data-stu-id="8c962-114">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="8c962-115">Range</span><span class="sxs-lookup"><span data-stu-id="8c962-115">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="8c962-116">workbookRange</span><span class="sxs-lookup"><span data-stu-id="8c962-116">workbookRange</span></span>](range.md)|<span data-ttu-id="8c962-117">返回与范围视图相关联的范围对象</span><span class="sxs-lookup"><span data-stu-id="8c962-117">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="8c962-118">属性</span><span class="sxs-lookup"><span data-stu-id="8c962-118">Properties</span></span>
| <span data-ttu-id="8c962-119">属性</span><span class="sxs-lookup"><span data-stu-id="8c962-119">Property</span></span>     | <span data-ttu-id="8c962-120">类型</span><span class="sxs-lookup"><span data-stu-id="8c962-120">Type</span></span>   |<span data-ttu-id="8c962-121">Description</span><span class="sxs-lookup"><span data-stu-id="8c962-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c962-122">cellAddresses</span><span class="sxs-lookup"><span data-stu-id="8c962-122">cellAddresses</span></span>|<span data-ttu-id="8c962-123">Json</span><span class="sxs-lookup"><span data-stu-id="8c962-123">Json</span></span>|<span data-ttu-id="8c962-124">代表单元格地址</span><span class="sxs-lookup"><span data-stu-id="8c962-124">Represents the cell addresses</span></span>
|<span data-ttu-id="8c962-125">columnCount</span><span class="sxs-lookup"><span data-stu-id="8c962-125">columnCount</span></span>|<span data-ttu-id="8c962-126">Int32</span><span class="sxs-lookup"><span data-stu-id="8c962-126">Int32</span></span>|<span data-ttu-id="8c962-p101">返回可见列数。只读。</span><span class="sxs-lookup"><span data-stu-id="8c962-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="8c962-129">formulas</span><span class="sxs-lookup"><span data-stu-id="8c962-129">formulas</span></span>|<span data-ttu-id="8c962-130">Json</span><span class="sxs-lookup"><span data-stu-id="8c962-130">Json</span></span>|<span data-ttu-id="8c962-131">表示采用 A1 表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="8c962-131">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="8c962-132">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="8c962-132">formulasLocal</span></span>|<span data-ttu-id="8c962-133">Json</span><span class="sxs-lookup"><span data-stu-id="8c962-133">Json</span></span>|<span data-ttu-id="8c962-p102">表示采用 A1 表示法的公式，使用用户语言和数字格式区域设置。例如，英语中的公式 "=SUM(A1, 1.5)" 在德语中变为 "=SUMME(A1; 1,5)"。</span><span class="sxs-lookup"><span data-stu-id="8c962-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="8c962-136">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="8c962-136">formulasR1C1</span></span>|<span data-ttu-id="8c962-137">Json</span><span class="sxs-lookup"><span data-stu-id="8c962-137">Json</span></span>|<span data-ttu-id="8c962-138">表示采用 R1C1 表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="8c962-138">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="8c962-139">index</span><span class="sxs-lookup"><span data-stu-id="8c962-139">index</span></span>|<span data-ttu-id="8c962-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8c962-140">Int32</span></span>|<span data-ttu-id="8c962-141">范围的索引。</span><span class="sxs-lookup"><span data-stu-id="8c962-141">Index of the range.</span></span>|
|<span data-ttu-id="8c962-142">numberFormat</span><span class="sxs-lookup"><span data-stu-id="8c962-142">numberFormat</span></span>|<span data-ttu-id="8c962-143">Json</span><span class="sxs-lookup"><span data-stu-id="8c962-143">Json</span></span>|<span data-ttu-id="8c962-p103">表示 Excel 中指定单元格的数字格式代码。只读。</span><span class="sxs-lookup"><span data-stu-id="8c962-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="8c962-146">rowCount</span><span class="sxs-lookup"><span data-stu-id="8c962-146">rowCount</span></span>|<span data-ttu-id="8c962-147">Int32</span><span class="sxs-lookup"><span data-stu-id="8c962-147">Int32</span></span>|<span data-ttu-id="8c962-p104">返回可见行数。只读。</span><span class="sxs-lookup"><span data-stu-id="8c962-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="8c962-150">text</span><span class="sxs-lookup"><span data-stu-id="8c962-150">text</span></span>|<span data-ttu-id="8c962-151">Json</span><span class="sxs-lookup"><span data-stu-id="8c962-151">Json</span></span>|<span data-ttu-id="8c962-p105">指定区域的文本值。文本值与单元格宽度无关。在 Excel UI 中替代 # 符号不会影响 API 返回的文本值。只读。</span><span class="sxs-lookup"><span data-stu-id="8c962-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="8c962-156">valueTypes</span><span class="sxs-lookup"><span data-stu-id="8c962-156">valueTypes</span></span>|<span data-ttu-id="8c962-157">Json</span><span class="sxs-lookup"><span data-stu-id="8c962-157">Json</span></span>|<span data-ttu-id="8c962-158">表示每个单元格的数据的类型。</span><span class="sxs-lookup"><span data-stu-id="8c962-158">Represents the type of data of each cell.</span></span> <span data-ttu-id="8c962-159">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="8c962-159">Read-only.</span></span> <span data-ttu-id="8c962-160">可能的值为： 未知、 空、 String、 Integer、 Double、 Boolean、 错误。</span><span class="sxs-lookup"><span data-stu-id="8c962-160">The possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="8c962-161">values</span><span class="sxs-lookup"><span data-stu-id="8c962-161">values</span></span>|<span data-ttu-id="8c962-162">Json</span><span class="sxs-lookup"><span data-stu-id="8c962-162">Json</span></span>|<span data-ttu-id="8c962-p107">表示指定的 RangeView 的原始值。返回的数据可能是字符串、数字，也可能是布尔值。包含错误的单元格将返回错误字符串。</span><span class="sxs-lookup"><span data-stu-id="8c962-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="8c962-166">关系</span><span class="sxs-lookup"><span data-stu-id="8c962-166">Relationships</span></span>
| <span data-ttu-id="8c962-167">关系</span><span class="sxs-lookup"><span data-stu-id="8c962-167">Relationship</span></span> | <span data-ttu-id="8c962-168">类型</span><span class="sxs-lookup"><span data-stu-id="8c962-168">Type</span></span>   |<span data-ttu-id="8c962-169">说明</span><span class="sxs-lookup"><span data-stu-id="8c962-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c962-170">rows</span><span class="sxs-lookup"><span data-stu-id="8c962-170">rows</span></span>|<span data-ttu-id="8c962-171">[workbookRangeView](workbookrangeview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8c962-171">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="8c962-p108">表示一组与范围相关联的范围视图。只读。  只读。</span><span class="sxs-lookup"><span data-stu-id="8c962-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c962-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c962-175">JSON representation</span></span>
<span data-ttu-id="8c962-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c962-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookRangeView"
}-->
```json
{
  "cellAddresses": "Json",
  "columnCount": 1024,
  "formulas": "Json",
  "formulasLocal": "Json",
  "formulasR1C1": "Json",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
