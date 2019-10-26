---
title: 获取 trustFrameworkKeySet
description: 检索 trustframeworkkeyset 对象的属性和关系。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e70f0cf3e7eaae0add9da7ded068b8c3517529bc
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734548"
---
# <a name="get-trustframeworkkeyset"></a><span data-ttu-id="0323b-103">获取 trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="0323b-103">Get trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0323b-104">检索[Trustframeworkkeyset](../resources/trustframeworkkeyset.md)的属性和关联。</span><span class="sxs-lookup"><span data-stu-id="0323b-104">Retrieve the properties and associations for a [Trustframeworkkeyset](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0323b-105">权限</span><span class="sxs-lookup"><span data-stu-id="0323b-105">Permissions</span></span>

<span data-ttu-id="0323b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0323b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0323b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0323b-108">Permission type</span></span>                        | <span data-ttu-id="0323b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0323b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0323b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0323b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0323b-111">TrustFrameworkKeySet、TrustFrameworkKeySet 和所有</span><span class="sxs-lookup"><span data-stu-id="0323b-111">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="0323b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0323b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0323b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0323b-113">Not supported.</span></span> |
| <span data-ttu-id="0323b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0323b-114">Application</span></span>                            | <span data-ttu-id="0323b-115">TrustFrameworkKeySet、TrustFrameworkKeySet 和所有</span><span class="sxs-lookup"><span data-stu-id="0323b-115">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0323b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0323b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0323b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0323b-117">Request headers</span></span>

| <span data-ttu-id="0323b-118">名称</span><span class="sxs-lookup"><span data-stu-id="0323b-118">Name</span></span>      |<span data-ttu-id="0323b-119">说明</span><span class="sxs-lookup"><span data-stu-id="0323b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0323b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0323b-120">Authorization</span></span> | <span data-ttu-id="0323b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0323b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0323b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0323b-123">Request body</span></span>

<span data-ttu-id="0323b-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0323b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0323b-125">响应</span><span class="sxs-lookup"><span data-stu-id="0323b-125">Response</span></span>

<span data-ttu-id="0323b-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[trustFrameworkKeySet](../resources/trustframeworkkeyset.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0323b-126">If successful, this method returns a `200 OK` response code and the requested [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0323b-127">示例</span><span class="sxs-lookup"><span data-stu-id="0323b-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0323b-128">请求</span><span class="sxs-lookup"><span data-stu-id="0323b-128">Request</span></span>

<span data-ttu-id="0323b-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0323b-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_trustframeworkkeyset"
}-->

```http
GET https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```

### <a name="response"></a><span data-ttu-id="0323b-130">响应</span><span class="sxs-lookup"><span data-stu-id="0323b-130">Response</span></span>

<span data-ttu-id="0323b-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0323b-131">The following is an example of the response.</span></span>

> <span data-ttu-id="0323b-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0323b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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