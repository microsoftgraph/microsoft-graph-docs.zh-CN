---
title: 'trustFrameworkKeySet: uploadPkcs12'
description: 将 PKCS 12 格式密钥（PFX）上传到键集。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9cb1ff03d392032ae99117991b0c8ff356621476
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938191"
---
# <a name="trustframeworkkeyset-uploadpkcs12"></a><span data-ttu-id="416c1-103">trustFrameworkKeySet: uploadPkcs12</span><span class="sxs-lookup"><span data-stu-id="416c1-103">trustFrameworkKeySet: uploadPkcs12</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="416c1-104">将 PKCS12 格式密钥（PFX）上载到[trustFrameworkKeyset](../resources/trustframeworkkeyset.md)。</span><span class="sxs-lookup"><span data-stu-id="416c1-104">Upload a PKCS12 format key (PFX) to a [trustFrameworkKeyset](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="416c1-105">输入是 Pfx 证书内容的 base-64 编码值。</span><span class="sxs-lookup"><span data-stu-id="416c1-105">The input is a base-64 encoded value of the Pfx certificate contents.</span></span> <span data-ttu-id="416c1-106">此方法返回[trustFrameworkKey](../resources/trustframeworkkey.md)。</span><span class="sxs-lookup"><span data-stu-id="416c1-106">This method returns [trustFrameworkKey](../resources/trustframeworkkey.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="416c1-107">权限</span><span class="sxs-lookup"><span data-stu-id="416c1-107">Permissions</span></span>

<span data-ttu-id="416c1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="416c1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="416c1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="416c1-110">Permission type</span></span>                        | <span data-ttu-id="416c1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="416c1-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="416c1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="416c1-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="416c1-113">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="416c1-113">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="416c1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="416c1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="416c1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="416c1-115">Not supported.</span></span> |
| <span data-ttu-id="416c1-116">Application</span><span class="sxs-lookup"><span data-stu-id="416c1-116">Application</span></span>                            | <span data-ttu-id="416c1-117">TrustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="416c1-117">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="416c1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="416c1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/uploadPkcs12
```

## <a name="request-headers"></a><span data-ttu-id="416c1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="416c1-119">Request headers</span></span>

| <span data-ttu-id="416c1-120">名称</span><span class="sxs-lookup"><span data-stu-id="416c1-120">Name</span></span>          | <span data-ttu-id="416c1-121">说明</span><span class="sxs-lookup"><span data-stu-id="416c1-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="416c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="416c1-122">Authorization</span></span> | <span data-ttu-id="416c1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="416c1-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="416c1-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="416c1-125">Content-type</span></span>  | <span data-ttu-id="416c1-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="416c1-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="416c1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="416c1-128">Request body</span></span>

<span data-ttu-id="416c1-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="416c1-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="416c1-130">参数</span><span class="sxs-lookup"><span data-stu-id="416c1-130">Parameter</span></span>    | <span data-ttu-id="416c1-131">类型</span><span class="sxs-lookup"><span data-stu-id="416c1-131">Type</span></span>        | <span data-ttu-id="416c1-132">描述</span><span class="sxs-lookup"><span data-stu-id="416c1-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="416c1-133">Key</span><span class="sxs-lookup"><span data-stu-id="416c1-133">key</span></span>|<span data-ttu-id="416c1-134">字符串</span><span class="sxs-lookup"><span data-stu-id="416c1-134">String</span></span>|<span data-ttu-id="416c1-135">这是用于发送 pfx 内容的字段。</span><span class="sxs-lookup"><span data-stu-id="416c1-135">This is the field for sending pfx content.</span></span> <span data-ttu-id="416c1-136">该值应为实际证书内容的以64编码的版本。</span><span class="sxs-lookup"><span data-stu-id="416c1-136">The value should be a base-64 encoded version of the actual certificate content.</span></span>|
|<span data-ttu-id="416c1-137">密码</span><span class="sxs-lookup"><span data-stu-id="416c1-137">password</span></span>|<span data-ttu-id="416c1-138">String</span><span class="sxs-lookup"><span data-stu-id="416c1-138">String</span></span>|<span data-ttu-id="416c1-139">这是将密码发送给 PFX 内容的字段。</span><span class="sxs-lookup"><span data-stu-id="416c1-139">This is the field for sending the password to PFX content.</span></span>|

## <a name="response"></a><span data-ttu-id="416c1-140">响应</span><span class="sxs-lookup"><span data-stu-id="416c1-140">Response</span></span>

<span data-ttu-id="416c1-141">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[trustFrameworkKey](../resources/trustframeworkkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="416c1-141">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="416c1-142">示例</span><span class="sxs-lookup"><span data-stu-id="416c1-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="416c1-143">请求</span><span class="sxs-lookup"><span data-stu-id="416c1-143">Request</span></span>

<span data-ttu-id="416c1-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="416c1-144">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="416c1-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="416c1-145">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="416c1-146">C#</span><span class="sxs-lookup"><span data-stu-id="416c1-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/trustframeworkkeyset-uploadpkcs12-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="416c1-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="416c1-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/trustframeworkkeyset-uploadpkcs12-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="416c1-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="416c1-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/trustframeworkkeyset-uploadpkcs12-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="416c1-149">响应</span><span class="sxs-lookup"><span data-stu-id="416c1-149">Response</span></span>

<span data-ttu-id="416c1-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="416c1-150">The following is an example of the response.</span></span>

> <span data-ttu-id="416c1-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="416c1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
