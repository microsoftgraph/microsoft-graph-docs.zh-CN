---
title: RangeSort 资源类型
description: 管理对 Range 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 6d1fb0be3feae69ff2cae34f360a0f78d46a6172
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947573"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="83d4f-103">RangeSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="83d4f-103">RangeSort resource type</span></span>

<span data-ttu-id="83d4f-104">管理对 Range 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="83d4f-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="83d4f-105">方法</span><span class="sxs-lookup"><span data-stu-id="83d4f-105">Methods</span></span>

| <span data-ttu-id="83d4f-106">方法</span><span class="sxs-lookup"><span data-stu-id="83d4f-106">Method</span></span>           | <span data-ttu-id="83d4f-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="83d4f-107">Return Type</span></span>    |<span data-ttu-id="83d4f-108">说明</span><span class="sxs-lookup"><span data-stu-id="83d4f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="83d4f-109">应用</span><span class="sxs-lookup"><span data-stu-id="83d4f-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="83d4f-110">无</span><span class="sxs-lookup"><span data-stu-id="83d4f-110">None</span></span>|<span data-ttu-id="83d4f-111">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="83d4f-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="83d4f-112">属性</span><span class="sxs-lookup"><span data-stu-id="83d4f-112">Properties</span></span>
<span data-ttu-id="83d4f-113">无</span><span class="sxs-lookup"><span data-stu-id="83d4f-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="83d4f-114">Relationships</span><span class="sxs-lookup"><span data-stu-id="83d4f-114">Relationships</span></span>
<span data-ttu-id="83d4f-115">无</span><span class="sxs-lookup"><span data-stu-id="83d4f-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83d4f-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83d4f-116">JSON representation</span></span>

<span data-ttu-id="83d4f-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83d4f-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="83d4f-118">请求</span><span class="sxs-lookup"><span data-stu-id="83d4f-118">Request</span></span>
<span data-ttu-id="83d4f-119">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83d4f-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="83d4f-120">响应</span><span class="sxs-lookup"><span data-stu-id="83d4f-120">Response</span></span>
<span data-ttu-id="83d4f-121">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="83d4f-121">Here is an example of the response.</span></span> 
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
  "tocPath": ""
}-->
