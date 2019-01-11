---
title: rangeView 资源类型
description: RangeView 表示父范围的一组可见单元格。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c356c737946dc70c6718b71c1c9aa7081069fd96
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859001"
---
# <a name="rangeview-resource-type"></a><span data-ttu-id="1408a-103">rangeView 资源类型</span><span class="sxs-lookup"><span data-stu-id="1408a-103">rangeView resource type</span></span>

> <span data-ttu-id="1408a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1408a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1408a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1408a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1408a-106">RangeView 表示父范围的一组可见单元格。</span><span class="sxs-lookup"><span data-stu-id="1408a-106">RangeView represents a set of visible cells of the parent range.</span></span>

## <a name="methods"></a><span data-ttu-id="1408a-107">方法</span><span class="sxs-lookup"><span data-stu-id="1408a-107">Methods</span></span>

| <span data-ttu-id="1408a-108">方法</span><span class="sxs-lookup"><span data-stu-id="1408a-108">Method</span></span>           | <span data-ttu-id="1408a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1408a-109">Return Type</span></span>    |<span data-ttu-id="1408a-110">说明</span><span class="sxs-lookup"><span data-stu-id="1408a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1408a-111">List rows</span><span class="sxs-lookup"><span data-stu-id="1408a-111">List rows</span></span>](../api/workbookrangeview-list-rows.md) |<span data-ttu-id="1408a-112">[workbookRangeView](workbookrangeview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1408a-112">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="1408a-113">获取一组 workbookRangeView 对象。</span><span class="sxs-lookup"><span data-stu-id="1408a-113">Get a workbookRangeView object collection.</span></span>|
|[<span data-ttu-id="1408a-114">Itemat</span><span class="sxs-lookup"><span data-stu-id="1408a-114">Itemat</span></span>](../api/workbookrangeview-itemat.md)|[<span data-ttu-id="1408a-115">workbookRangeView</span><span class="sxs-lookup"><span data-stu-id="1408a-115">workbookRangeView</span></span>](workbookrangeview.md)|<span data-ttu-id="1408a-116">按索引获取范围视图项。</span><span class="sxs-lookup"><span data-stu-id="1408a-116">Get a range view item based in index.</span></span>|
|[<span data-ttu-id="1408a-117">Range</span><span class="sxs-lookup"><span data-stu-id="1408a-117">Range</span></span>](../api/workbookrangeview-range.md)|[<span data-ttu-id="1408a-118">workbookRange</span><span class="sxs-lookup"><span data-stu-id="1408a-118">workbookRange</span></span>](range.md)|<span data-ttu-id="1408a-119">返回与范围视图相关联的范围对象</span><span class="sxs-lookup"><span data-stu-id="1408a-119">Return the range object associated with the range view</span></span>|

## <a name="properties"></a><span data-ttu-id="1408a-120">属性</span><span class="sxs-lookup"><span data-stu-id="1408a-120">Properties</span></span>
| <span data-ttu-id="1408a-121">属性</span><span class="sxs-lookup"><span data-stu-id="1408a-121">Property</span></span>     | <span data-ttu-id="1408a-122">类型</span><span class="sxs-lookup"><span data-stu-id="1408a-122">Type</span></span>   |<span data-ttu-id="1408a-123">说明</span><span class="sxs-lookup"><span data-stu-id="1408a-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1408a-124">columnCount</span><span class="sxs-lookup"><span data-stu-id="1408a-124">columnCount</span></span>|<span data-ttu-id="1408a-125">Int32</span><span class="sxs-lookup"><span data-stu-id="1408a-125">Int32</span></span>|<span data-ttu-id="1408a-p102">返回可见列数。只读。</span><span class="sxs-lookup"><span data-stu-id="1408a-p102">Returns the number of visible columns. Read-only.</span></span>|
|<span data-ttu-id="1408a-128">formulas</span><span class="sxs-lookup"><span data-stu-id="1408a-128">formulas</span></span>|<span data-ttu-id="1408a-129">Json</span><span class="sxs-lookup"><span data-stu-id="1408a-129">Json</span></span>|<span data-ttu-id="1408a-130">表示采用 A1 表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="1408a-130">Represents the formula in A1-style notation.</span></span> |
|<span data-ttu-id="1408a-131">formulasLocal</span><span class="sxs-lookup"><span data-stu-id="1408a-131">formulasLocal</span></span>|<span data-ttu-id="1408a-132">Json</span><span class="sxs-lookup"><span data-stu-id="1408a-132">Json</span></span>|<span data-ttu-id="1408a-p103">表示采用 A1 表示法的公式，使用用户语言和数字格式区域设置。例如，英语中的公式 "=SUM(A1, 1.5)" 在德语中变为 "=SUMME(A1; 1,5)"。</span><span class="sxs-lookup"><span data-stu-id="1408a-p103">Represents the formula in A1-style notation, in the user's language and number-formatting locale. For example, the English "=SUM(A1, 1.5)" formula would become "=SUMME(A1; 1,5)" in German.</span></span>    |
|<span data-ttu-id="1408a-135">formulasR1C1</span><span class="sxs-lookup"><span data-stu-id="1408a-135">formulasR1C1</span></span>|<span data-ttu-id="1408a-136">Json</span><span class="sxs-lookup"><span data-stu-id="1408a-136">Json</span></span>|<span data-ttu-id="1408a-137">表示采用 R1C1 表示法的公式。</span><span class="sxs-lookup"><span data-stu-id="1408a-137">Represents the formula in R1C1-style notation.</span></span>   |
|<span data-ttu-id="1408a-138">index</span><span class="sxs-lookup"><span data-stu-id="1408a-138">index</span></span>|<span data-ttu-id="1408a-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1408a-139">Int32</span></span>|<span data-ttu-id="1408a-140">范围的索引。</span><span class="sxs-lookup"><span data-stu-id="1408a-140">Index of the range.</span></span>|
|<span data-ttu-id="1408a-141">numberFormat</span><span class="sxs-lookup"><span data-stu-id="1408a-141">numberFormat</span></span>|<span data-ttu-id="1408a-142">Json</span><span class="sxs-lookup"><span data-stu-id="1408a-142">Json</span></span>|<span data-ttu-id="1408a-p104">表示 Excel 中指定单元格的数字格式代码。只读。</span><span class="sxs-lookup"><span data-stu-id="1408a-p104">Represents Excel's number format code for the given cell. Read-only.</span></span> |
|<span data-ttu-id="1408a-145">rowCount</span><span class="sxs-lookup"><span data-stu-id="1408a-145">rowCount</span></span>|<span data-ttu-id="1408a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1408a-146">Int32</span></span>|<span data-ttu-id="1408a-p105">返回可见行数。只读。</span><span class="sxs-lookup"><span data-stu-id="1408a-p105">Returns the number of visible rows. Read-only.</span></span>  |
|<span data-ttu-id="1408a-149">text</span><span class="sxs-lookup"><span data-stu-id="1408a-149">text</span></span>|<span data-ttu-id="1408a-150">Json</span><span class="sxs-lookup"><span data-stu-id="1408a-150">Json</span></span>|<span data-ttu-id="1408a-p106">指定区域的文本值。文本值与单元格宽度无关。在 Excel UI 中替代 # 符号不会影响 API 返回的文本值。只读。</span><span class="sxs-lookup"><span data-stu-id="1408a-p106">Text values of the specified range. The Text value will not depend on the cell width. The # sign substitution that happens in Excel UI will not affect the text value returned by the API. Read-only.</span></span>    |
|<span data-ttu-id="1408a-155">valueTypes</span><span class="sxs-lookup"><span data-stu-id="1408a-155">valueTypes</span></span>|<span data-ttu-id="1408a-156">Json</span><span class="sxs-lookup"><span data-stu-id="1408a-156">Json</span></span>|<span data-ttu-id="1408a-p107">表示每个单元格的数据类型。只读。可能的值是：Unknown、Empty、String、Integer、Double、Boolean、Error。</span><span class="sxs-lookup"><span data-stu-id="1408a-p107">Represents the type of data of each cell. Read-only. Possible values are: Unknown, Empty, String, Integer, Double, Boolean, Error.</span></span> |
|<span data-ttu-id="1408a-160">values</span><span class="sxs-lookup"><span data-stu-id="1408a-160">values</span></span>|<span data-ttu-id="1408a-161">Json</span><span class="sxs-lookup"><span data-stu-id="1408a-161">Json</span></span>|<span data-ttu-id="1408a-p108">表示指定的 RangeView 的原始值。返回的数据可能是字符串、数字，也可能是布尔值。包含错误的单元格将返回错误字符串。</span><span class="sxs-lookup"><span data-stu-id="1408a-p108">Represents the raw values of the specified range view. The data returned could be of type string, number, or a boolean. Cell that contain an error will return the error string.</span></span>   |

## <a name="relationships"></a><span data-ttu-id="1408a-165">关系</span><span class="sxs-lookup"><span data-stu-id="1408a-165">Relationships</span></span>
| <span data-ttu-id="1408a-166">关系</span><span class="sxs-lookup"><span data-stu-id="1408a-166">Relationship</span></span> | <span data-ttu-id="1408a-167">类型</span><span class="sxs-lookup"><span data-stu-id="1408a-167">Type</span></span>   |<span data-ttu-id="1408a-168">说明</span><span class="sxs-lookup"><span data-stu-id="1408a-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1408a-169">rows</span><span class="sxs-lookup"><span data-stu-id="1408a-169">rows</span></span>|<span data-ttu-id="1408a-170">[workbookRangeView](workbookrangeview.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1408a-170">[workbookRangeView](workbookrangeview.md) collection</span></span>| <span data-ttu-id="1408a-p109">表示一组与范围相关联的范围视图。只读。  只读。</span><span class="sxs-lookup"><span data-stu-id="1408a-p109">Represents a collection of range views associated with the range. Read-only.    Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1408a-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1408a-174">JSON representation</span></span>
<span data-ttu-id="1408a-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1408a-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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
  "id": "String (identifier)",
  "index": 1024,
  "numberFormat": "Json",
  "rowCount": 1024,
  "text": "Json",
  "valueTypes": "Json",
  "values": "Json"
}
```
