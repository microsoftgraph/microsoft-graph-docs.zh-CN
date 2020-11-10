---
title: 列出 keySets
description: 检索 trustframeworkkeyset 对象的列表。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e824e9a677c9749a1956900908a46409c969c0c7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971857"
---
# <a name="list-keysets"></a><span data-ttu-id="82d38-103">列出 keySets</span><span class="sxs-lookup"><span data-stu-id="82d38-103">List keySets</span></span>

<span data-ttu-id="82d38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82d38-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82d38-105">检索 [trustFrameworkKeySets](../resources/trustframeworkkeyset.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="82d38-105">Retrieve a list of [trustFrameworkKeySets](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="82d38-106">权限</span><span class="sxs-lookup"><span data-stu-id="82d38-106">Permissions</span></span>

<span data-ttu-id="82d38-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82d38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="82d38-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="82d38-109">Permission type</span></span>                        | <span data-ttu-id="82d38-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="82d38-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="82d38-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82d38-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="82d38-112">TrustFrameworkKeySet、TrustFrameworkKeySet 和所有</span><span class="sxs-lookup"><span data-stu-id="82d38-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="82d38-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82d38-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82d38-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="82d38-114">Not supported.</span></span> |
| <span data-ttu-id="82d38-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="82d38-115">Application</span></span>                            | <span data-ttu-id="82d38-116">TrustFrameworkKeySet、TrustFrameworkKeySet 和所有</span><span class="sxs-lookup"><span data-stu-id="82d38-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82d38-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82d38-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="82d38-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="82d38-118">Request headers</span></span>

| <span data-ttu-id="82d38-119">名称</span><span class="sxs-lookup"><span data-stu-id="82d38-119">Name</span></span>      |<span data-ttu-id="82d38-120">说明</span><span class="sxs-lookup"><span data-stu-id="82d38-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="82d38-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="82d38-121">Authorization</span></span> | <span data-ttu-id="82d38-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="82d38-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82d38-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="82d38-124">Request body</span></span>

<span data-ttu-id="82d38-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="82d38-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82d38-126">响应</span><span class="sxs-lookup"><span data-stu-id="82d38-126">Response</span></span>

<span data-ttu-id="82d38-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="82d38-127">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="82d38-128">示例</span><span class="sxs-lookup"><span data-stu-id="82d38-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="82d38-129">请求</span><span class="sxs-lookup"><span data-stu-id="82d38-129">Request</span></span>

<span data-ttu-id="82d38-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="82d38-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="82d38-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="82d38-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_keysets"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets
```
# <a name="c"></a>[<span data-ttu-id="82d38-132">C#</span><span class="sxs-lookup"><span data-stu-id="82d38-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-keysets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="82d38-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="82d38-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-keysets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="82d38-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="82d38-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-keysets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="82d38-135">Java</span><span class="sxs-lookup"><span data-stu-id="82d38-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-keysets-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="82d38-136">响应</span><span class="sxs-lookup"><span data-stu-id="82d38-136">Response</span></span>

<span data-ttu-id="82d38-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="82d38-137">The following is an example of the response.</span></span>

> <span data-ttu-id="82d38-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="82d38-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
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
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List keySets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


