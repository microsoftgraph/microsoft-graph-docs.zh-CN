---
title: workbookRangeView 资源类型
description: RangeView 表示父范围的一组可见单元格。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: da469982ba0f5adf8c6387057d21f31b6d977baa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046172"
---
# <a name="workbookrangeview-resource-type"></a><span data-ttu-id="7f949-103">workbookRangeView 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f949-103">workbookRangeView resource type</span></span>

<span data-ttu-id="7f949-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f949-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f949-105">RangeView 表示父范围的一组可见单元格。</span><span class="sxs-lookup"><span data-stu-id="7f949-105">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="7f949-106">方法</span><span class="sxs-lookup"><span data-stu-id="7f949-106">Methods</span></span>

| <span data-ttu-id="7f949-107">方法</span><span class="sxs-lookup"><span data-stu-id="7f949-107">Method</span></span>           | <span data-ttu-id="7f949-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="7f949-108">Return Type</span></span>    |<span data-ttu-id="7f949-109">说明</span><span class="sxs-lookup"><span data-stu-id="7f949-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f949-110">List rows</span><span class="sxs-lookup"><span data-stu-id="7f949-110">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="7f949-111">[workbookRangeView](workbookrangeview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7f949-111">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="7f949-112">获取一组 workbookRangeView 对象。</span><span class="sxs-lookup"><span data-stu-id="7f949-112">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="7f949-113">Itemat</span><span class="sxs-lookup"><span data-stu-id="7f949-113">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="7f949-114">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="7f949-114">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="7f949-115">按索引获取范围视图项。</span><span class="sxs-lookup"><span data-stu-id="7f949-115">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="7f949-116">Range</span><span class="sxs-lookup"><span data-stu-id="7f949-116">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="7f949-117">workbookRange</span><span class="sxs-lookup"><span data-stu-id="7f949-117">workbookRange</span></span>](workbookrange.md)|<span data-ttu-id="7f949-118">返回与范围视图相关联的范围对象</span><span class="sxs-lookup"><span data-stu-id="7f949-118">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="7f949-119">属性</span><span class="sxs-lookup"><span data-stu-id="7f949-119">Properties</span></span>
| <span data-ttu-id="7f949-120">属性</span><span class="sxs-lookup"><span data-stu-id="7f949-120">Property</span></span>     | <span data-ttu-id="7f949-121">类型</span><span class="sxs-lookup"><span data-stu-id="7f949-121">Type</span></span>   |<span data-ttu-id="7f949-122">说明</span><span class="sxs-lookup"><span data-stu-id="7f949-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f949-123">columnCount</span><span class="sxs-lookup"><span data-stu-id="7f949-123">columnCount</span></span>|<span data-ttu-id="7f949-124">Int32</span><span class="sxs-lookup"><span data-stu-id="7f949-124">Int32</span></span>|<span data-ttu-id="7f949-p101">返回可见列数。只读。</span><span class="sxs-lookup"><span data-stu-id="7f949-p101">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="7f949-127">formulas</span><span class="sxs-lookup"><span data-stu-id="7f949-127">formulas</span></span>|<span data-ttu-id="7f949-128">Json</span><span class="sxs-lookup"><span data-stu-id="7f949-128">Json</span></span>|<span data-ttu-id="7f949-129">表示采用 A1 表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="7f949-129">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="7f949-130">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="7f949-130">formulasLocal</span></span>|<span data-ttu-id="7f949-131">Json</span><span class="sxs-lookup"><span data-stu-id="7f949-131">Json</span></span>|<span data-ttu-id="7f949-p102">表示采用 A1 表示法的公式，使用用户语言和数字格式区域设置。例如，英语中的公式 "=SUM(A1, 1.5)" 在德语中变为 "=SUMME(A1; 1,5)"。</span><span class="sxs-lookup"><span data-stu-id="7f949-p102">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="7f949-134">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="7f949-134">formulasR1C1</span></span>|<span data-ttu-id="7f949-135">Json</span><span class="sxs-lookup"><span data-stu-id="7f949-135">Json</span></span>|<span data-ttu-id="7f949-136">表示采用 R1C1 样式表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="7f949-136">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="7f949-137">index</span><span class="sxs-lookup"><span data-stu-id="7f949-137">index</span></span>|<span data-ttu-id="7f949-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7f949-138">Int32</span></span>|<span data-ttu-id="7f949-139">范围的索引。</span><span class="sxs-lookup"><span data-stu-id="7f949-139">Index of the range.</span></span>|
|<span data-ttu-id="7f949-140">numberFormat</span><span class="sxs-lookup"><span data-stu-id="7f949-140">numberFormat</span></span>|<span data-ttu-id="7f949-141">Json</span><span class="sxs-lookup"><span data-stu-id="7f949-141">Json</span></span>|<span data-ttu-id="7f949-p103">表示 Excel 中指定单元格的数字格式代码。只读。</span><span class="sxs-lookup"><span data-stu-id="7f949-p103">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="7f949-144">rowCount</span><span class="sxs-lookup"><span data-stu-id="7f949-144">rowCount</span></span>|<span data-ttu-id="7f949-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7f949-145">Int32</span></span>|<span data-ttu-id="7f949-p104">返回可见行数。只读。</span><span class="sxs-lookup"><span data-stu-id="7f949-p104">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="7f949-148">text</span><span class="sxs-lookup"><span data-stu-id="7f949-148">text</span></span>|<span data-ttu-id="7f949-149">Json</span><span class="sxs-lookup"><span data-stu-id="7f949-149">Json</span></span>|<span data-ttu-id="7f949-p105">指定区域的文本值。文本值与单元格宽度无关。在 Excel UI 中替代 # 符号不会影响 API 返回的文本值。只读。</span><span class="sxs-lookup"><span data-stu-id="7f949-p105">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="7f949-154">valueTypes</span><span class="sxs-lookup"><span data-stu-id="7f949-154">valueTypes</span></span>|<span data-ttu-id="7f949-155">Json</span><span class="sxs-lookup"><span data-stu-id="7f949-155">Json</span></span>|<span data-ttu-id="7f949-p106">表示每个单元格的数据类型。只读。可能的值是：Unknown、Empty、String、Integer、Double、Boolean、Error。</span><span class="sxs-lookup"><span data-stu-id="7f949-p106">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="7f949-159">values</span><span class="sxs-lookup"><span data-stu-id="7f949-159">values</span></span>|<span data-ttu-id="7f949-160">Json</span><span class="sxs-lookup"><span data-stu-id="7f949-160">Json</span></span>|<span data-ttu-id="7f949-p107">表示指定的 RangeView 的原始值。返回的数据可能是字符串、数字，也可能是布尔值。包含错误的单元格将返回错误字符串。</span><span class="sxs-lookup"><span data-stu-id="7f949-p107">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="7f949-164">关系</span><span class="sxs-lookup"><span data-stu-id="7f949-164">Relationships</span></span>
| <span data-ttu-id="7f949-165">关系</span><span class="sxs-lookup"><span data-stu-id="7f949-165">Relationship</span></span> | <span data-ttu-id="7f949-166">类型</span><span class="sxs-lookup"><span data-stu-id="7f949-166">Type</span></span>   |<span data-ttu-id="7f949-167">说明</span><span class="sxs-lookup"><span data-stu-id="7f949-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f949-168">rows</span><span class="sxs-lookup"><span data-stu-id="7f949-168">rows</span></span>|<span data-ttu-id="7f949-169">[workbookRangeView](workbookrangeview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7f949-169">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="7f949-p108">表示一组与范围相关联的范围视图。只读。  只读。</span><span class="sxs-lookup"><span data-stu-id="7f949-p108">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f949-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f949-173">JSON representation</span></span>
<span data-ttu-id="7f949-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f949-174">Here is a JSON representation of the resource.</span></span>
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


