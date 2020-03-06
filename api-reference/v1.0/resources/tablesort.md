---
title: TableSort 资源类型
description: 管理对 Table 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 3772d0063fc19eb3a3c46953d5c85d8085f0a72a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533565"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="077ef-103">TableSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="077ef-103">TableSort resource type</span></span>

<span data-ttu-id="077ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="077ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="077ef-105">管理对 Table 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="077ef-105">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="077ef-106">Methods</span><span class="sxs-lookup"><span data-stu-id="077ef-106">Methods</span></span>

| <span data-ttu-id="077ef-107">方法</span><span class="sxs-lookup"><span data-stu-id="077ef-107">Method</span></span>           | <span data-ttu-id="077ef-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="077ef-108">Return Type</span></span>    |<span data-ttu-id="077ef-109">说明</span><span class="sxs-lookup"><span data-stu-id="077ef-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="077ef-110">获取 TableSort</span><span class="sxs-lookup"><span data-stu-id="077ef-110">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="077ef-111">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="077ef-111">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="077ef-112">读取 tableSort 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="077ef-112">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="077ef-113">应用</span><span class="sxs-lookup"><span data-stu-id="077ef-113">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="077ef-114">无</span><span class="sxs-lookup"><span data-stu-id="077ef-114">None</span></span>|<span data-ttu-id="077ef-115">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="077ef-115">Perform a sort operation.</span></span>|
|[<span data-ttu-id="077ef-116">清除</span><span class="sxs-lookup"><span data-stu-id="077ef-116">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="077ef-117">None</span><span class="sxs-lookup"><span data-stu-id="077ef-117">None</span></span>|<span data-ttu-id="077ef-p101">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="077ef-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="077ef-120">重新应用</span><span class="sxs-lookup"><span data-stu-id="077ef-120">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="077ef-121">无</span><span class="sxs-lookup"><span data-stu-id="077ef-121">None</span></span>|<span data-ttu-id="077ef-122">对表重新应用当前的排序参数。</span><span class="sxs-lookup"><span data-stu-id="077ef-122">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="077ef-123">属性</span><span class="sxs-lookup"><span data-stu-id="077ef-123">Properties</span></span>
| <span data-ttu-id="077ef-124">属性</span><span class="sxs-lookup"><span data-stu-id="077ef-124">Property</span></span>     | <span data-ttu-id="077ef-125">类型</span><span class="sxs-lookup"><span data-stu-id="077ef-125">Type</span></span>   |<span data-ttu-id="077ef-126">说明</span><span class="sxs-lookup"><span data-stu-id="077ef-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="077ef-127">域</span><span class="sxs-lookup"><span data-stu-id="077ef-127">fields</span></span>|<span data-ttu-id="077ef-128">[WorkbookSortField](sortfield.md)集合</span><span class="sxs-lookup"><span data-stu-id="077ef-128">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="077ef-129">表示最后一次对表排序所使用的当前条件。</span><span class="sxs-lookup"><span data-stu-id="077ef-129">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="077ef-130">只读。</span><span class="sxs-lookup"><span data-stu-id="077ef-130">Read-only.</span></span>|
|<span data-ttu-id="077ef-131">matchCase</span><span class="sxs-lookup"><span data-stu-id="077ef-131">matchCase</span></span>|<span data-ttu-id="077ef-132">boolean</span><span class="sxs-lookup"><span data-stu-id="077ef-132">boolean</span></span>|<span data-ttu-id="077ef-p103">表示最后一次对表进行排序时大小写是否有影响。只读。</span><span class="sxs-lookup"><span data-stu-id="077ef-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="077ef-135">方法</span><span class="sxs-lookup"><span data-stu-id="077ef-135">method</span></span>|<span data-ttu-id="077ef-136">string</span><span class="sxs-lookup"><span data-stu-id="077ef-136">string</span></span>|<span data-ttu-id="077ef-137">表示最后一次对表排序所使用的中文字符排序方法。</span><span class="sxs-lookup"><span data-stu-id="077ef-137">Represents Chinese character ordering method last used to sort the table.</span></span> <span data-ttu-id="077ef-138">可能的值为： `PinYin`、 `StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="077ef-138">The possible values are: `PinYin`, `StrokeCount`.</span></span> <span data-ttu-id="077ef-139">只读。</span><span class="sxs-lookup"><span data-stu-id="077ef-139">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="077ef-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="077ef-140">JSON representation</span></span>

<span data-ttu-id="077ef-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="077ef-141">Here is a JSON representation of the resource.</span></span>

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
