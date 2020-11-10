---
title: 'trustFrameworkKeySet: getActiveKey'
description: 获取键集中的活动键。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d387cbeb9dc668f3c52583ef1573ad3951aed8ee
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980942"
---
# <a name="trustframeworkkeyset-getactivekey"></a><span data-ttu-id="41e21-103">trustFrameworkKeySet: getActiveKey</span><span class="sxs-lookup"><span data-stu-id="41e21-103">trustFrameworkKeySet: getActiveKey</span></span>

<span data-ttu-id="41e21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41e21-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41e21-105">获取[trustFrameworkKeySet](../resources/trustframeworkkeyset.md)中当前处于活动状态的[trustFrameworkKey](../resources/trustframeworkkey.md) 。</span><span class="sxs-lookup"><span data-stu-id="41e21-105">Get the currently active [trustFrameworkKey](../resources/trustframeworkkey.md) in a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="41e21-106">键集中一次只能有一个键处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="41e21-106">Only one key is active in the keyset at a time.</span></span>


## <a name="permissions"></a><span data-ttu-id="41e21-107">权限</span><span class="sxs-lookup"><span data-stu-id="41e21-107">Permissions</span></span>

<span data-ttu-id="41e21-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41e21-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="41e21-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="41e21-110">Permission type</span></span>                        | <span data-ttu-id="41e21-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41e21-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="41e21-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41e21-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="41e21-113">TrustFrameworkKeySet、TrustFrameworkKeySet 和所有</span><span class="sxs-lookup"><span data-stu-id="41e21-113">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="41e21-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41e21-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41e21-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="41e21-115">Not supported.</span></span> |
| <span data-ttu-id="41e21-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="41e21-116">Application</span></span>                            | <span data-ttu-id="41e21-117">TrustFrameworkKeySet、TrustFrameworkKeySet 和所有</span><span class="sxs-lookup"><span data-stu-id="41e21-117">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41e21-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41e21-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /trustFramework/keySets/{id}/getActiveKey
```

## <a name="request-headers"></a><span data-ttu-id="41e21-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="41e21-119">Request headers</span></span>

| <span data-ttu-id="41e21-120">名称</span><span class="sxs-lookup"><span data-stu-id="41e21-120">Name</span></span>          | <span data-ttu-id="41e21-121">说明</span><span class="sxs-lookup"><span data-stu-id="41e21-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="41e21-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41e21-122">Authorization</span></span> | <span data-ttu-id="41e21-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41e21-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41e21-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="41e21-125">Request body</span></span>

<span data-ttu-id="41e21-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41e21-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41e21-127">响应</span><span class="sxs-lookup"><span data-stu-id="41e21-127">Response</span></span>

<span data-ttu-id="41e21-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和新的 [trustFrameworkKey](../resources/trustframeworkkey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41e21-128">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="41e21-129">示例</span><span class="sxs-lookup"><span data-stu-id="41e21-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="41e21-130">请求</span><span class="sxs-lookup"><span data-stu-id="41e21-130">Request</span></span>

<span data-ttu-id="41e21-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="41e21-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41e21-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="41e21-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_getactivekey"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/keySets/{id}/getActiveKey
```
# <a name="c"></a>[<span data-ttu-id="41e21-133">C#</span><span class="sxs-lookup"><span data-stu-id="41e21-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-getactivekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41e21-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41e21-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-getactivekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41e21-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41e21-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-getactivekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41e21-136">Java</span><span class="sxs-lookup"><span data-stu-id="41e21-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-getactivekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41e21-137">响应</span><span class="sxs-lookup"><span data-stu-id="41e21-137">Response</span></span>

<span data-ttu-id="41e21-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="41e21-138">The following is an example of the response.</span></span>

> <span data-ttu-id="41e21-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="41e21-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "k": "k-value",
  "x5c": [
    "x5c-value"
  ],
  "x5t": "x5t-value",
  "kty": "kty-value",
  "use": "use-value",
  "exp": 99
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: getActiveKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


