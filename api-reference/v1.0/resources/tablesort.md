---
title: TableSort 资源类型
description: 管理对 Table 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: be607832be82b99853b4cd44cfa5b60449a2c432
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929471"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="87a15-103">TableSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="87a15-103">TableSort resource type</span></span>

<span data-ttu-id="87a15-104">管理对 Table 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="87a15-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="87a15-105">方法</span><span class="sxs-lookup"><span data-stu-id="87a15-105">Methods</span></span>

| <span data-ttu-id="87a15-106">方法</span><span class="sxs-lookup"><span data-stu-id="87a15-106">Method</span></span>           | <span data-ttu-id="87a15-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="87a15-107">Return Type</span></span>    |<span data-ttu-id="87a15-108">说明</span><span class="sxs-lookup"><span data-stu-id="87a15-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="87a15-109">获取 TableSort</span><span class="sxs-lookup"><span data-stu-id="87a15-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="87a15-110">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="87a15-110">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="87a15-111">读取 tableSort 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="87a15-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="87a15-112">应用</span><span class="sxs-lookup"><span data-stu-id="87a15-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="87a15-113">无</span><span class="sxs-lookup"><span data-stu-id="87a15-113">None</span></span>|<span data-ttu-id="87a15-114">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="87a15-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="87a15-115">Clear</span><span class="sxs-lookup"><span data-stu-id="87a15-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="87a15-116">无</span><span class="sxs-lookup"><span data-stu-id="87a15-116">None</span></span>|<span data-ttu-id="87a15-p101">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="87a15-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="87a15-119">重新应用</span><span class="sxs-lookup"><span data-stu-id="87a15-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="87a15-120">无</span><span class="sxs-lookup"><span data-stu-id="87a15-120">None</span></span>|<span data-ttu-id="87a15-121">对表重新应用当前的排序参数。</span><span class="sxs-lookup"><span data-stu-id="87a15-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="87a15-122">属性</span><span class="sxs-lookup"><span data-stu-id="87a15-122">Properties</span></span>
| <span data-ttu-id="87a15-123">属性</span><span class="sxs-lookup"><span data-stu-id="87a15-123">Property</span></span>     | <span data-ttu-id="87a15-124">类型</span><span class="sxs-lookup"><span data-stu-id="87a15-124">Type</span></span>   |<span data-ttu-id="87a15-125">说明</span><span class="sxs-lookup"><span data-stu-id="87a15-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87a15-126">fields</span><span class="sxs-lookup"><span data-stu-id="87a15-126">fields</span></span>|<span data-ttu-id="87a15-127">[WorkbookSortField](sortfield.md)集合</span><span class="sxs-lookup"><span data-stu-id="87a15-127">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="87a15-p102">表示最后一次对表排序所使用的当前条件。只读。</span><span class="sxs-lookup"><span data-stu-id="87a15-p102">Represents the current conditions used to last sort the table. Read-only.</span></span>|
|<span data-ttu-id="87a15-130">matchCase</span><span class="sxs-lookup"><span data-stu-id="87a15-130">matchCase</span></span>|<span data-ttu-id="87a15-131">boolean</span><span class="sxs-lookup"><span data-stu-id="87a15-131">boolean</span></span>|<span data-ttu-id="87a15-p103">表示最后一次对表进行排序时大小写是否有影响。只读。</span><span class="sxs-lookup"><span data-stu-id="87a15-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="87a15-134">方法</span><span class="sxs-lookup"><span data-stu-id="87a15-134">method</span></span>|<span data-ttu-id="87a15-135">string</span><span class="sxs-lookup"><span data-stu-id="87a15-135">string</span></span>|<span data-ttu-id="87a15-136">代表中文排序方法上次使用的表进行排序的字符。</span><span class="sxs-lookup"><span data-stu-id="87a15-136">Represents Chinese character ordering method last used to sort the table.</span></span> <span data-ttu-id="87a15-137">可能的值为： `PinYin`， `StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="87a15-137">The possible values are: `PinYin`, `StrokeCount`.</span></span> <span data-ttu-id="87a15-138">只读。</span><span class="sxs-lookup"><span data-stu-id="87a15-138">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="87a15-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="87a15-139">JSON representation</span></span>

<span data-ttu-id="87a15-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="87a15-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string",
  "fields": [{ "@odata.type": "microsoft.graph.workbookSortField" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
