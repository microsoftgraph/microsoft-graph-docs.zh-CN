---
title: trustFrameworkKeySet： generateKey
description: 在密钥集内自动生成密钥和密码。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6ffcb8beb1744d8ca702ed1d9fd550721b6e7747
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433653"
---
# <a name="trustframeworkkeyset-generatekey"></a><span data-ttu-id="15a5c-103">trustFrameworkKeySet： generateKey</span><span class="sxs-lookup"><span data-stu-id="15a5c-103">trustFrameworkKeySet: generateKey</span></span>

<span data-ttu-id="15a5c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15a5c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15a5c-105">在 [trustFrameworkKeyset](../resources/trustFrameworkKey.md) 中自动生成 [trustFrameworkKey](../resources/trustframeworkkeyset.md)和密码。</span><span class="sxs-lookup"><span data-stu-id="15a5c-105">Generate a [trustFrameworkKey](../resources/trustFrameworkKey.md) and a secret automatically in the [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="15a5c-106">呼叫者不必提供机密。</span><span class="sxs-lookup"><span data-stu-id="15a5c-106">The caller doesn't have to provide a secret.</span></span>

## <a name="permissions"></a><span data-ttu-id="15a5c-107">权限</span><span class="sxs-lookup"><span data-stu-id="15a5c-107">Permissions</span></span>

<span data-ttu-id="15a5c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="15a5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15a5c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="15a5c-110">Permission type</span></span>                        | <span data-ttu-id="15a5c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="15a5c-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="15a5c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15a5c-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="15a5c-113">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15a5c-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="15a5c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15a5c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15a5c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="15a5c-115">Not supported.</span></span> |
| <span data-ttu-id="15a5c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="15a5c-116">Application</span></span>                            | <span data-ttu-id="15a5c-117">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15a5c-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="15a5c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15a5c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/generateKey
```

## <a name="request-headers"></a><span data-ttu-id="15a5c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="15a5c-119">Request headers</span></span>

| <span data-ttu-id="15a5c-120">名称</span><span class="sxs-lookup"><span data-stu-id="15a5c-120">Name</span></span>          | <span data-ttu-id="15a5c-121">说明</span><span class="sxs-lookup"><span data-stu-id="15a5c-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="15a5c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15a5c-122">Authorization</span></span> | <span data-ttu-id="15a5c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="15a5c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15a5c-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="15a5c-125">Content-type</span></span>  | <span data-ttu-id="15a5c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="15a5c-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15a5c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="15a5c-128">Request body</span></span>

<span data-ttu-id="15a5c-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="15a5c-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="15a5c-130">参数</span><span class="sxs-lookup"><span data-stu-id="15a5c-130">Parameter</span></span>    | <span data-ttu-id="15a5c-131">类型</span><span class="sxs-lookup"><span data-stu-id="15a5c-131">Type</span></span>        | <span data-ttu-id="15a5c-132">说明</span><span class="sxs-lookup"><span data-stu-id="15a5c-132">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="15a5c-133">use</span><span class="sxs-lookup"><span data-stu-id="15a5c-133">use</span></span> | <span data-ttu-id="15a5c-134">string</span><span class="sxs-lookup"><span data-stu-id="15a5c-134">string</span></span> | <span data-ttu-id="15a5c-135">类似于 **trustFrameworkKey 的 use 属性**。 </span><span class="sxs-lookup"><span data-stu-id="15a5c-135">Similar to the **use** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="15a5c-136">kty</span><span class="sxs-lookup"><span data-stu-id="15a5c-136">kty</span></span> | <span data-ttu-id="15a5c-137">string</span><span class="sxs-lookup"><span data-stu-id="15a5c-137">string</span></span> | <span data-ttu-id="15a5c-138">类似于 **trustFrameworkKey** 的 **kty** 属性。</span><span class="sxs-lookup"><span data-stu-id="15a5c-138">Similar to **kty** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="15a5c-139">nbf</span><span class="sxs-lookup"><span data-stu-id="15a5c-139">nbf</span></span> | <span data-ttu-id="15a5c-140">int</span><span class="sxs-lookup"><span data-stu-id="15a5c-140">int</span></span> | <span data-ttu-id="15a5c-141">类似于 **trustFrameworkKey** 的 **nbf** 属性。</span><span class="sxs-lookup"><span data-stu-id="15a5c-141">Similar to **nbf** property of **trustFrameworkKey**.</span></span> |
| <span data-ttu-id="15a5c-142">exp</span><span class="sxs-lookup"><span data-stu-id="15a5c-142">exp</span></span> | <span data-ttu-id="15a5c-143">int</span><span class="sxs-lookup"><span data-stu-id="15a5c-143">int</span></span> | <span data-ttu-id="15a5c-144">类似于 **trustFrameworkKey 的 exp 属性**。</span><span class="sxs-lookup"><span data-stu-id="15a5c-144">Similar to **exp** property of **trustFrameworkKey**.</span></span> |

## <a name="response"></a><span data-ttu-id="15a5c-145">响应</span><span class="sxs-lookup"><span data-stu-id="15a5c-145">Response</span></span>

<span data-ttu-id="15a5c-146">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和新的 [trustFrameworkKey](../resources/trustframeworkkey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="15a5c-146">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15a5c-147">示例</span><span class="sxs-lookup"><span data-stu-id="15a5c-147">Examples</span></span>

### <a name="request"></a><span data-ttu-id="15a5c-148">请求</span><span class="sxs-lookup"><span data-stu-id="15a5c-148">Request</span></span>

<span data-ttu-id="15a5c-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="15a5c-149">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="15a5c-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="15a5c-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_generatekey"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/generateKey
Content-type: application/json

{
  "use": "sig",
  "kty": "RSA",
  "nbf": 1508969811,
  "exp": 1508969811
}
```
# <a name="c"></a>[<span data-ttu-id="15a5c-151">C#</span><span class="sxs-lookup"><span data-stu-id="15a5c-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-generatekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15a5c-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15a5c-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-generatekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15a5c-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15a5c-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-generatekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15a5c-154">Java</span><span class="sxs-lookup"><span data-stu-id="15a5c-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-generatekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="15a5c-155">响应</span><span class="sxs-lookup"><span data-stu-id="15a5c-155">Response</span></span>

<span data-ttu-id="15a5c-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="15a5c-156">The following is an example of the response.</span></span>

> <span data-ttu-id="15a5c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="15a5c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.trustFrameworkKey",
    "k": null,
    "x5c": [],
    "kty": "RSA",
    "use": "sig",
    "exp": 1908969811,
    "nbf": 1908969811,
    "kid": "Gaid7K8sO8RavMX9fzHir_Wg0femGhbY9b-B4rVIxbE",
    "e": "AQAB",
    "n": "rd54s6",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: generateKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


