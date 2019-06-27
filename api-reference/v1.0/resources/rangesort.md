---
title: RangeSort 资源类型
description: 管理对 Range 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 8f917cb2fa7c8ade81fef2d713e368cc43ab40b3
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275143"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="94c0b-103">RangeSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="94c0b-103">RangeSort resource type</span></span>

<span data-ttu-id="94c0b-104">管理对 Range 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="94c0b-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="94c0b-105">方法</span><span class="sxs-lookup"><span data-stu-id="94c0b-105">Methods</span></span>

| <span data-ttu-id="94c0b-106">方法</span><span class="sxs-lookup"><span data-stu-id="94c0b-106">Method</span></span>           | <span data-ttu-id="94c0b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="94c0b-107">Return Type</span></span>    |<span data-ttu-id="94c0b-108">说明</span><span class="sxs-lookup"><span data-stu-id="94c0b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94c0b-109">应用</span><span class="sxs-lookup"><span data-stu-id="94c0b-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="94c0b-110">无</span><span class="sxs-lookup"><span data-stu-id="94c0b-110">None</span></span>|<span data-ttu-id="94c0b-111">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="94c0b-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="94c0b-112">属性</span><span class="sxs-lookup"><span data-stu-id="94c0b-112">Properties</span></span>
<span data-ttu-id="94c0b-113">无</span><span class="sxs-lookup"><span data-stu-id="94c0b-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="94c0b-114">关系</span><span class="sxs-lookup"><span data-stu-id="94c0b-114">Relationships</span></span>
<span data-ttu-id="94c0b-115">无</span><span class="sxs-lookup"><span data-stu-id="94c0b-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94c0b-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94c0b-116">JSON representation</span></span>

<span data-ttu-id="94c0b-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94c0b-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookRangeSort"
}-->

```json
{
}
```

##### <a name="request"></a><span data-ttu-id="94c0b-118">请求</span><span class="sxs-lookup"><span data-stu-id="94c0b-118">Request</span></span>
<span data-ttu-id="94c0b-119">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94c0b-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="94c0b-120">响应</span><span class="sxs-lookup"><span data-stu-id="94c0b-120">Response</span></span>
<span data-ttu-id="94c0b-121">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="94c0b-121">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeSort"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="94c0b-122">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="94c0b-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="94c0b-123">C#</span><span class="sxs-lookup"><span data-stu-id="94c0b-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_sort-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94c0b-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="94c0b-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_sort-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="94c0b-125">目标-C</span><span class="sxs-lookup"><span data-stu-id="94c0b-125">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/range_sort-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
