---
title: workbookTableSort 资源类型
description: 管理对 Table 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 77f4fb1dcaed54c2b4cd992b7d6105e194812149
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023742"
---
# <a name="workbooktablesort-resource-type"></a><span data-ttu-id="a521c-103">workbookTableSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="a521c-103">workbookTableSort resource type</span></span>

<span data-ttu-id="a521c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a521c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a521c-105">管理对 Table 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="a521c-105">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="a521c-106">方法</span><span class="sxs-lookup"><span data-stu-id="a521c-106">Methods</span></span>

| <span data-ttu-id="a521c-107">方法</span><span class="sxs-lookup"><span data-stu-id="a521c-107">Method</span></span>           | <span data-ttu-id="a521c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a521c-108">Return Type</span></span>    |<span data-ttu-id="a521c-109">说明</span><span class="sxs-lookup"><span data-stu-id="a521c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a521c-110">获取 TableSort</span><span class="sxs-lookup"><span data-stu-id="a521c-110">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="a521c-111">workbookTableSort</span><span class="sxs-lookup"><span data-stu-id="a521c-111">workbookTableSort</span></span>](workbooktablesort.md) |<span data-ttu-id="a521c-112">读取 tableSort 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a521c-112">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="a521c-113">应用</span><span class="sxs-lookup"><span data-stu-id="a521c-113">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="a521c-114">无</span><span class="sxs-lookup"><span data-stu-id="a521c-114">None</span></span>|<span data-ttu-id="a521c-115">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="a521c-115">Perform a sort operation.</span></span>|
|[<span data-ttu-id="a521c-116">清除</span><span class="sxs-lookup"><span data-stu-id="a521c-116">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="a521c-117">None</span><span class="sxs-lookup"><span data-stu-id="a521c-117">None</span></span>|<span data-ttu-id="a521c-p101">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="a521c-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="a521c-120">重新应用</span><span class="sxs-lookup"><span data-stu-id="a521c-120">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="a521c-121">无</span><span class="sxs-lookup"><span data-stu-id="a521c-121">None</span></span>|<span data-ttu-id="a521c-122">对表重新应用当前的排序参数。</span><span class="sxs-lookup"><span data-stu-id="a521c-122">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="a521c-123">属性</span><span class="sxs-lookup"><span data-stu-id="a521c-123">Properties</span></span>
| <span data-ttu-id="a521c-124">属性</span><span class="sxs-lookup"><span data-stu-id="a521c-124">Property</span></span>     | <span data-ttu-id="a521c-125">类型</span><span class="sxs-lookup"><span data-stu-id="a521c-125">Type</span></span>   |<span data-ttu-id="a521c-126">说明</span><span class="sxs-lookup"><span data-stu-id="a521c-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a521c-127">matchCase</span><span class="sxs-lookup"><span data-stu-id="a521c-127">matchCase</span></span>|<span data-ttu-id="a521c-128">boolean</span><span class="sxs-lookup"><span data-stu-id="a521c-128">boolean</span></span>|<span data-ttu-id="a521c-p102">表示最后一次对表进行排序时大小写是否有影响。只读。</span><span class="sxs-lookup"><span data-stu-id="a521c-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="a521c-131">方法</span><span class="sxs-lookup"><span data-stu-id="a521c-131">method</span></span>|<span data-ttu-id="a521c-132">string</span><span class="sxs-lookup"><span data-stu-id="a521c-132">string</span></span>|<span data-ttu-id="a521c-p103">表示最后一次对表排序所使用的中文字符排序方法。可能的值是：`PinYin`、`StrokeCount`。只读。</span><span class="sxs-lookup"><span data-stu-id="a521c-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a521c-136">关系</span><span class="sxs-lookup"><span data-stu-id="a521c-136">Relationships</span></span>
| <span data-ttu-id="a521c-137">关系</span><span class="sxs-lookup"><span data-stu-id="a521c-137">Relationship</span></span> | <span data-ttu-id="a521c-138">类型</span><span class="sxs-lookup"><span data-stu-id="a521c-138">Type</span></span>   |<span data-ttu-id="a521c-139">说明</span><span class="sxs-lookup"><span data-stu-id="a521c-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a521c-140">域</span><span class="sxs-lookup"><span data-stu-id="a521c-140">fields</span></span>|[<span data-ttu-id="a521c-141">workbookSortField</span><span class="sxs-lookup"><span data-stu-id="a521c-141">workbookSortField</span></span>](workbooksortfield.md)|<span data-ttu-id="a521c-142">表示最后一次对表排序所使用的当前条件。</span><span class="sxs-lookup"><span data-stu-id="a521c-142">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="a521c-143">只读。</span><span class="sxs-lookup"><span data-stu-id="a521c-143">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a521c-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a521c-144">JSON representation</span></span>

<span data-ttu-id="a521c-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a521c-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
 
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableSort"
}-->

```json
{
  "id": "string",
  "matchCase": true,
  "method": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


