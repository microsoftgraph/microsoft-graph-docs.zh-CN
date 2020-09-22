---
title: RangeSort 资源类型
description: 管理对 Range 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 4964162d6c3380f3dcbe12ef0ed6ce0009149bb3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028250"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="1410f-103">RangeSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="1410f-103">RangeSort resource type</span></span>

<span data-ttu-id="1410f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1410f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1410f-105">管理对 Range 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="1410f-105">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="1410f-106">方法</span><span class="sxs-lookup"><span data-stu-id="1410f-106">Methods</span></span>

| <span data-ttu-id="1410f-107">方法</span><span class="sxs-lookup"><span data-stu-id="1410f-107">Method</span></span>           | <span data-ttu-id="1410f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1410f-108">Return Type</span></span>    |<span data-ttu-id="1410f-109">说明</span><span class="sxs-lookup"><span data-stu-id="1410f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1410f-110">应用</span><span class="sxs-lookup"><span data-stu-id="1410f-110">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="1410f-111">无</span><span class="sxs-lookup"><span data-stu-id="1410f-111">None</span></span>|<span data-ttu-id="1410f-112">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="1410f-112">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="1410f-113">属性</span><span class="sxs-lookup"><span data-stu-id="1410f-113">Properties</span></span>
<span data-ttu-id="1410f-114">无</span><span class="sxs-lookup"><span data-stu-id="1410f-114">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1410f-115">关系</span><span class="sxs-lookup"><span data-stu-id="1410f-115">Relationships</span></span>
<span data-ttu-id="1410f-116">无</span><span class="sxs-lookup"><span data-stu-id="1410f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1410f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1410f-117">JSON representation</span></span>

<span data-ttu-id="1410f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1410f-118">Here is a JSON representation of the resource.</span></span>


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

##### <a name="request"></a><span data-ttu-id="1410f-119">请求</span><span class="sxs-lookup"><span data-stu-id="1410f-119">Request</span></span>
<span data-ttu-id="1410f-120">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1410f-120">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1410f-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="1410f-121">HTTP</span></span>](#tab/http)
<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```
# <a name="c"></a>[<span data-ttu-id="1410f-122">C#</span><span class="sxs-lookup"><span data-stu-id="1410f-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/range-sort-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1410f-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1410f-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/range-sort-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1410f-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1410f-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/range-sort-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1410f-125">Java</span><span class="sxs-lookup"><span data-stu-id="1410f-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/range-sort-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1410f-126">响应</span><span class="sxs-lookup"><span data-stu-id="1410f-126">Response</span></span>
<span data-ttu-id="1410f-127">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1410f-127">Here is an example of the response.</span></span> 
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

