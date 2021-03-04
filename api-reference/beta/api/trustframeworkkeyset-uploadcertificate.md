---
title: trustFrameworkKeySet： uploadCertificate
description: 将证书上载到密钥集。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 279794743f6f6b4cbd80fd9b3793195a73ff0e18
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433612"
---
# <a name="trustframeworkkeyset-uploadcertificate"></a><span data-ttu-id="684bb-103">trustFrameworkKeySet： uploadCertificate</span><span class="sxs-lookup"><span data-stu-id="684bb-103">trustFrameworkKeySet: uploadCertificate</span></span>

<span data-ttu-id="684bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="684bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="684bb-105">将证书上载到 [trustFrameworkKeyset](../resources/trustframeworkkeyset.md)。</span><span class="sxs-lookup"><span data-stu-id="684bb-105">Upload a certificate to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="684bb-106">输入是证书内容的 base-64 编码值。</span><span class="sxs-lookup"><span data-stu-id="684bb-106">The input is a base-64 encoded value of the certificate contents.</span></span> <span data-ttu-id="684bb-107">此方法返回 [trustFrameworkKey](../resources/trustframeworkkey.md)。</span><span class="sxs-lookup"><span data-stu-id="684bb-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="684bb-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="684bb-108">Permissions</span></span>

<span data-ttu-id="684bb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="684bb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="684bb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="684bb-111">Permission type</span></span>                        | <span data-ttu-id="684bb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="684bb-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="684bb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="684bb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="684bb-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="684bb-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="684bb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="684bb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="684bb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="684bb-116">Not supported.</span></span> |
| <span data-ttu-id="684bb-117">Application</span><span class="sxs-lookup"><span data-stu-id="684bb-117">Application</span></span>                            | <span data-ttu-id="684bb-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="684bb-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="684bb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="684bb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadCertificate
```

## <a name="request-headers"></a><span data-ttu-id="684bb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="684bb-120">Request headers</span></span>

| <span data-ttu-id="684bb-121">名称</span><span class="sxs-lookup"><span data-stu-id="684bb-121">Name</span></span>          | <span data-ttu-id="684bb-122">说明</span><span class="sxs-lookup"><span data-stu-id="684bb-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="684bb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="684bb-123">Authorization</span></span> | <span data-ttu-id="684bb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="684bb-p103">Bearer {token}. Required.</span></span> |
|<span data-ttu-id="684bb-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="684bb-126">Content-type</span></span> | <span data-ttu-id="684bb-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="684bb-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="684bb-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="684bb-129">Request body</span></span>

<span data-ttu-id="684bb-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="684bb-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="684bb-131">参数</span><span class="sxs-lookup"><span data-stu-id="684bb-131">Parameter</span></span>    | <span data-ttu-id="684bb-132">类型</span><span class="sxs-lookup"><span data-stu-id="684bb-132">Type</span></span>        | <span data-ttu-id="684bb-133">说明</span><span class="sxs-lookup"><span data-stu-id="684bb-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="684bb-134">Key</span><span class="sxs-lookup"><span data-stu-id="684bb-134">key</span></span>|<span data-ttu-id="684bb-135">String</span><span class="sxs-lookup"><span data-stu-id="684bb-135">String</span></span>| <span data-ttu-id="684bb-136">这是用于发送证书内容的字段。</span><span class="sxs-lookup"><span data-stu-id="684bb-136">This is the field for sending certificate content.</span></span> <span data-ttu-id="684bb-137">该值应为实际证书内容的 base-64 编码版本。</span><span class="sxs-lookup"><span data-stu-id="684bb-137">The value should be a base-64 encoded version of the actual certificate content.</span></span> |

## <a name="response"></a><span data-ttu-id="684bb-138">响应</span><span class="sxs-lookup"><span data-stu-id="684bb-138">Response</span></span>

<span data-ttu-id="684bb-139">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和新的 [trustFrameworkKey](../resources/trustframeworkkey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="684bb-139">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="684bb-140">示例</span><span class="sxs-lookup"><span data-stu-id="684bb-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="684bb-141">请求</span><span class="sxs-lookup"><span data-stu-id="684bb-141">Request</span></span>

<span data-ttu-id="684bb-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="684bb-142">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="684bb-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="684bb-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadcertificate"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadCertificate
Content-type: application/json

{
  "key": "key-value"
}
```
# <a name="c"></a>[<span data-ttu-id="684bb-144">C#</span><span class="sxs-lookup"><span data-stu-id="684bb-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadcertificate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="684bb-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="684bb-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadcertificate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="684bb-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="684bb-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadcertificate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="684bb-147">Java</span><span class="sxs-lookup"><span data-stu-id="684bb-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-uploadcertificate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="684bb-148">响应</span><span class="sxs-lookup"><span data-stu-id="684bb-148">Response</span></span>

<span data-ttu-id="684bb-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="684bb-149">The following is an example of the response.</span></span>

> <span data-ttu-id="684bb-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="684bb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "kid": "kid-value",
    "use": "sig",
    "kty": "oct",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadCertificate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


