---
title: 'Filter: apply'
description: 在给定列中应用给定的筛选条件。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 51d78cf2d839968a9683c7ecab910ce0aeccb611
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038646"
---
# <a name="filter-apply"></a><span data-ttu-id="2d87a-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="2d87a-103">Filter: apply</span></span>

<span data-ttu-id="2d87a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d87a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2d87a-105">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="2d87a-105">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d87a-106">权限</span><span class="sxs-lookup"><span data-stu-id="2d87a-106">Permissions</span></span>
<span data-ttu-id="2d87a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d87a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d87a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d87a-109">Permission type</span></span>      | <span data-ttu-id="2d87a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2d87a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d87a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d87a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2d87a-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d87a-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2d87a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d87a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d87a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d87a-114">Not supported.</span></span>    |
|<span data-ttu-id="2d87a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d87a-115">Application</span></span> | <span data-ttu-id="2d87a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d87a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d87a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d87a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="2d87a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d87a-118">Request headers</span></span>
| <span data-ttu-id="2d87a-119">名称</span><span class="sxs-lookup"><span data-stu-id="2d87a-119">Name</span></span>       | <span data-ttu-id="2d87a-120">说明</span><span class="sxs-lookup"><span data-stu-id="2d87a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2d87a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d87a-121">Authorization</span></span>  | <span data-ttu-id="2d87a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2d87a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d87a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d87a-124">Request body</span></span>
<span data-ttu-id="2d87a-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2d87a-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2d87a-126">参数</span><span class="sxs-lookup"><span data-stu-id="2d87a-126">Parameter</span></span>    | <span data-ttu-id="2d87a-127">类型</span><span class="sxs-lookup"><span data-stu-id="2d87a-127">Type</span></span>   |<span data-ttu-id="2d87a-128">说明</span><span class="sxs-lookup"><span data-stu-id="2d87a-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d87a-129">条件</span><span class="sxs-lookup"><span data-stu-id="2d87a-129">criteria</span></span>|<span data-ttu-id="2d87a-130">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="2d87a-130">WorkbookFilterCriteria</span></span>|<span data-ttu-id="2d87a-131">要应用的条件。</span><span class="sxs-lookup"><span data-stu-id="2d87a-131">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="2d87a-132">响应</span><span class="sxs-lookup"><span data-stu-id="2d87a-132">Response</span></span>

<span data-ttu-id="2d87a-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2d87a-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d87a-135">示例</span><span class="sxs-lookup"><span data-stu-id="2d87a-135">Example</span></span>
<span data-ttu-id="2d87a-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="2d87a-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2d87a-137">请求</span><span class="sxs-lookup"><span data-stu-id="2d87a-137">Request</span></span>
<span data-ttu-id="2d87a-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d87a-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2d87a-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="2d87a-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
Content-type: application/json
Content-length: 321

{
  "criteria": {
    "criterion1": "criterion1-value",
    "criterion2": "criterion2-value",
    "color": "color-value",
    "operator": {
    },
    "icon": {
      "set": "set-value",
      "index": 99
    },
    "dynamicCriteria": "dynamicCriteria-value",
    "values": {
    },
    "filterOn": "filterOn-value"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="2d87a-140">C#</span><span class="sxs-lookup"><span data-stu-id="2d87a-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2d87a-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2d87a-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2d87a-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2d87a-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2d87a-143">Java</span><span class="sxs-lookup"><span data-stu-id="2d87a-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="2d87a-144">响应</span><span class="sxs-lookup"><span data-stu-id="2d87a-144">Response</span></span>
<span data-ttu-id="2d87a-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2d87a-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

