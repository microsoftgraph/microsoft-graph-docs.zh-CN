---
title: 获取 trustFrameworkKeySet
description: 检索 trustframeworkkeyset 对象的属性和关系。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 31272fc287ceba29dd39286a0e103ebcf6829e1d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433654"
---
# <a name="get-trustframeworkkeyset"></a><span data-ttu-id="f7784-103">获取 trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="f7784-103">Get trustFrameworkKeySet</span></span>

<span data-ttu-id="f7784-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7784-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7784-105">检索 [Trustframeworkkeyset 的属性和关联](../resources/trustframeworkkeyset.md)。</span><span class="sxs-lookup"><span data-stu-id="f7784-105">Retrieve the properties and associations for a [Trustframeworkkeyset](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f7784-106">权限</span><span class="sxs-lookup"><span data-stu-id="f7784-106">Permissions</span></span>

<span data-ttu-id="f7784-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7784-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7784-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7784-109">Permission type</span></span>                        | <span data-ttu-id="f7784-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7784-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f7784-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7784-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7784-112">TrustFrameworkKeySet.Read.All、TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7784-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="f7784-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7784-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7784-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7784-114">Not supported.</span></span> |
| <span data-ttu-id="f7784-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7784-115">Application</span></span>                            | <span data-ttu-id="f7784-116">TrustFrameworkKeySet.Read.All、TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7784-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7784-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7784-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f7784-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7784-118">Request headers</span></span>

| <span data-ttu-id="f7784-119">名称</span><span class="sxs-lookup"><span data-stu-id="f7784-119">Name</span></span>      |<span data-ttu-id="f7784-120">说明</span><span class="sxs-lookup"><span data-stu-id="f7784-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7784-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7784-121">Authorization</span></span> | <span data-ttu-id="f7784-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7784-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7784-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7784-124">Request body</span></span>

<span data-ttu-id="f7784-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7784-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7784-126">响应</span><span class="sxs-lookup"><span data-stu-id="f7784-126">Response</span></span>

<span data-ttu-id="f7784-127">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和请求 [的 trustFrameworkKeySet](../resources/trustframeworkkeyset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7784-127">If successful, this method returns a `200 OK` response code and the requested [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7784-128">示例</span><span class="sxs-lookup"><span data-stu-id="f7784-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f7784-129">请求</span><span class="sxs-lookup"><span data-stu-id="f7784-129">Request</span></span>

<span data-ttu-id="f7784-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f7784-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7784-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7784-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustframeworkkeyset"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```
# <a name="c"></a>[<span data-ttu-id="f7784-132">C#</span><span class="sxs-lookup"><span data-stu-id="f7784-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7784-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7784-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7784-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7784-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7784-135">Java</span><span class="sxs-lookup"><span data-stu-id="f7784-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-trustframeworkkeyset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f7784-136">响应</span><span class="sxs-lookup"><span data-stu-id="f7784-136">Response</span></span>

<span data-ttu-id="f7784-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f7784-137">The following is an example of the response.</span></span>

> <span data-ttu-id="f7784-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f7784-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value",
  "keys": [
    {
      "k": "k-value",
      "x5c": [
        "x5c-value"
      ],
      "x5t": "x5t-value",
      "kty": "kty-value",
      "use": "use-value",
      "exp": 99,
      "nbf": 99,
      "kid": "kid-value",
      "e": "e-value",
      "n": "n-value",
      "d": "d-value",
      "p": "p-value",
      "q": "q-value",
      "dp": "dp-value",
      "dq": "dq-value",
      "qi": "qi-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


