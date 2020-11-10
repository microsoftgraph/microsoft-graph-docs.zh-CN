---
title: 创建 trustFrameworkKeySet
description: 创建新的 **trustFrameworkKeySet** 对象。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c00701e2a6f1e370f2f646c225c2154a83441aa9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971828"
---
# <a name="create-trustframeworkkeyset"></a><span data-ttu-id="18152-103">创建 trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="18152-103">Create trustFrameworkKeySet</span></span>

<span data-ttu-id="18152-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18152-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18152-105">创建新的 [trustFrameworkKeySet](../resources/trustframeworkkeyset.md)。</span><span class="sxs-lookup"><span data-stu-id="18152-105">Create a new [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="18152-106">创建请求中应有 **trustFrameworkKeySet** 的 ID;但是，服务可以对其进行修改。</span><span class="sxs-lookup"><span data-stu-id="18152-106">The ID of the **trustFrameworkKeySet** is expected in the create request; however, it can be modified by the service.</span></span> <span data-ttu-id="18152-107">已修改的 ID 将出现在响应中和位置标头中。</span><span class="sxs-lookup"><span data-stu-id="18152-107">The modified ID will be available in the response and in the location header.</span></span>

## <a name="permissions"></a><span data-ttu-id="18152-108">权限</span><span class="sxs-lookup"><span data-stu-id="18152-108">Permissions</span></span>

<span data-ttu-id="18152-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18152-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18152-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="18152-111">Permission type</span></span>                        | <span data-ttu-id="18152-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18152-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="18152-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18152-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="18152-114">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="18152-114">TrustFrameworkKeySet.ReadWrite.All</span></span>   |
| <span data-ttu-id="18152-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18152-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18152-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="18152-116">Not supported.</span></span> |
| <span data-ttu-id="18152-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="18152-117">Application</span></span>                            | <span data-ttu-id="18152-118">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="18152-118">TrustFrameworkKeySet.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="18152-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18152-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="18152-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="18152-120">Request headers</span></span>

| <span data-ttu-id="18152-121">名称</span><span class="sxs-lookup"><span data-stu-id="18152-121">Name</span></span>          | <span data-ttu-id="18152-122">说明</span><span class="sxs-lookup"><span data-stu-id="18152-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="18152-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="18152-123">Authorization</span></span> | <span data-ttu-id="18152-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="18152-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="18152-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="18152-126">Content-type</span></span> | <span data-ttu-id="18152-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="18152-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18152-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="18152-129">Request body</span></span>

<span data-ttu-id="18152-130">在请求正文中，提供 [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18152-130">In the request body, supply a JSON representation of a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="18152-131">响应</span><span class="sxs-lookup"><span data-stu-id="18152-131">Response</span></span>

<span data-ttu-id="18152-132">如果成功，此方法将在 `201 Created` 响应正文中返回响应代码、新创建的对象的位置标头和新的 [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18152-132">If successful, this method returns a `201 Created` response code, a location header for the newly created object, and a new [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18152-133">示例</span><span class="sxs-lookup"><span data-stu-id="18152-133">Examples</span></span>

### <a name="example-1-create-an-empty-keyset"></a><span data-ttu-id="18152-134">示例1：创建空键集</span><span class="sxs-lookup"><span data-stu-id="18152-134">Example 1: Create an empty keyset</span></span>
<span data-ttu-id="18152-135">这是最有用的操作之一。</span><span class="sxs-lookup"><span data-stu-id="18152-135">This is one of the most useful operations.</span></span> <span data-ttu-id="18152-136">首先，创建一个空键集。</span><span class="sxs-lookup"><span data-stu-id="18152-136">First, you create an empty keyset.</span></span> <span data-ttu-id="18152-137">然后，在新的密钥集中，您可以生成密钥，上载手动机密，并上传证书或 PKCS12 密钥。</span><span class="sxs-lookup"><span data-stu-id="18152-137">Then, in the new keyset, you can generate a key, upload a manual secret, and upload a certificate or a PKCS12 key.</span></span> 

#### <a name="request"></a><span data-ttu-id="18152-138">请求</span><span class="sxs-lookup"><span data-stu-id="18152-138">Request</span></span>

<span data-ttu-id="18152-139">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="18152-139">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18152-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="18152-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkkeyset_from_trustframework1"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets
Content-type: application/json

{
  "id": "keyset1"  
}
```
# <a name="c"></a>[<span data-ttu-id="18152-141">C#</span><span class="sxs-lookup"><span data-stu-id="18152-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-trustframeworkkeyset-from-trustframework-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18152-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18152-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-trustframeworkkeyset-from-trustframework-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18152-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18152-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-trustframeworkkeyset-from-trustframework-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18152-144">Java</span><span class="sxs-lookup"><span data-stu-id="18152-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-trustframeworkkeyset-from-trustframework-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="18152-145">响应</span><span class="sxs-lookup"><span data-stu-id="18152-145">Response</span></span>

<span data-ttu-id="18152-146">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="18152-146">The following example shows the response.</span></span>

> <span data-ttu-id="18152-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="18152-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Location: /trustFramework/keySets('B2C_1A_keyset1')

{
  "id": "B2C_1A_keyset1",
  "keys": []
}
```

### <a name="example-2-create-a-keyset-with-a-key"></a><span data-ttu-id="18152-149">示例2：创建具有键的键集</span><span class="sxs-lookup"><span data-stu-id="18152-149">Example 2: Create a keyset with a key</span></span>

<span data-ttu-id="18152-150">这是一种高级方案，需要知道密钥的 [RFC 7517](https://tools.ietf.org/html/rfc7517#section-5) 兼容 JSON Web 密钥格式。</span><span class="sxs-lookup"><span data-stu-id="18152-150">This is an advanced scenario where you need to know the [RFC 7517](https://tools.ietf.org/html/rfc7517#section-5) compliant JSON Web Key format of the key.</span></span>

#### <a name="request"></a><span data-ttu-id="18152-151">请求</span><span class="sxs-lookup"><span data-stu-id="18152-151">Request</span></span>

<span data-ttu-id="18152-152">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="18152-152">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkkeyset_from_trustframework"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets
Content-type: application/json

{
  "id": "keyset1",
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

#### <a name="response"></a><span data-ttu-id="18152-153">响应</span><span class="sxs-lookup"><span data-stu-id="18152-153">Response</span></span>

<span data-ttu-id="18152-154">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="18152-154">The following example shows the response.</span></span>

> <span data-ttu-id="18152-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="18152-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Location: /trustFramework/keySets('B2C_1A_keyset1')

{
  "id": "B2C_1A_keyset1",
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
  "description": "Create trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


