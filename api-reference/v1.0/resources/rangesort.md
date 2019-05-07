---
title: RangeSort 资源类型
description: 管理对 Range 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 3204a72fe51d3afd3771c0e6775138277ef450e2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601144"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="e299d-103">RangeSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="e299d-103">RangeSort resource type</span></span>

<span data-ttu-id="e299d-104">管理对 Range 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="e299d-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="e299d-105">方法</span><span class="sxs-lookup"><span data-stu-id="e299d-105">Methods</span></span>

| <span data-ttu-id="e299d-106">方法</span><span class="sxs-lookup"><span data-stu-id="e299d-106">Method</span></span>           | <span data-ttu-id="e299d-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="e299d-107">Return Type</span></span>    |<span data-ttu-id="e299d-108">说明</span><span class="sxs-lookup"><span data-stu-id="e299d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e299d-109">应用</span><span class="sxs-lookup"><span data-stu-id="e299d-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="e299d-110">无</span><span class="sxs-lookup"><span data-stu-id="e299d-110">None</span></span>|<span data-ttu-id="e299d-111">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="e299d-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="e299d-112">属性</span><span class="sxs-lookup"><span data-stu-id="e299d-112">Properties</span></span>
<span data-ttu-id="e299d-113">无</span><span class="sxs-lookup"><span data-stu-id="e299d-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="e299d-114">关系</span><span class="sxs-lookup"><span data-stu-id="e299d-114">Relationships</span></span>
<span data-ttu-id="e299d-115">无</span><span class="sxs-lookup"><span data-stu-id="e299d-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e299d-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e299d-116">JSON representation</span></span>

<span data-ttu-id="e299d-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e299d-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="e299d-118">请求</span><span class="sxs-lookup"><span data-stu-id="e299d-118">Request</span></span>
<span data-ttu-id="e299d-119">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e299d-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="e299d-120">响应</span><span class="sxs-lookup"><span data-stu-id="e299d-120">Response</span></span>
<span data-ttu-id="e299d-121">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e299d-121">Here is an example of the response.</span></span> 
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e299d-122">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e299d-122">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e299d-123">语言</span><span class="sxs-lookup"><span data-stu-id="e299d-123">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/range_sort-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e299d-124">Javascript</span><span class="sxs-lookup"><span data-stu-id="e299d-124">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/range_sort-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/rangesort.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
