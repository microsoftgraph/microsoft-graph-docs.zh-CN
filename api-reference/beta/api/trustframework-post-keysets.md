---
title: 创建 trustFrameworkKeySet
description: 创建新的**trustFrameworkKeySet**对象。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b6cd03a38e4e115befacb13909d1ba0040b3aff
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734557"
---
# <a name="create-trustframeworkkeyset"></a><span data-ttu-id="170b4-103">创建 trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="170b4-103">Create trustFrameworkKeySet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="170b4-104">创建新的[trustFrameworkKeySet](../resources/trustframeworkkeyset.md)。</span><span class="sxs-lookup"><span data-stu-id="170b4-104">Create a new [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="170b4-105">创建请求中应有**trustFrameworkKeySet**的 ID;但是，服务可以对其进行修改。</span><span class="sxs-lookup"><span data-stu-id="170b4-105">The ID of the **trustFrameworkKeySet** is expected in the create request; however, it can be modified by the service.</span></span> <span data-ttu-id="170b4-106">已修改的 ID 将出现在响应中和位置标头中。</span><span class="sxs-lookup"><span data-stu-id="170b4-106">The modified ID will be available in the response and in the location header.</span></span>

## <a name="permissions"></a><span data-ttu-id="170b4-107">权限</span><span class="sxs-lookup"><span data-stu-id="170b4-107">Permissions</span></span>

<span data-ttu-id="170b4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="170b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="170b4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="170b4-110">Permission type</span></span>                        | <span data-ttu-id="170b4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="170b4-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="170b4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="170b4-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="170b4-113">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="170b4-113">TrustFrameworkKeySet.ReadWrite.All</span></span>   |
| <span data-ttu-id="170b4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="170b4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="170b4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="170b4-115">Not supported.</span></span> |
| <span data-ttu-id="170b4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="170b4-116">Application</span></span>                            | <span data-ttu-id="170b4-117">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="170b4-117">TrustFrameworkKeySet.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="170b4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="170b4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets
```

## <a name="request-headers"></a><span data-ttu-id="170b4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="170b4-119">Request headers</span></span>

| <span data-ttu-id="170b4-120">名称</span><span class="sxs-lookup"><span data-stu-id="170b4-120">Name</span></span>          | <span data-ttu-id="170b4-121">说明</span><span class="sxs-lookup"><span data-stu-id="170b4-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="170b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="170b4-122">Authorization</span></span> | <span data-ttu-id="170b4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="170b4-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="170b4-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="170b4-125">Content-type</span></span> | <span data-ttu-id="170b4-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="170b4-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="170b4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="170b4-128">Request body</span></span>

<span data-ttu-id="170b4-129">在请求正文中，提供[trustFrameworkKeySet](../resources/trustframeworkkeyset.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="170b4-129">In the request body, supply a JSON representation of a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="170b4-130">响应</span><span class="sxs-lookup"><span data-stu-id="170b4-130">Response</span></span>

<span data-ttu-id="170b4-131">如果成功，此方法将在`201 Created`响应正文中返回响应代码、新创建的对象的位置标头和新的[trustFrameworkKeySet](../resources/trustframeworkkeyset.md)对象。</span><span class="sxs-lookup"><span data-stu-id="170b4-131">If successful, this method returns a `201 Created` response code, a location header for the newly created object, and a new [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="170b4-132">示例</span><span class="sxs-lookup"><span data-stu-id="170b4-132">Examples</span></span>

### <a name="example-1-create-an-empty-keyset"></a><span data-ttu-id="170b4-133">示例1：创建空键集</span><span class="sxs-lookup"><span data-stu-id="170b4-133">Example 1: Create an empty keyset</span></span>
<span data-ttu-id="170b4-134">此模式创建一个 enpty 键集，然后生成一个密钥，上载一个手动机密，并在大多数情况下上传证书或 PKCS12 密钥是足够的。</span><span class="sxs-lookup"><span data-stu-id="170b4-134">This pattern to create an enpty keyset and then generate a key, upload a manual secret, and upload a certificate or a PKCS12 key is sufficient for most scenarios.</span></span> 

#### <a name="request"></a><span data-ttu-id="170b4-135">请求</span><span class="sxs-lookup"><span data-stu-id="170b4-135">Request</span></span>

<span data-ttu-id="170b4-136">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="170b4-136">The following example shows the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="170b4-137">响应</span><span class="sxs-lookup"><span data-stu-id="170b4-137">Response</span></span>

<span data-ttu-id="170b4-138">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="170b4-138">The following example shows the response.</span></span>

> <span data-ttu-id="170b4-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="170b4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-a-keyset-with-a-key"></a><span data-ttu-id="170b4-141">示例2：创建具有键的键集</span><span class="sxs-lookup"><span data-stu-id="170b4-141">Example 2: Create a keyset with a key</span></span>

<span data-ttu-id="170b4-142">这是一种高级方案，需要知道密钥的[RFC 7517](https://tools.ietf.org/html/rfc7517#section-5)兼容 JSON Web 密钥格式。</span><span class="sxs-lookup"><span data-stu-id="170b4-142">This is an advanced scenario where you need to know the [RFC 7517](https://tools.ietf.org/html/rfc7517#section-5) compliant JSON Web Key format of the key.</span></span>

#### <a name="request"></a><span data-ttu-id="170b4-143">请求</span><span class="sxs-lookup"><span data-stu-id="170b4-143">Request</span></span>

<span data-ttu-id="170b4-144">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="170b4-144">The following example shows the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="170b4-145">响应</span><span class="sxs-lookup"><span data-stu-id="170b4-145">Response</span></span>

<span data-ttu-id="170b4-146">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="170b4-146">The following example shows the response.</span></span>

> <span data-ttu-id="170b4-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="170b4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
