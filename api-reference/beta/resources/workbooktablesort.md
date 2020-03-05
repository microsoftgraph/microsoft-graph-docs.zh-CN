---
title: workbookTableSort 资源类型
description: 管理对 Table 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 422c1836317d7299b2e485d578561dda6e1bab91
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519111"
---
# <a name="workbooktablesort-resource-type"></a><span data-ttu-id="a01d7-103">workbookTableSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="a01d7-103">workbookTableSort resource type</span></span>

<span data-ttu-id="a01d7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a01d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a01d7-105">管理对 Table 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="a01d7-105">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="a01d7-106">方法</span><span class="sxs-lookup"><span data-stu-id="a01d7-106">Methods</span></span>

| <span data-ttu-id="a01d7-107">方法</span><span class="sxs-lookup"><span data-stu-id="a01d7-107">Method</span></span>           | <span data-ttu-id="a01d7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a01d7-108">Return Type</span></span>    |<span data-ttu-id="a01d7-109">说明</span><span class="sxs-lookup"><span data-stu-id="a01d7-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a01d7-110">获取 TableSort</span><span class="sxs-lookup"><span data-stu-id="a01d7-110">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="a01d7-111">workbookTableSort</span><span class="sxs-lookup"><span data-stu-id="a01d7-111">workbookTableSort</span></span>](workbooktablesort.md) |<span data-ttu-id="a01d7-112">读取 tableSort 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a01d7-112">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="a01d7-113">应用</span><span class="sxs-lookup"><span data-stu-id="a01d7-113">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="a01d7-114">无</span><span class="sxs-lookup"><span data-stu-id="a01d7-114">None</span></span>|<span data-ttu-id="a01d7-115">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="a01d7-115">Perform a sort operation.</span></span>|
|[<span data-ttu-id="a01d7-116">清除</span><span class="sxs-lookup"><span data-stu-id="a01d7-116">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="a01d7-117">None</span><span class="sxs-lookup"><span data-stu-id="a01d7-117">None</span></span>|<span data-ttu-id="a01d7-p101">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="a01d7-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="a01d7-120">重新应用</span><span class="sxs-lookup"><span data-stu-id="a01d7-120">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="a01d7-121">无</span><span class="sxs-lookup"><span data-stu-id="a01d7-121">None</span></span>|<span data-ttu-id="a01d7-122">对表重新应用当前的排序参数。</span><span class="sxs-lookup"><span data-stu-id="a01d7-122">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="a01d7-123">属性</span><span class="sxs-lookup"><span data-stu-id="a01d7-123">Properties</span></span>
| <span data-ttu-id="a01d7-124">属性</span><span class="sxs-lookup"><span data-stu-id="a01d7-124">Property</span></span>     | <span data-ttu-id="a01d7-125">类型</span><span class="sxs-lookup"><span data-stu-id="a01d7-125">Type</span></span>   |<span data-ttu-id="a01d7-126">说明</span><span class="sxs-lookup"><span data-stu-id="a01d7-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a01d7-127">matchCase</span><span class="sxs-lookup"><span data-stu-id="a01d7-127">matchCase</span></span>|<span data-ttu-id="a01d7-128">boolean</span><span class="sxs-lookup"><span data-stu-id="a01d7-128">boolean</span></span>|<span data-ttu-id="a01d7-p102">表示最后一次对表进行排序时大小写是否有影响。只读。</span><span class="sxs-lookup"><span data-stu-id="a01d7-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="a01d7-131">方法</span><span class="sxs-lookup"><span data-stu-id="a01d7-131">method</span></span>|<span data-ttu-id="a01d7-132">string</span><span class="sxs-lookup"><span data-stu-id="a01d7-132">string</span></span>|<span data-ttu-id="a01d7-p103">表示最后一次对表排序所使用的中文字符排序方法。可能的值是：`PinYin`、`StrokeCount`。只读。</span><span class="sxs-lookup"><span data-stu-id="a01d7-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a01d7-136">关系</span><span class="sxs-lookup"><span data-stu-id="a01d7-136">Relationships</span></span>
| <span data-ttu-id="a01d7-137">关系</span><span class="sxs-lookup"><span data-stu-id="a01d7-137">Relationship</span></span> | <span data-ttu-id="a01d7-138">类型</span><span class="sxs-lookup"><span data-stu-id="a01d7-138">Type</span></span>   |<span data-ttu-id="a01d7-139">说明</span><span class="sxs-lookup"><span data-stu-id="a01d7-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a01d7-140">域</span><span class="sxs-lookup"><span data-stu-id="a01d7-140">fields</span></span>|[<span data-ttu-id="a01d7-141">workbookSortField</span><span class="sxs-lookup"><span data-stu-id="a01d7-141">workbookSortField</span></span>](workbooksortfield.md)|<span data-ttu-id="a01d7-142">表示最后一次对表排序所使用的当前条件。</span><span class="sxs-lookup"><span data-stu-id="a01d7-142">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="a01d7-143">只读。</span><span class="sxs-lookup"><span data-stu-id="a01d7-143">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a01d7-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a01d7-144">JSON representation</span></span>

<span data-ttu-id="a01d7-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a01d7-145">Here is a JSON representation of the resource.</span></span>

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
