---
title: RangeSort 资源类型
description: 管理对 Range 对象的排序操作。
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: c52b4c6cc50bce7d518d26798db9f3d3da49cd1c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816426"
---
# <a name="rangesort-resource-type"></a><span data-ttu-id="cc33c-103">RangeSort 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc33c-103">RangeSort resource type</span></span>

<span data-ttu-id="cc33c-104">管理对 Range 对象的排序操作。</span><span class="sxs-lookup"><span data-stu-id="cc33c-104">Manages sorting operations on Range objects.</span></span>


## <a name="methods"></a><span data-ttu-id="cc33c-105">方法</span><span class="sxs-lookup"><span data-stu-id="cc33c-105">Methods</span></span>

| <span data-ttu-id="cc33c-106">方法</span><span class="sxs-lookup"><span data-stu-id="cc33c-106">Method</span></span>           | <span data-ttu-id="cc33c-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="cc33c-107">Return Type</span></span>    |<span data-ttu-id="cc33c-108">说明</span><span class="sxs-lookup"><span data-stu-id="cc33c-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc33c-109">应用</span><span class="sxs-lookup"><span data-stu-id="cc33c-109">Apply</span></span>](../api/rangesort-apply.md)|<span data-ttu-id="cc33c-110">无</span><span class="sxs-lookup"><span data-stu-id="cc33c-110">None</span></span>|<span data-ttu-id="cc33c-111">执行排序操作。</span><span class="sxs-lookup"><span data-stu-id="cc33c-111">Perform a sort operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc33c-112">属性</span><span class="sxs-lookup"><span data-stu-id="cc33c-112">Properties</span></span>
<span data-ttu-id="cc33c-113">无</span><span class="sxs-lookup"><span data-stu-id="cc33c-113">None</span></span>

## <a name="relationships"></a><span data-ttu-id="cc33c-114">Relationships</span><span class="sxs-lookup"><span data-stu-id="cc33c-114">Relationships</span></span>
<span data-ttu-id="cc33c-115">无</span><span class="sxs-lookup"><span data-stu-id="cc33c-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc33c-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc33c-116">JSON representation</span></span>

<span data-ttu-id="cc33c-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc33c-117">Here is a JSON representation of the resource.</span></span>

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

##### <a name="request"></a><span data-ttu-id="cc33c-118">请求</span><span class="sxs-lookup"><span data-stu-id="cc33c-118">Request</span></span>
<span data-ttu-id="cc33c-119">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cc33c-119">Here is an example of the request.</span></span>

<!--{
  "blockType": "request",
  "name": "range_sort"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/sort
```

##### <a name="response"></a><span data-ttu-id="cc33c-120">响应</span><span class="sxs-lookup"><span data-stu-id="cc33c-120">Response</span></span>
<span data-ttu-id="cc33c-121">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cc33c-121">Here is an example of the response.</span></span> 
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
