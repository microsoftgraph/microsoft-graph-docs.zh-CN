---
title: RangeSort 资源类型
description: 管理对 Range 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: f4b5ffac155542615d17db0f6e511cf77c72cc82
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36730307"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="fbe37-103">RangeSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="fbe37-103">RangeSort resource type</span></span>

<span data-ttu-id="fbe37-104">管理对 Range 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="fbe37-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="fbe37-105">方法</span><span class="sxs-lookup"><span data-stu-id="fbe37-105">Methods</span></span>

| <span data-ttu-id="fbe37-106">方法</span><span class="sxs-lookup"><span data-stu-id="fbe37-106">Method</span></span>           | <span data-ttu-id="fbe37-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="fbe37-107">Return Type</span></span>    |<span data-ttu-id="fbe37-108">说明</span><span class="sxs-lookup"><span data-stu-id="fbe37-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fbe37-109">应用</span><span class="sxs-lookup"><span data-stu-id="fbe37-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="fbe37-110">无</span><span class="sxs-lookup"><span data-stu-id="fbe37-110">None</span></span>|<span data-ttu-id="fbe37-111">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="fbe37-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="fbe37-112">属性</span><span class="sxs-lookup"><span data-stu-id="fbe37-112">Properties</span></span>
<span data-ttu-id="fbe37-113">无</span><span class="sxs-lookup"><span data-stu-id="fbe37-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="fbe37-114">关系</span><span class="sxs-lookup"><span data-stu-id="fbe37-114">Relationships</span></span>
<span data-ttu-id="fbe37-115">无</span><span class="sxs-lookup"><span data-stu-id="fbe37-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fbe37-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fbe37-116">JSON representation</span></span>

<span data-ttu-id="fbe37-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbe37-117">Here is a JSON representation of the resource.</span></span>


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

##### <a name="request"></a><span data-ttu-id="fbe37-118">请求</span><span class="sxs-lookup"><span data-stu-id="fbe37-118">Request</span></span>
<span data-ttu-id="fbe37-119">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fbe37-119">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fbe37-120">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fbe37-120">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fbe37-121">C#</span><span class="sxs-lookup"><span data-stu-id="fbe37-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-sort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fbe37-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fbe37-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-sort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fbe37-123">目标-C</span><span class="sxs-lookup"><span data-stu-id="fbe37-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-sort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fbe37-124">Java</span><span class="sxs-lookup"><span data-stu-id="fbe37-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-sort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="fbe37-125">响应</span><span class="sxs-lookup"><span data-stu-id="fbe37-125">Response</span></span>
<span data-ttu-id="fbe37-126">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fbe37-126">Here is an example of the response.</span></span> 
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
