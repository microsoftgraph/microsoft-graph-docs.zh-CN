---
title: 更新 trustFrameworkKeySet
description: 更新 **trustFrameworkKeySet 对象** 的属性。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c0375dbb052c061330d26120783f69d4a8327440
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053431"
---
# <a name="update-trustframeworkkeyset"></a><span data-ttu-id="0a169-103">更新 trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="0a169-103">Update trustFrameworkKeySet</span></span>

<span data-ttu-id="0a169-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a169-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a169-105">更新 [trustFrameworkKeyset 的属性](../resources/trustframeworkkeyset.md)。</span><span class="sxs-lookup"><span data-stu-id="0a169-105">Update the properties of a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="0a169-106">此操作将替换现有键集的内容。</span><span class="sxs-lookup"><span data-stu-id="0a169-106">This operation will replace the content of an existing keyset.</span></span> <span data-ttu-id="0a169-107">在请求有效负载中指定 ID 是可选的。</span><span class="sxs-lookup"><span data-stu-id="0a169-107">Specifying the ID in the request payload is optional.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a169-108">权限</span><span class="sxs-lookup"><span data-stu-id="0a169-108">Permissions</span></span>

<span data-ttu-id="0a169-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a169-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a169-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a169-111">Permission type</span></span>                        | <span data-ttu-id="0a169-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a169-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0a169-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a169-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a169-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a169-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="0a169-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a169-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a169-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a169-116">Not supported.</span></span> |
| <span data-ttu-id="0a169-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a169-117">Application</span></span>                            | <span data-ttu-id="0a169-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a169-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a169-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a169-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0a169-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a169-120">Request headers</span></span>

| <span data-ttu-id="0a169-121">名称</span><span class="sxs-lookup"><span data-stu-id="0a169-121">Name</span></span>       | <span data-ttu-id="0a169-122">说明</span><span class="sxs-lookup"><span data-stu-id="0a169-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0a169-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a169-123">Authorization</span></span> | <span data-ttu-id="0a169-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a169-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0a169-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="0a169-126">Content-type</span></span>  | <span data-ttu-id="0a169-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0a169-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a169-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a169-129">Request body</span></span>


| <span data-ttu-id="0a169-130">属性</span><span class="sxs-lookup"><span data-stu-id="0a169-130">Property</span></span>     | <span data-ttu-id="0a169-131">类型</span><span class="sxs-lookup"><span data-stu-id="0a169-131">Type</span></span>        | <span data-ttu-id="0a169-132">说明</span><span class="sxs-lookup"><span data-stu-id="0a169-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0a169-133">键</span><span class="sxs-lookup"><span data-stu-id="0a169-133">keys</span></span>|<span data-ttu-id="0a169-134">[trustFrameworkKey](../resources/trustframeworkkey.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0a169-134">[trustFrameworkKey](../resources/trustframeworkkey.md) collection</span></span>| <span data-ttu-id="0a169-135">更新 Trustframeworkkeys 的集合</span><span class="sxs-lookup"><span data-stu-id="0a169-135">updates a collection of Trustframeworkkeys</span></span>|

## <a name="response"></a><span data-ttu-id="0a169-136">响应</span><span class="sxs-lookup"><span data-stu-id="0a169-136">Response</span></span>

<span data-ttu-id="0a169-137">如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` 的 [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0a169-137">If successful, this method returns a `200 OK` response code and an updated [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0a169-138">示例</span><span class="sxs-lookup"><span data-stu-id="0a169-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a169-139">请求</span><span class="sxs-lookup"><span data-stu-id="0a169-139">Request</span></span>

<span data-ttu-id="0a169-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0a169-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a169-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a169-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0a169-142">C#</span><span class="sxs-lookup"><span data-stu-id="0a169-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a169-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a169-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a169-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a169-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a169-145">Java</span><span class="sxs-lookup"><span data-stu-id="0a169-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-trustframeworkkeyset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a169-146">响应</span><span class="sxs-lookup"><span data-stu-id="0a169-146">Response</span></span>

<span data-ttu-id="0a169-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0a169-147">The following is an example of the response.</span></span>

> <span data-ttu-id="0a169-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0a169-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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


