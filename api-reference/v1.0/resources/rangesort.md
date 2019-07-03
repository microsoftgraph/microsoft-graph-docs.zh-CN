---
title: RangeSort 资源类型
description: 管理对 Range 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fb7f99cc1d7dbdf3ecb81de6bd3e08f87b329642
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35460873"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="94a23-103">RangeSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="94a23-103">RangeSort resource type</span></span>

<span data-ttu-id="94a23-104">管理对 Range 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="94a23-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="94a23-105">方法</span><span class="sxs-lookup"><span data-stu-id="94a23-105">Methods</span></span>

| <span data-ttu-id="94a23-106">方法</span><span class="sxs-lookup"><span data-stu-id="94a23-106">Method</span></span>           | <span data-ttu-id="94a23-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="94a23-107">Return Type</span></span>    |<span data-ttu-id="94a23-108">说明</span><span class="sxs-lookup"><span data-stu-id="94a23-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94a23-109">应用</span><span class="sxs-lookup"><span data-stu-id="94a23-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="94a23-110">无</span><span class="sxs-lookup"><span data-stu-id="94a23-110">None</span></span>|<span data-ttu-id="94a23-111">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="94a23-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="94a23-112">属性</span><span class="sxs-lookup"><span data-stu-id="94a23-112">Properties</span></span>
<span data-ttu-id="94a23-113">无</span><span class="sxs-lookup"><span data-stu-id="94a23-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="94a23-114">关系</span><span class="sxs-lookup"><span data-stu-id="94a23-114">Relationships</span></span>
<span data-ttu-id="94a23-115">无</span><span class="sxs-lookup"><span data-stu-id="94a23-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94a23-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94a23-116">JSON representation</span></span>

<span data-ttu-id="94a23-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94a23-117">Here is a JSON representation of the resource.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="94a23-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="94a23-118">HTTP</span></span>](#tab/http)
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

##### <a name="request"></a><span data-ttu-id="94a23-119">请求</span><span class="sxs-lookup"><span data-stu-id="94a23-119">Request</span></span>
<span data-ttu-id="94a23-120">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="94a23-120">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="94a23-121">C#</span><span class="sxs-lookup"><span data-stu-id="94a23-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-sort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94a23-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="94a23-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-sort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94a23-123">目标-C</span><span class="sxs-lookup"><span data-stu-id="94a23-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-sort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="94a23-124">响应</span><span class="sxs-lookup"><span data-stu-id="94a23-124">Response</span></span>
<span data-ttu-id="94a23-125">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="94a23-125">Here is an example of the response.</span></span> 
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


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
