---
title: TableSort 资源类型
description: 管理对 Table 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 7e3eae5ef21bc8d8ea1fba395b369ea35d1f80b9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873043"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="6a8ff-103">TableSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a8ff-103">TableSort resource type</span></span>

> <span data-ttu-id="6a8ff-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6a8ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a8ff-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6a8ff-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a8ff-106">管理对 Table 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="6a8ff-106">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="6a8ff-107">方法</span><span class="sxs-lookup"><span data-stu-id="6a8ff-107">Methods</span></span>

| <span data-ttu-id="6a8ff-108">方法</span><span class="sxs-lookup"><span data-stu-id="6a8ff-108">Method</span></span>           | <span data-ttu-id="6a8ff-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="6a8ff-109">Return Type</span></span>    |<span data-ttu-id="6a8ff-110">说明</span><span class="sxs-lookup"><span data-stu-id="6a8ff-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6a8ff-111">获取 TableSort</span><span class="sxs-lookup"><span data-stu-id="6a8ff-111">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="6a8ff-112">TableSort</span><span class="sxs-lookup"><span data-stu-id="6a8ff-112">TableSort</span></span>](tablesort.md) |<span data-ttu-id="6a8ff-113">读取 tableSort 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6a8ff-113">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="6a8ff-114">应用</span><span class="sxs-lookup"><span data-stu-id="6a8ff-114">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="6a8ff-115">无</span><span class="sxs-lookup"><span data-stu-id="6a8ff-115">None</span></span>|<span data-ttu-id="6a8ff-116">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="6a8ff-116">Perform a sort operation.</span></span>|
|[<span data-ttu-id="6a8ff-117">Clear</span><span class="sxs-lookup"><span data-stu-id="6a8ff-117">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="6a8ff-118">无</span><span class="sxs-lookup"><span data-stu-id="6a8ff-118">None</span></span>|<span data-ttu-id="6a8ff-p102">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="6a8ff-p102">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="6a8ff-121">重新应用</span><span class="sxs-lookup"><span data-stu-id="6a8ff-121">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="6a8ff-122">无</span><span class="sxs-lookup"><span data-stu-id="6a8ff-122">None</span></span>|<span data-ttu-id="6a8ff-123">对表重新应用当前的排序参数。</span><span class="sxs-lookup"><span data-stu-id="6a8ff-123">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a8ff-124">属性</span><span class="sxs-lookup"><span data-stu-id="6a8ff-124">Properties</span></span>
| <span data-ttu-id="6a8ff-125">属性</span><span class="sxs-lookup"><span data-stu-id="6a8ff-125">Property</span></span>     | <span data-ttu-id="6a8ff-126">类型</span><span class="sxs-lookup"><span data-stu-id="6a8ff-126">Type</span></span>   |<span data-ttu-id="6a8ff-127">说明</span><span class="sxs-lookup"><span data-stu-id="6a8ff-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a8ff-128">matchCase</span><span class="sxs-lookup"><span data-stu-id="6a8ff-128">matchCase</span></span>|<span data-ttu-id="6a8ff-129">boolean</span><span class="sxs-lookup"><span data-stu-id="6a8ff-129">boolean</span></span>|<span data-ttu-id="6a8ff-p103">表示最后一次对表进行排序时大小写是否有影响。只读。</span><span class="sxs-lookup"><span data-stu-id="6a8ff-p103">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="6a8ff-132">方法</span><span class="sxs-lookup"><span data-stu-id="6a8ff-132">method</span></span>|<span data-ttu-id="6a8ff-133">string</span><span class="sxs-lookup"><span data-stu-id="6a8ff-133">string</span></span>|<span data-ttu-id="6a8ff-p104">表示最后一次对表排序所使用的中文字符排序方法。可能的值是：`PinYin`、`StrokeCount`。只读。</span><span class="sxs-lookup"><span data-stu-id="6a8ff-p104">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a8ff-137">Relationships</span><span class="sxs-lookup"><span data-stu-id="6a8ff-137">Relationships</span></span>
| <span data-ttu-id="6a8ff-138">关系</span><span class="sxs-lookup"><span data-stu-id="6a8ff-138">Relationship</span></span> | <span data-ttu-id="6a8ff-139">类型</span><span class="sxs-lookup"><span data-stu-id="6a8ff-139">Type</span></span>   |<span data-ttu-id="6a8ff-140">说明</span><span class="sxs-lookup"><span data-stu-id="6a8ff-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a8ff-141">fields</span><span class="sxs-lookup"><span data-stu-id="6a8ff-141">fields</span></span>|[<span data-ttu-id="6a8ff-142">SortField</span><span class="sxs-lookup"><span data-stu-id="6a8ff-142">SortField</span></span>](sortfield.md)|<span data-ttu-id="6a8ff-p105">表示最后一次对表排序所使用的当前条件。只读。</span><span class="sxs-lookup"><span data-stu-id="6a8ff-p105">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a8ff-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a8ff-145">JSON representation</span></span>

<span data-ttu-id="6a8ff-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a8ff-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string"
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
