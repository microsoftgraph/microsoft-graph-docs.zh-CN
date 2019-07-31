---
title: workbookTableSort 资源类型
description: 管理对 Table 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ea0332f1ad00029cf511f2bc55aca80836e5ef2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007030"
---
# <a name="workbooktablesort-resource-type"></a><span data-ttu-id="019d9-103">workbookTableSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="019d9-103">workbookTableSort resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="019d9-104">管理对 Table 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="019d9-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="019d9-105">方法</span><span class="sxs-lookup"><span data-stu-id="019d9-105">Methods</span></span>

| <span data-ttu-id="019d9-106">方法</span><span class="sxs-lookup"><span data-stu-id="019d9-106">Method</span></span>           | <span data-ttu-id="019d9-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="019d9-107">Return Type</span></span>    |<span data-ttu-id="019d9-108">说明</span><span class="sxs-lookup"><span data-stu-id="019d9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="019d9-109">获取 TableSort</span><span class="sxs-lookup"><span data-stu-id="019d9-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="019d9-110">workbookTableSort</span><span class="sxs-lookup"><span data-stu-id="019d9-110">workbookTableSort</span></span>](workbooktablesort.md) |<span data-ttu-id="019d9-111">读取 tableSort 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="019d9-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="019d9-112">应用</span><span class="sxs-lookup"><span data-stu-id="019d9-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="019d9-113">无</span><span class="sxs-lookup"><span data-stu-id="019d9-113">None</span></span>|<span data-ttu-id="019d9-114">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="019d9-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="019d9-115">清除</span><span class="sxs-lookup"><span data-stu-id="019d9-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="019d9-116">None</span><span class="sxs-lookup"><span data-stu-id="019d9-116">None</span></span>|<span data-ttu-id="019d9-p101">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="019d9-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="019d9-119">重新应用</span><span class="sxs-lookup"><span data-stu-id="019d9-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="019d9-120">无</span><span class="sxs-lookup"><span data-stu-id="019d9-120">None</span></span>|<span data-ttu-id="019d9-121">对表重新应用当前的排序参数。</span><span class="sxs-lookup"><span data-stu-id="019d9-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="019d9-122">属性</span><span class="sxs-lookup"><span data-stu-id="019d9-122">Properties</span></span>
| <span data-ttu-id="019d9-123">属性</span><span class="sxs-lookup"><span data-stu-id="019d9-123">Property</span></span>     | <span data-ttu-id="019d9-124">类型</span><span class="sxs-lookup"><span data-stu-id="019d9-124">Type</span></span>   |<span data-ttu-id="019d9-125">说明</span><span class="sxs-lookup"><span data-stu-id="019d9-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="019d9-126">matchCase</span><span class="sxs-lookup"><span data-stu-id="019d9-126">matchCase</span></span>|<span data-ttu-id="019d9-127">boolean</span><span class="sxs-lookup"><span data-stu-id="019d9-127">boolean</span></span>|<span data-ttu-id="019d9-p102">表示最后一次对表进行排序时大小写是否有影响。只读。</span><span class="sxs-lookup"><span data-stu-id="019d9-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="019d9-130">方法</span><span class="sxs-lookup"><span data-stu-id="019d9-130">method</span></span>|<span data-ttu-id="019d9-131">string</span><span class="sxs-lookup"><span data-stu-id="019d9-131">string</span></span>|<span data-ttu-id="019d9-p103">表示最后一次对表排序所使用的中文字符排序方法。可能的值是：`PinYin`、`StrokeCount`。只读。</span><span class="sxs-lookup"><span data-stu-id="019d9-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="019d9-135">关系</span><span class="sxs-lookup"><span data-stu-id="019d9-135">Relationships</span></span>
| <span data-ttu-id="019d9-136">关系</span><span class="sxs-lookup"><span data-stu-id="019d9-136">Relationship</span></span> | <span data-ttu-id="019d9-137">类型</span><span class="sxs-lookup"><span data-stu-id="019d9-137">Type</span></span>   |<span data-ttu-id="019d9-138">说明</span><span class="sxs-lookup"><span data-stu-id="019d9-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="019d9-139">域</span><span class="sxs-lookup"><span data-stu-id="019d9-139">fields</span></span>|[<span data-ttu-id="019d9-140">workbookSortField</span><span class="sxs-lookup"><span data-stu-id="019d9-140">workbookSortField</span></span>](workbooksortfield.md)|<span data-ttu-id="019d9-141">表示最后一次对表排序所使用的当前条件。</span><span class="sxs-lookup"><span data-stu-id="019d9-141">Represents the current conditions used to last sort the table.</span></span> <span data-ttu-id="019d9-142">只读。</span><span class="sxs-lookup"><span data-stu-id="019d9-142">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="019d9-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="019d9-143">JSON representation</span></span>

<span data-ttu-id="019d9-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="019d9-144">Here is a JSON representation of the resource.</span></span>

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
