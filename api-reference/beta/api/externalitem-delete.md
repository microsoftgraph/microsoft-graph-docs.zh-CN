---
title: 删除 externalItem
description: 删除 externalItem。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: apiPageType
ms.openlocfilehash: 143b2d266eeea7a7b776f3f75e8005740b4c498e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954585"
---
# <a name="delete-externalitem"></a><span data-ttu-id="428f8-103">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="428f8-103">Delete externalItem</span></span>

<span data-ttu-id="428f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="428f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="428f8-105">删除 [externalitem](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="428f8-105">Delete an [externalitem](../resources/externalitem.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="permissions"></a><span data-ttu-id="428f8-106">权限</span><span class="sxs-lookup"><span data-stu-id="428f8-106">Permissions</span></span>

<span data-ttu-id="428f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="428f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="428f8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="428f8-109">Permission type</span></span>                        | <span data-ttu-id="428f8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="428f8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="428f8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="428f8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="428f8-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="428f8-112">Not supported.</span></span> |
| <span data-ttu-id="428f8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="428f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="428f8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="428f8-114">Not supported.</span></span> |
| <span data-ttu-id="428f8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="428f8-115">Application</span></span>                            | <span data-ttu-id="428f8-116">ExternalItem.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="428f8-116">ExternalItem.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="428f8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="428f8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /external/connections/{connection-id}/items/{item-id}
```

## <a name="path-parameters"></a><span data-ttu-id="428f8-118">路径参数</span><span class="sxs-lookup"><span data-stu-id="428f8-118">Path parameters</span></span>

| <span data-ttu-id="428f8-119">参数</span><span class="sxs-lookup"><span data-stu-id="428f8-119">Parameter</span></span>     | <span data-ttu-id="428f8-120">类型</span><span class="sxs-lookup"><span data-stu-id="428f8-120">Type</span></span>   | <span data-ttu-id="428f8-121">说明</span><span class="sxs-lookup"><span data-stu-id="428f8-121">Description</span></span>                                         |
|:--------------|:-------|:----------------------------------------------------|
| <span data-ttu-id="428f8-122">connection-id</span><span class="sxs-lookup"><span data-stu-id="428f8-122">connection-id</span></span> | <span data-ttu-id="428f8-123">string</span><span class="sxs-lookup"><span data-stu-id="428f8-123">string</span></span> | <span data-ttu-id="428f8-124">`id`包含[externalConnection](../resources/externalconnection.md)的属性</span><span class="sxs-lookup"><span data-stu-id="428f8-124">The `id` property of the containing [externalConnection](../resources/externalconnection.md)</span></span> |
| <span data-ttu-id="428f8-125">item-id</span><span class="sxs-lookup"><span data-stu-id="428f8-125">item-id</span></span>       | <span data-ttu-id="428f8-126">string</span><span class="sxs-lookup"><span data-stu-id="428f8-126">string</span></span> | <span data-ttu-id="428f8-127">ExternalItem 的开发人员提供的 `id` 属性[externalItem](../resources/externalitem.md)。</span><span class="sxs-lookup"><span data-stu-id="428f8-127">The developer-provided `id` property of the [externalItem](../resources/externalitem.md).</span></span> |

## <a name="request-headers"></a><span data-ttu-id="428f8-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="428f8-128">Request headers</span></span>

| <span data-ttu-id="428f8-129">名称</span><span class="sxs-lookup"><span data-stu-id="428f8-129">Name</span></span>          | <span data-ttu-id="428f8-130">说明</span><span class="sxs-lookup"><span data-stu-id="428f8-130">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="428f8-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="428f8-131">Authorization</span></span> | <span data-ttu-id="428f8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="428f8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="428f8-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="428f8-134">Request body</span></span>

<span data-ttu-id="428f8-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="428f8-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="428f8-136">响应</span><span class="sxs-lookup"><span data-stu-id="428f8-136">Response</span></span>

<span data-ttu-id="428f8-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="428f8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="428f8-139">示例</span><span class="sxs-lookup"><span data-stu-id="428f8-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="428f8-140">请求</span><span class="sxs-lookup"><span data-stu-id="428f8-140">Request</span></span>

<span data-ttu-id="428f8-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="428f8-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="428f8-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="428f8-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_externalitem"
}-->

```http
DELETE https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938
```
# <a name="objective-c"></a>[<span data-ttu-id="428f8-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="428f8-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-externalitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="428f8-144">C#</span><span class="sxs-lookup"><span data-stu-id="428f8-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-externalitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="428f8-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="428f8-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-externalitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="428f8-146">Java</span><span class="sxs-lookup"><span data-stu-id="428f8-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-externalitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="428f8-147">响应</span><span class="sxs-lookup"><span data-stu-id="428f8-147">Response</span></span>
<!-- markdownlint-enable MD024 -->

<span data-ttu-id="428f8-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="428f8-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete externalItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


