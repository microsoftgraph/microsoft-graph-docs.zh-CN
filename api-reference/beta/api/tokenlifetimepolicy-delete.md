---
title: 删除 tokenLifetimePolicy
description: 删除 tokenLifetimePolicy。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: d73fd917d7fa503857cf7592c2c95925166b133b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443374"
---
# <a name="delete-tokenlifetimepolicy"></a><span data-ttu-id="481c5-103">删除 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="481c5-103">Delete tokenLifetimePolicy</span></span>

<span data-ttu-id="481c5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="481c5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="481c5-105">删除 [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="481c5-105">Delete a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="481c5-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="481c5-106">Permissions</span></span>

<span data-ttu-id="481c5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="481c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="481c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="481c5-109">Permission type</span></span>                        | <span data-ttu-id="481c5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="481c5-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="481c5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="481c5-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="481c5-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="481c5-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="481c5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="481c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="481c5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="481c5-114">Not supported.</span></span> |
| <span data-ttu-id="481c5-115">Application</span><span class="sxs-lookup"><span data-stu-id="481c5-115">Application</span></span>                            | <span data-ttu-id="481c5-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="481c5-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="481c5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="481c5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/tokenLifetimePolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="481c5-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="481c5-118">Request headers</span></span>

| <span data-ttu-id="481c5-119">名称</span><span class="sxs-lookup"><span data-stu-id="481c5-119">Name</span></span>          | <span data-ttu-id="481c5-120">说明</span><span class="sxs-lookup"><span data-stu-id="481c5-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="481c5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="481c5-121">Authorization</span></span> | <span data-ttu-id="481c5-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="481c5-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="481c5-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="481c5-123">Request body</span></span>

<span data-ttu-id="481c5-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="481c5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="481c5-125">响应</span><span class="sxs-lookup"><span data-stu-id="481c5-125">Response</span></span>

<span data-ttu-id="481c5-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="481c5-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="481c5-127">示例</span><span class="sxs-lookup"><span data-stu-id="481c5-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="481c5-128">请求</span><span class="sxs-lookup"><span data-stu-id="481c5-128">Request</span></span>

<span data-ttu-id="481c5-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="481c5-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="481c5-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="481c5-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="481c5-131">C#</span><span class="sxs-lookup"><span data-stu-id="481c5-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenlifetimepolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="481c5-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="481c5-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenlifetimepolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="481c5-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="481c5-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenlifetimepolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="481c5-134">Java</span><span class="sxs-lookup"><span data-stu-id="481c5-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenlifetimepolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="481c5-135">响应</span><span class="sxs-lookup"><span data-stu-id="481c5-135">Response</span></span>

<span data-ttu-id="481c5-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="481c5-136">The following is an example of the response.</span></span>

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
  "description": "Delete tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


