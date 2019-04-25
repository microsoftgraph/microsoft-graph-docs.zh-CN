---
title: TableSort 资源类型
description: 管理对 Table 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 612e0cb7d59011f04ae992f80119fc1da572b582
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583205"
---
# <a name="tablesort-resource-type"></a><span data-ttu-id="b5d3c-103">TableSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5d3c-103">TableSort resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5d3c-104">管理对 Table 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="b5d3c-104">Manages sorting operations on Table objects.</span></span>


## <a name="methods"></a><span data-ttu-id="b5d3c-105">方法</span><span class="sxs-lookup"><span data-stu-id="b5d3c-105">Methods</span></span>

| <span data-ttu-id="b5d3c-106">方法</span><span class="sxs-lookup"><span data-stu-id="b5d3c-106">Method</span></span>           | <span data-ttu-id="b5d3c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="b5d3c-107">Return Type</span></span>    |<span data-ttu-id="b5d3c-108">说明</span><span class="sxs-lookup"><span data-stu-id="b5d3c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b5d3c-109">获取 TableSort</span><span class="sxs-lookup"><span data-stu-id="b5d3c-109">Get TableSort</span></span>](../api/tablesort-get.md) | [<span data-ttu-id="b5d3c-110">TableSort</span><span class="sxs-lookup"><span data-stu-id="b5d3c-110">TableSort</span></span>](tablesort.md) |<span data-ttu-id="b5d3c-111">读取 tableSort 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b5d3c-111">Read properties and relationships of tableSort object.</span></span>|
|[<span data-ttu-id="b5d3c-112">应用</span><span class="sxs-lookup"><span data-stu-id="b5d3c-112">Apply</span></span>](../api/tablesort-apply.md)|<span data-ttu-id="b5d3c-113">无</span><span class="sxs-lookup"><span data-stu-id="b5d3c-113">None</span></span>|<span data-ttu-id="b5d3c-114">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="b5d3c-114">Perform a sort operation.</span></span>|
|[<span data-ttu-id="b5d3c-115">清除</span><span class="sxs-lookup"><span data-stu-id="b5d3c-115">Clear</span></span>](../api/tablesort-clear.md)|<span data-ttu-id="b5d3c-116">None</span><span class="sxs-lookup"><span data-stu-id="b5d3c-116">None</span></span>|<span data-ttu-id="b5d3c-p101">清除表上的当前排序。尽管这不能修改表的排序，但它会清除标题按钮的状态。</span><span class="sxs-lookup"><span data-stu-id="b5d3c-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>|
|[<span data-ttu-id="b5d3c-119">重新应用</span><span class="sxs-lookup"><span data-stu-id="b5d3c-119">Reapply</span></span>](../api/tablesort-reapply.md)|<span data-ttu-id="b5d3c-120">无</span><span class="sxs-lookup"><span data-stu-id="b5d3c-120">None</span></span>|<span data-ttu-id="b5d3c-121">对表重新应用当前的排序参数。</span><span class="sxs-lookup"><span data-stu-id="b5d3c-121">Reapplies the current sorting parameters to the table.</span></span>|

## <a name="properties"></a><span data-ttu-id="b5d3c-122">属性</span><span class="sxs-lookup"><span data-stu-id="b5d3c-122">Properties</span></span>
| <span data-ttu-id="b5d3c-123">属性</span><span class="sxs-lookup"><span data-stu-id="b5d3c-123">Property</span></span>     | <span data-ttu-id="b5d3c-124">类型</span><span class="sxs-lookup"><span data-stu-id="b5d3c-124">Type</span></span>   |<span data-ttu-id="b5d3c-125">说明</span><span class="sxs-lookup"><span data-stu-id="b5d3c-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5d3c-126">matchCase</span><span class="sxs-lookup"><span data-stu-id="b5d3c-126">matchCase</span></span>|<span data-ttu-id="b5d3c-127">boolean</span><span class="sxs-lookup"><span data-stu-id="b5d3c-127">boolean</span></span>|<span data-ttu-id="b5d3c-p102">表示最后一次对表进行排序时大小写是否有影响。只读。</span><span class="sxs-lookup"><span data-stu-id="b5d3c-p102">Represents whether the casing impacted the last sort of the table. Read-only.</span></span>|
|<span data-ttu-id="b5d3c-130">方法</span><span class="sxs-lookup"><span data-stu-id="b5d3c-130">method</span></span>|<span data-ttu-id="b5d3c-131">string</span><span class="sxs-lookup"><span data-stu-id="b5d3c-131">string</span></span>|<span data-ttu-id="b5d3c-p103">表示最后一次对表排序所使用的中文字符排序方法。可能的值是：`PinYin`、`StrokeCount`。只读。</span><span class="sxs-lookup"><span data-stu-id="b5d3c-p103">Represents Chinese character ordering method last used to sort the table. Possible values are: `PinYin`, `StrokeCount`. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5d3c-135">关系</span><span class="sxs-lookup"><span data-stu-id="b5d3c-135">Relationships</span></span>
| <span data-ttu-id="b5d3c-136">关系</span><span class="sxs-lookup"><span data-stu-id="b5d3c-136">Relationship</span></span> | <span data-ttu-id="b5d3c-137">类型</span><span class="sxs-lookup"><span data-stu-id="b5d3c-137">Type</span></span>   |<span data-ttu-id="b5d3c-138">说明</span><span class="sxs-lookup"><span data-stu-id="b5d3c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5d3c-139">域</span><span class="sxs-lookup"><span data-stu-id="b5d3c-139">fields</span></span>|[<span data-ttu-id="b5d3c-140">SortField</span><span class="sxs-lookup"><span data-stu-id="b5d3c-140">SortField</span></span>](sortfield.md)|<span data-ttu-id="b5d3c-p104">表示最后一次对表排序所使用的当前条件。只读。</span><span class="sxs-lookup"><span data-stu-id="b5d3c-p104">Represents the current conditions used to last sort the table. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5d3c-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5d3c-143">JSON representation</span></span>

<span data-ttu-id="b5d3c-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5d3c-144">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tablesort.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
