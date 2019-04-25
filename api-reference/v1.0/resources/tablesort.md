---
title: TableSort 资源类型
description: 管理对 Table 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: be607832be82b99853b4cd44cfa5b60449a2c432
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534512"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="57b99-103">TableSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="57b99-103">TableSort resource type</span></span>

<span data-ttu-id="57b99-104">管理对 Table 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="57b99-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="57b99-105">方法</span><span class="sxs-lookup"><span data-stu-id="57b99-105">Methods</span></span>

| <span data-ttu-id="57b99-106">方法</span><span class="sxs-lookup"><span data-stu-id="57b99-106">Method</span></span>           | <span data-ttu-id="57b99-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="57b99-107">Return Type</span></span>    |<span data-ttu-id="57b99-108">说明</span><span class="sxs-lookup"><span data-stu-id="57b99-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="57b99-109">获取 TableSort</span><span class="sxs-lookup"><span data-stu-id="57b99-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="57b99-110">WorkbookTableSort</span><span class="sxs-lookup"><span data-stu-id="57b99-110">WorkbookTableSort</span></span>](tablesort.md) |<span data-ttu-id="57b99-111">读取 tableSort 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="57b99-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="57b99-112">应用</span><span class="sxs-lookup"><span data-stu-id="57b99-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="57b99-113">无</span><span class="sxs-lookup"><span data-stu-id="57b99-113">None</span></span>|<span data-ttu-id="57b99-114">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="57b99-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="57b99-115">清除</span><span class="sxs-lookup"><span data-stu-id="57b99-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="57b99-116">None</span><span class="sxs-lookup"><span data-stu-id="57b99-116">None</span></span>|<span data-ttu-id="57b99-p101">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="57b99-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="57b99-119">重新应用</span><span class="sxs-lookup"><span data-stu-id="57b99-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="57b99-120">无</span><span class="sxs-lookup"><span data-stu-id="57b99-120">None</span></span>|<span data-ttu-id="57b99-121">对表重新应用当前的排序参数。</span><span class="sxs-lookup"><span data-stu-id="57b99-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="57b99-122">属性</span><span class="sxs-lookup"><span data-stu-id="57b99-122">Properties</span></span>
| <span data-ttu-id="57b99-123">属性</span><span class="sxs-lookup"><span data-stu-id="57b99-123">Property</span></span>     | <span data-ttu-id="57b99-124">类型</span><span class="sxs-lookup"><span data-stu-id="57b99-124">Type</span></span>   |<span data-ttu-id="57b99-125">说明</span><span class="sxs-lookup"><span data-stu-id="57b99-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57b99-126">域</span><span class="sxs-lookup"><span data-stu-id="57b99-126">fields</span></span>|<span data-ttu-id="57b99-127">[WorkbookSortField](sortfield.md)集合</span><span class="sxs-lookup"><span data-stu-id="57b99-127">[WorkbookSortField](sortfield.md) collection</span></span>|<span data-ttu-id="57b99-128">表示最后一次对表排序所使用的当前条件。</span><span class="sxs-lookup"><span data-stu-id="57b99-128">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="57b99-129">只读。</span><span class="sxs-lookup"><span data-stu-id="57b99-129">Read-only.</span></span>|
|<span data-ttu-id="57b99-130">matchCase</span><span class="sxs-lookup"><span data-stu-id="57b99-130">matchCase</span></span>|<span data-ttu-id="57b99-131">boolean</span><span class="sxs-lookup"><span data-stu-id="57b99-131">boolean</span></span>|<span data-ttu-id="57b99-p103">表示最后一次对表进行排序时大小写是否有影响。只读。</span><span class="sxs-lookup"><span data-stu-id="57b99-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="57b99-134">方法</span><span class="sxs-lookup"><span data-stu-id="57b99-134">method</span></span>|<span data-ttu-id="57b99-135">string</span><span class="sxs-lookup"><span data-stu-id="57b99-135">string</span></span>|<span data-ttu-id="57b99-136">表示最后一次对表排序所使用的中文字符排序方法。</span><span class="sxs-lookup"><span data-stu-id="57b99-136">Represents Chinese character ordering method last used to sort the table.</span></span> <span data-ttu-id="57b99-137">可能的值为: `PinYin`、 `StrokeCount`。</span><span class="sxs-lookup"><span data-stu-id="57b99-137">The possible values are: `PinYin`, `StrokeCount`.</span></span> <span data-ttu-id="57b99-138">只读。</span><span class="sxs-lookup"><span data-stu-id="57b99-138">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57b99-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57b99-139">JSON representation</span></span>

<span data-ttu-id="57b99-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57b99-140">Here is a JSON representation of the resource.</span></span>

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
