---
title: RangeSort 资源类型
description: 管理对 Range 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: bf1006197a82d5b1d5d30124e47d7125424f0eee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034879"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="f12a2-103">RangeSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="f12a2-103">RangeSort resource type</span></span>

<span data-ttu-id="f12a2-104">管理对 Range 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="f12a2-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="f12a2-105">方法</span><span class="sxs-lookup"><span data-stu-id="f12a2-105">Methods</span></span>

| <span data-ttu-id="f12a2-106">方法</span><span class="sxs-lookup"><span data-stu-id="f12a2-106">Method</span></span>           | <span data-ttu-id="f12a2-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="f12a2-107">Return Type</span></span>    |<span data-ttu-id="f12a2-108">说明</span><span class="sxs-lookup"><span data-stu-id="f12a2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f12a2-109">应用</span><span class="sxs-lookup"><span data-stu-id="f12a2-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="f12a2-110">无</span><span class="sxs-lookup"><span data-stu-id="f12a2-110">None</span></span>|<span data-ttu-id="f12a2-111">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="f12a2-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="f12a2-112">属性</span><span class="sxs-lookup"><span data-stu-id="f12a2-112">Properties</span></span>
<span data-ttu-id="f12a2-113">无</span><span class="sxs-lookup"><span data-stu-id="f12a2-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="f12a2-114">关系</span><span class="sxs-lookup"><span data-stu-id="f12a2-114">Relationships</span></span>
<span data-ttu-id="f12a2-115">无</span><span class="sxs-lookup"><span data-stu-id="f12a2-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f12a2-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f12a2-116">JSON representation</span></span>

<span data-ttu-id="f12a2-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f12a2-117">Here is a JSON representation of the resource.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f12a2-118">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="f12a2-118">HTTP</span></span>](#tab/http)
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

##### <a name="request"></a><span data-ttu-id="f12a2-119">请求</span><span class="sxs-lookup"><span data-stu-id="f12a2-119">Request</span></span>
<span data-ttu-id="f12a2-120">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f12a2-120">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f12a2-121">C#</span><span class="sxs-lookup"><span data-stu-id="f12a2-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-sort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f12a2-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="f12a2-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-sort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f12a2-123">目标-C</span><span class="sxs-lookup"><span data-stu-id="f12a2-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-sort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f12a2-124">Java</span><span class="sxs-lookup"><span data-stu-id="f12a2-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-sort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f12a2-125">响应</span><span class="sxs-lookup"><span data-stu-id="f12a2-125">Response</span></span>
<span data-ttu-id="f12a2-126">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f12a2-126">Here is an example of the response.</span></span> 
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
