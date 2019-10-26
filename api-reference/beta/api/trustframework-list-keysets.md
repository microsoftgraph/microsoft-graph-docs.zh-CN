---
title: 列出 keySets
description: 检索 trustframeworkkeyset 对象的列表。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 229ec09241de019910781a3bf37fe2c39db2c399
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734560"
---
# <a name="list-keysets"></a><span data-ttu-id="1103e-103">列出 keySets</span><span class="sxs-lookup"><span data-stu-id="1103e-103">List keySets</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1103e-104">检索[trustFrameworkKeySets](../resources/trustframeworkkeyset.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="1103e-104">Retrieve a list of [trustFrameworkKeySets](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1103e-105">权限</span><span class="sxs-lookup"><span data-stu-id="1103e-105">Permissions</span></span>

<span data-ttu-id="1103e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1103e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1103e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1103e-108">Permission type</span></span>                        | <span data-ttu-id="1103e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1103e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1103e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1103e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1103e-111">TrustFrameworkKeySet、TrustFrameworkKeySet 和所有</span><span class="sxs-lookup"><span data-stu-id="1103e-111">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="1103e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1103e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1103e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1103e-113">Not supported.</span></span> |
| <span data-ttu-id="1103e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1103e-114">Application</span></span>                            | <span data-ttu-id="1103e-115">TrustFrameworkKeySet、TrustFrameworkKeySet 和所有</span><span class="sxs-lookup"><span data-stu-id="1103e-115">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1103e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1103e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="1103e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1103e-117">Request headers</span></span>

| <span data-ttu-id="1103e-118">名称</span><span class="sxs-lookup"><span data-stu-id="1103e-118">Name</span></span>      |<span data-ttu-id="1103e-119">说明</span><span class="sxs-lookup"><span data-stu-id="1103e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1103e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1103e-120">Authorization</span></span> | <span data-ttu-id="1103e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1103e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1103e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1103e-123">Request body</span></span>

<span data-ttu-id="1103e-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1103e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1103e-125">响应</span><span class="sxs-lookup"><span data-stu-id="1103e-125">Response</span></span>

<span data-ttu-id="1103e-126">如果成功，此方法在响应`200 OK`正文中返回响应代码和[trustFrameworkKeySet](../resources/trustframeworkkeyset.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="1103e-126">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1103e-127">示例</span><span class="sxs-lookup"><span data-stu-id="1103e-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1103e-128">请求</span><span class="sxs-lookup"><span data-stu-id="1103e-128">Request</span></span>

<span data-ttu-id="1103e-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1103e-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_keysets"
}-->

```http
GET https://graph.microsoft.com/beta/trustFramework/keySets
```

### <a name="response"></a><span data-ttu-id="1103e-130">响应</span><span class="sxs-lookup"><span data-stu-id="1103e-130">Response</span></span>

<span data-ttu-id="1103e-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1103e-131">The following is an example of the response.</span></span>

> <span data-ttu-id="1103e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1103e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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