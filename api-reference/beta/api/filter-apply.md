---
title: 'Filter: apply'
description: 在给定列中应用给定的筛选条件。
localization_priority: Normal
doc_type: apiPageType
author: ruoyingl
ms.prod: ''
ms.openlocfilehash: 4484f678c85b85fed0b659bfc45a7afaf869c840
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787262"
---
# <a name="filter-apply"></a><span data-ttu-id="7e88c-103">Filter: apply</span><span class="sxs-lookup"><span data-stu-id="7e88c-103">Filter: apply</span></span>

<span data-ttu-id="7e88c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e88c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e88c-105">在给定列中应用给定的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="7e88c-105">Apply the given filter criteria on the given column.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e88c-106">权限</span><span class="sxs-lookup"><span data-stu-id="7e88c-106">Permissions</span></span>
<span data-ttu-id="7e88c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e88c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e88c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e88c-109">Permission type</span></span>      | <span data-ttu-id="7e88c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e88c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e88c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e88c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e88c-112">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e88c-112">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7e88c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e88c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e88c-114">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7e88c-114">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7e88c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e88c-115">Application</span></span> | <span data-ttu-id="7e88c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e88c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e88c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e88c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /me/drive/root:/{item-path}:/workbook/tables/{id|name}/columns/{id|name}/filter/apply
POST /me/drive/items/{id}/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply
POST /me/drive/root:/{item-path}:/workbook/worksheets/{id|name}/tables/{id|name}/columns/{id|name}/filter/apply

```
## <a name="request-headers"></a><span data-ttu-id="7e88c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e88c-118">Request headers</span></span>
| <span data-ttu-id="7e88c-119">名称</span><span class="sxs-lookup"><span data-stu-id="7e88c-119">Name</span></span>       | <span data-ttu-id="7e88c-120">说明</span><span class="sxs-lookup"><span data-stu-id="7e88c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7e88c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e88c-121">Authorization</span></span>  | <span data-ttu-id="7e88c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7e88c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e88c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e88c-124">Request body</span></span>
<span data-ttu-id="7e88c-125">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7e88c-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7e88c-126">参数</span><span class="sxs-lookup"><span data-stu-id="7e88c-126">Parameter</span></span>    | <span data-ttu-id="7e88c-127">类型</span><span class="sxs-lookup"><span data-stu-id="7e88c-127">Type</span></span>   |<span data-ttu-id="7e88c-128">说明</span><span class="sxs-lookup"><span data-stu-id="7e88c-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e88c-129">条件</span><span class="sxs-lookup"><span data-stu-id="7e88c-129">criteria</span></span>|<span data-ttu-id="7e88c-130">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="7e88c-130">workbookFilterCriteria</span></span>|<span data-ttu-id="7e88c-131">要应用的条件。</span><span class="sxs-lookup"><span data-stu-id="7e88c-131">The criteria to apply.</span></span>|

## <a name="response"></a><span data-ttu-id="7e88c-132">响应</span><span class="sxs-lookup"><span data-stu-id="7e88c-132">Response</span></span>

<span data-ttu-id="7e88c-p103">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7e88c-p103">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e88c-135">示例</span><span class="sxs-lookup"><span data-stu-id="7e88c-135">Example</span></span>
<span data-ttu-id="7e88c-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7e88c-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7e88c-137">请求</span><span class="sxs-lookup"><span data-stu-id="7e88c-137">Request</span></span>
<span data-ttu-id="7e88c-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7e88c-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e88c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e88c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "filter_apply"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply
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
# <a name="c"></a>[<span data-ttu-id="7e88c-140">C#</span><span class="sxs-lookup"><span data-stu-id="7e88c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/filter-apply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e88c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e88c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/filter-apply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e88c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e88c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/filter-apply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e88c-143">Java</span><span class="sxs-lookup"><span data-stu-id="7e88c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/filter-apply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7e88c-144">响应</span><span class="sxs-lookup"><span data-stu-id="7e88c-144">Response</span></span>
<span data-ttu-id="7e88c-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7e88c-145">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter: apply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


