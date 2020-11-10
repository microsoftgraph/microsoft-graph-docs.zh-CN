---
title: 获取 trustFrameworkKeySet
description: 检索 trustframeworkkeyset 对象的属性和关系。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 35fc4afe312c5a09e97d4c0fef2bf476f7450d32
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980949"
---
# <a name="get-trustframeworkkeyset"></a><span data-ttu-id="fb935-103">获取 trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="fb935-103">Get trustFrameworkKeySet</span></span>

<span data-ttu-id="fb935-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb935-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb935-105">检索 [Trustframeworkkeyset](../resources/trustframeworkkeyset.md)的属性和关联。</span><span class="sxs-lookup"><span data-stu-id="fb935-105">Retrieve the properties and associations for a [Trustframeworkkeyset](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fb935-106">权限</span><span class="sxs-lookup"><span data-stu-id="fb935-106">Permissions</span></span>

<span data-ttu-id="fb935-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb935-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb935-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb935-109">Permission type</span></span>                        | <span data-ttu-id="fb935-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb935-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fb935-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb935-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb935-112">TrustFrameworkKeySet、TrustFrameworkKeySet 和所有</span><span class="sxs-lookup"><span data-stu-id="fb935-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="fb935-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb935-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb935-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb935-114">Not supported.</span></span> |
| <span data-ttu-id="fb935-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb935-115">Application</span></span>                            | <span data-ttu-id="fb935-116">TrustFrameworkKeySet、TrustFrameworkKeySet 和所有</span><span class="sxs-lookup"><span data-stu-id="fb935-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb935-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb935-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fb935-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb935-118">Request headers</span></span>

| <span data-ttu-id="fb935-119">名称</span><span class="sxs-lookup"><span data-stu-id="fb935-119">Name</span></span>      |<span data-ttu-id="fb935-120">说明</span><span class="sxs-lookup"><span data-stu-id="fb935-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fb935-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb935-121">Authorization</span></span> | <span data-ttu-id="fb935-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb935-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb935-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb935-124">Request body</span></span>

<span data-ttu-id="fb935-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb935-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb935-126">响应</span><span class="sxs-lookup"><span data-stu-id="fb935-126">Response</span></span>

<span data-ttu-id="fb935-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb935-127">If successful, this method returns a `200 OK` response code and the requested [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb935-128">示例</span><span class="sxs-lookup"><span data-stu-id="fb935-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb935-129">请求</span><span class="sxs-lookup"><span data-stu-id="fb935-129">Request</span></span>

<span data-ttu-id="fb935-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fb935-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fb935-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb935-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustframeworkkeyset"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```
# <a name="c"></a>[<span data-ttu-id="fb935-132">C#</span><span class="sxs-lookup"><span data-stu-id="fb935-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb935-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb935-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb935-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb935-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb935-135">Java</span><span class="sxs-lookup"><span data-stu-id="fb935-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-trustframeworkkeyset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fb935-136">响应</span><span class="sxs-lookup"><span data-stu-id="fb935-136">Response</span></span>

<span data-ttu-id="fb935-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fb935-137">The following is an example of the response.</span></span>

> <span data-ttu-id="fb935-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fb935-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


