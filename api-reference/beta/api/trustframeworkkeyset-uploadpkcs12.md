---
title: trustFrameworkKeySet： uploadPkcs12
description: 将 PKCS 12 格式密钥 (PFX) 到密钥集。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9de90df699c3086261321b38375373a00b464da1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433593"
---
# <a name="trustframeworkkeyset-uploadpkcs12"></a><span data-ttu-id="7be16-103">trustFrameworkKeySet： uploadPkcs12</span><span class="sxs-lookup"><span data-stu-id="7be16-103">trustFrameworkKeySet: uploadPkcs12</span></span>

<span data-ttu-id="7be16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7be16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7be16-105">将 PKCS12 格式密钥 (PFX) [trustFrameworkKeyset。](../resources/trustframeworkkeyset.md)</span><span class="sxs-lookup"><span data-stu-id="7be16-105">Upload a PKCS12 format key (PFX) to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="7be16-106">输入是 Pfx 证书内容的 base-64 编码值。</span><span class="sxs-lookup"><span data-stu-id="7be16-106">The input is a base-64 encoded value of the Pfx certificate contents.</span></span> <span data-ttu-id="7be16-107">此方法返回 [trustFrameworkKey](../resources/trustframeworkkey.md)。</span><span class="sxs-lookup"><span data-stu-id="7be16-107">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7be16-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="7be16-108">Permissions</span></span>

<span data-ttu-id="7be16-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7be16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7be16-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7be16-111">Permission type</span></span>                        | <span data-ttu-id="7be16-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7be16-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7be16-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7be16-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7be16-114">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7be16-114">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="7be16-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7be16-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7be16-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7be16-116">Not supported.</span></span> |
| <span data-ttu-id="7be16-117">Application</span><span class="sxs-lookup"><span data-stu-id="7be16-117">Application</span></span>                            | <span data-ttu-id="7be16-118">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7be16-118">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7be16-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7be16-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadPkcs12
```

## <a name="request-headers"></a><span data-ttu-id="7be16-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7be16-120">Request headers</span></span>

| <span data-ttu-id="7be16-121">名称</span><span class="sxs-lookup"><span data-stu-id="7be16-121">Name</span></span>          | <span data-ttu-id="7be16-122">说明</span><span class="sxs-lookup"><span data-stu-id="7be16-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7be16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7be16-123">Authorization</span></span> | <span data-ttu-id="7be16-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7be16-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7be16-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="7be16-126">Content-type</span></span>  | <span data-ttu-id="7be16-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7be16-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7be16-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7be16-129">Request body</span></span>

<span data-ttu-id="7be16-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7be16-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7be16-131">参数</span><span class="sxs-lookup"><span data-stu-id="7be16-131">Parameter</span></span>    | <span data-ttu-id="7be16-132">类型</span><span class="sxs-lookup"><span data-stu-id="7be16-132">Type</span></span>        | <span data-ttu-id="7be16-133">说明</span><span class="sxs-lookup"><span data-stu-id="7be16-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7be16-134">Key</span><span class="sxs-lookup"><span data-stu-id="7be16-134">key</span></span>|<span data-ttu-id="7be16-135">String</span><span class="sxs-lookup"><span data-stu-id="7be16-135">String</span></span>|<span data-ttu-id="7be16-136">这是用于发送 pfx 内容的字段。</span><span class="sxs-lookup"><span data-stu-id="7be16-136">This is the field for sending pfx content.</span></span> <span data-ttu-id="7be16-137">该值应为实际证书内容的 base-64 编码版本。</span><span class="sxs-lookup"><span data-stu-id="7be16-137">The value should be a base-64 encoded version of the actual certificate content.</span></span>|
|<span data-ttu-id="7be16-138">密码</span><span class="sxs-lookup"><span data-stu-id="7be16-138">password</span></span>|<span data-ttu-id="7be16-139">String</span><span class="sxs-lookup"><span data-stu-id="7be16-139">String</span></span>|<span data-ttu-id="7be16-140">这是用于将密码发送到 PFX 内容的字段。</span><span class="sxs-lookup"><span data-stu-id="7be16-140">This is the field for sending the password to PFX content.</span></span>|

## <a name="response"></a><span data-ttu-id="7be16-141">响应</span><span class="sxs-lookup"><span data-stu-id="7be16-141">Response</span></span>

<span data-ttu-id="7be16-142">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和新的 [trustFrameworkKey](../resources/trustframeworkkey.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7be16-142">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7be16-143">示例</span><span class="sxs-lookup"><span data-stu-id="7be16-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7be16-144">请求</span><span class="sxs-lookup"><span data-stu-id="7be16-144">Request</span></span>

<span data-ttu-id="7be16-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7be16-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7be16-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="7be16-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_uploadpkcs12"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/uploadPkcs12
Content-type: application/json

{
  "key": "Base64-encoded-pfx-content",
  "password": "password-value"
}
```
# <a name="c"></a>[<span data-ttu-id="7be16-147">C#</span><span class="sxs-lookup"><span data-stu-id="7be16-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadpkcs12-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7be16-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7be16-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadpkcs12-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7be16-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7be16-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadpkcs12-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7be16-150">Java</span><span class="sxs-lookup"><span data-stu-id="7be16-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/trustframeworkkeyset-uploadpkcs12-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7be16-151">响应</span><span class="sxs-lookup"><span data-stu-id="7be16-151">Response</span></span>

<span data-ttu-id="7be16-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7be16-152">The following is an example of the response.</span></span>

> <span data-ttu-id="7be16-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7be16-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "kty": "OCT",
    "nbf": 1508969811,
    "exp": 1508973711
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: uploadPkcs12",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


