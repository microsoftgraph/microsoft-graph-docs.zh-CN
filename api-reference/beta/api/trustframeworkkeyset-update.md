---
title: 更新 trustFrameworkKeySet
description: 更新**trustFrameworkKeySet**对象的属性。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9f78bde00aee45dedc6d55d765aead8331605f0f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938221"
---
# <a name="update-trustframeworkkeyset"></a><span data-ttu-id="6e243-103">更新 trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="6e243-103">Update trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e243-104">更新[trustFrameworkKeyset](../resources/trustframeworkkeyset.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="6e243-104">Update the properties of a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="6e243-105">此操作将替换现有键集的内容。</span><span class="sxs-lookup"><span data-stu-id="6e243-105">This operation will replace the content of an existing keyset.</span></span> <span data-ttu-id="6e243-106">在请求负载中指定 ID 是可选的。</span><span class="sxs-lookup"><span data-stu-id="6e243-106">Specifying the ID in the request payload is optional.</span></span>

## <a name="permissions"></a><span data-ttu-id="6e243-107">权限</span><span class="sxs-lookup"><span data-stu-id="6e243-107">Permissions</span></span>

<span data-ttu-id="6e243-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e243-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6e243-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e243-110">Permission type</span></span>                        | <span data-ttu-id="6e243-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6e243-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6e243-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e243-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6e243-113">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="6e243-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="6e243-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e243-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6e243-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e243-115">Not supported.</span></span> |
| <span data-ttu-id="6e243-116">Application</span><span class="sxs-lookup"><span data-stu-id="6e243-116">Application</span></span>                            | <span data-ttu-id="6e243-117">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="6e243-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6e243-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e243-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6e243-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e243-119">Request headers</span></span>

| <span data-ttu-id="6e243-120">名称</span><span class="sxs-lookup"><span data-stu-id="6e243-120">Name</span></span>       | <span data-ttu-id="6e243-121">说明</span><span class="sxs-lookup"><span data-stu-id="6e243-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="6e243-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e243-122">Authorization</span></span> | <span data-ttu-id="6e243-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6e243-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6e243-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="6e243-125">Content-type</span></span>  | <span data-ttu-id="6e243-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6e243-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e243-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e243-128">Request body</span></span>


| <span data-ttu-id="6e243-129">属性</span><span class="sxs-lookup"><span data-stu-id="6e243-129">Property</span></span>     | <span data-ttu-id="6e243-130">类型</span><span class="sxs-lookup"><span data-stu-id="6e243-130">Type</span></span>        | <span data-ttu-id="6e243-131">描述</span><span class="sxs-lookup"><span data-stu-id="6e243-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6e243-132">标示</span><span class="sxs-lookup"><span data-stu-id="6e243-132">keys</span></span>|<span data-ttu-id="6e243-133">[trustFrameworkKey](../resources/trustframeworkkey.md)集合</span><span class="sxs-lookup"><span data-stu-id="6e243-133">[trustFrameworkKey](../resources/trustframeworkkey.md) collection</span></span>| <span data-ttu-id="6e243-134">更新 Trustframeworkkeys 的集合</span><span class="sxs-lookup"><span data-stu-id="6e243-134">updates a collection of Trustframeworkkeys</span></span>|

## <a name="response"></a><span data-ttu-id="6e243-135">响应</span><span class="sxs-lookup"><span data-stu-id="6e243-135">Response</span></span>

<span data-ttu-id="6e243-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[trustFrameworkKeySet](../resources/trustframeworkkeyset.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6e243-136">If successful, this method returns a `200 OK` response code and an updated [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6e243-137">示例</span><span class="sxs-lookup"><span data-stu-id="6e243-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6e243-138">请求</span><span class="sxs-lookup"><span data-stu-id="6e243-138">Request</span></span>

<span data-ttu-id="6e243-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6e243-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6e243-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="6e243-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_trustframeworkkeyset"
}-->

```http
PUT https://graph.microsoft.com/beta/trustFramework/keySets/{id}
Content-type: application/json

{
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6e243-141">C#</span><span class="sxs-lookup"><span data-stu-id="6e243-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6e243-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6e243-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6e243-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6e243-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6e243-144">响应</span><span class="sxs-lookup"><span data-stu-id="6e243-144">Response</span></span>

<span data-ttu-id="6e243-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6e243-145">The following is an example of the response.</span></span>

> <span data-ttu-id="6e243-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6e243-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Update trustframeworkkeyset",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
