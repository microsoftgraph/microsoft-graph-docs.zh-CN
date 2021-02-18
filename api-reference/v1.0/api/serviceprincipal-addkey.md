---
title: servicePrincipal： addKey
description: 向 servicePrincipal 添加密钥凭据。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ee7fa067e22ce072126c78385970919bf5fa1095
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292313"
---
# <a name="serviceprincipal-addkey"></a><span data-ttu-id="a01f2-103">servicePrincipal： addKey</span><span class="sxs-lookup"><span data-stu-id="a01f2-103">servicePrincipal: addKey</span></span>

<span data-ttu-id="a01f2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a01f2-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a01f2-105">向 [servicePrincipal 添加密钥凭据](../resources/serviceprincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="a01f2-105">Adds a key credential to a [servicePrincipal](../resources/serviceprincipal.md).</span></span> <span data-ttu-id="a01f2-106">servicePrincipal 可以使用 [此方法和 removeKey](serviceprincipal-removekey.md) 自动滚动即将过期的密钥。</span><span class="sxs-lookup"><span data-stu-id="a01f2-106">This method along with [removeKey](serviceprincipal-removekey.md) can be used by a servicePrincipal to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="a01f2-107">[创建 servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) 和更新 [servicePrincipal](../api/serviceprincipal-update.md) 操作可以继续用于添加和更新具有或不带用户上下文的任何 servicePrincipal 的关键凭据。</span><span class="sxs-lookup"><span data-stu-id="a01f2-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) and [Update servicePrincipal](../api/serviceprincipal-update.md) operations can continue to be used to add and update key credentials for any servicePrincipal with or without a user's context.</span></span>

<span data-ttu-id="a01f2-108">作为此方法的请求验证的一部分，先验证现有密钥的拥有证明，然后才能执行该操作。</span><span class="sxs-lookup"><span data-stu-id="a01f2-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span> 

<span data-ttu-id="a01f2-109">没有任何现有有效证书的 ServicePrincipals (即尚未添加任何证书，或者所有证书都已过期) ，将无法使用此服务操作。</span><span class="sxs-lookup"><span data-stu-id="a01f2-109">ServicePrincipals that don’t have any existing valid certificates (i.e.: no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="a01f2-110">[更新 servicePrincipal](../api/serviceprincipal-update.md) 可用于执行更新。</span><span class="sxs-lookup"><span data-stu-id="a01f2-110">[Update servicePrincipal](../api/serviceprincipal-update.md) can be used to perform an update instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="a01f2-111">权限</span><span class="sxs-lookup"><span data-stu-id="a01f2-111">Permissions</span></span>

|<span data-ttu-id="a01f2-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a01f2-112">Permission type</span></span>      | <span data-ttu-id="a01f2-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a01f2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a01f2-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a01f2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a01f2-115">无。</span><span class="sxs-lookup"><span data-stu-id="a01f2-115">None.</span></span>  |
|<span data-ttu-id="a01f2-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a01f2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a01f2-117">无。</span><span class="sxs-lookup"><span data-stu-id="a01f2-117">None.</span></span>    |
|<span data-ttu-id="a01f2-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a01f2-118">Application</span></span> | <span data-ttu-id="a01f2-119">无。</span><span class="sxs-lookup"><span data-stu-id="a01f2-119">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="a01f2-120">servicePrincipal 不需要任何特定权限来滚动自己的密钥。</span><span class="sxs-lookup"><span data-stu-id="a01f2-120">A servicePrincipal does not need any specific permission to roll it's own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="a01f2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a01f2-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/addKey
```

## <a name="request-headers"></a><span data-ttu-id="a01f2-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a01f2-122">Request headers</span></span>

| <span data-ttu-id="a01f2-123">名称</span><span class="sxs-lookup"><span data-stu-id="a01f2-123">Name</span></span>           | <span data-ttu-id="a01f2-124">说明</span><span class="sxs-lookup"><span data-stu-id="a01f2-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="a01f2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a01f2-125">Authorization</span></span>  | <span data-ttu-id="a01f2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a01f2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a01f2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a01f2-128">Content-Type</span></span>   | <span data-ttu-id="a01f2-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a01f2-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a01f2-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a01f2-131">Request body</span></span>

<span data-ttu-id="a01f2-132">在请求正文中，提供以下必需属性。</span><span class="sxs-lookup"><span data-stu-id="a01f2-132">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="a01f2-133">属性</span><span class="sxs-lookup"><span data-stu-id="a01f2-133">Property</span></span>     | <span data-ttu-id="a01f2-134">类型</span><span class="sxs-lookup"><span data-stu-id="a01f2-134">Type</span></span>   |<span data-ttu-id="a01f2-135">说明</span><span class="sxs-lookup"><span data-stu-id="a01f2-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a01f2-136">keyCredential</span><span class="sxs-lookup"><span data-stu-id="a01f2-136">keyCredential</span></span> | [<span data-ttu-id="a01f2-137">keyCredential</span><span class="sxs-lookup"><span data-stu-id="a01f2-137">keyCredential</span></span>](../resources/keycredential.md) | <span data-ttu-id="a01f2-138">要添加的新 servicePrincipal 密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="a01f2-138">The new servicePrincipal key credential to add.</span></span> <span data-ttu-id="a01f2-139">__类型____、用法____和密钥__ 是此用法的必需属性。</span><span class="sxs-lookup"><span data-stu-id="a01f2-139">The __type__, __usage__ and __key__ are required properties for this usage.</span></span> <span data-ttu-id="a01f2-140">受支持的密钥类型包括：</span><span class="sxs-lookup"><span data-stu-id="a01f2-140">Supported key types are:</span></span><br><ul><li><span data-ttu-id="a01f2-141">`AsymmetricX509Cert`：用法必须为 `Verify` 。</span><span class="sxs-lookup"><span data-stu-id="a01f2-141">`AsymmetricX509Cert`: The usage must be `Verify`.</span></span></li><li><span data-ttu-id="a01f2-142">`X509CertAndPassword`：用法必须为 `Sign`</span><span class="sxs-lookup"><span data-stu-id="a01f2-142">`X509CertAndPassword`: The usage must be `Sign`</span></span></li></ul>|
| <span data-ttu-id="a01f2-143">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="a01f2-143">passwordCredential</span></span> | [<span data-ttu-id="a01f2-144">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="a01f2-144">passwordCredential</span></span>](../resources/passwordcredential.md) | <span data-ttu-id="a01f2-145">只需设置应包含密钥密码的 __secretText。__</span><span class="sxs-lookup"><span data-stu-id="a01f2-145">Only __secretText__ is required to be set which should contain the password for the key.</span></span> <span data-ttu-id="a01f2-146">此属性仅对于类型键是必需的 `X509CertAndPassword` 。</span><span class="sxs-lookup"><span data-stu-id="a01f2-146">This property is required only for keys of type `X509CertAndPassword`.</span></span> <span data-ttu-id="a01f2-147">设置为 `null` 其他方式。</span><span class="sxs-lookup"><span data-stu-id="a01f2-147">Set it to `null` otherwise.</span></span>|
| <span data-ttu-id="a01f2-148">proof</span><span class="sxs-lookup"><span data-stu-id="a01f2-148">proof</span></span> | <span data-ttu-id="a01f2-149">String</span><span class="sxs-lookup"><span data-stu-id="a01f2-149">String</span></span> | <span data-ttu-id="a01f2-150">自签名 JWT 令牌，用于证明拥有现有密钥。</span><span class="sxs-lookup"><span data-stu-id="a01f2-150">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="a01f2-151">必须使用 servicePrincipal 的现有有效证书之一的私钥对此 JWT 令牌进行签名。</span><span class="sxs-lookup"><span data-stu-id="a01f2-151">This JWT token must be signed using the private key of one of the servicePrincipal's existing valid certificates.</span></span> <span data-ttu-id="a01f2-152">令牌应包含以下声明：</span><span class="sxs-lookup"><span data-stu-id="a01f2-152">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="a01f2-153">`aud` - 受众需要是 `00000002-0000-0000-c000-000000000000`。</span><span class="sxs-lookup"><span data-stu-id="a01f2-153">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="a01f2-154">`iss`- 颁发者需要是发出调用的 servicePrincipal 的 ID。</span><span class="sxs-lookup"><span data-stu-id="a01f2-154">`iss` - Issuer needs to be the __id__  of the servicePrincipal that is making the call.</span></span></li><li><span data-ttu-id="a01f2-155">`nbf` -“不早于”时间。</span><span class="sxs-lookup"><span data-stu-id="a01f2-155">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="a01f2-156">`exp` - 过期时间应该是“不早于”+ 10 分钟。</span><span class="sxs-lookup"><span data-stu-id="a01f2-156">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="a01f2-157">下面是可用于 [生成](/graph/application-rollkey-prooftoken) 此拥有令牌证明的代码示例。</span><span class="sxs-lookup"><span data-stu-id="a01f2-157">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|


## <a name="response"></a><span data-ttu-id="a01f2-158">响应</span><span class="sxs-lookup"><span data-stu-id="a01f2-158">Response</span></span>

<span data-ttu-id="a01f2-159">如果成功，此方法在响应正文中返回响应代码和新 `200 OK` [keyCredential](../resources/keycredential.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a01f2-159">If successful, this method returns a `200 OK` response code and a new [keyCredential](../resources/keycredential.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a01f2-160">示例</span><span class="sxs-lookup"><span data-stu-id="a01f2-160">Examples</span></span>

### <a name="example-1-adding-a-new-key-credential-to-a-serviceprincipal"></a><span data-ttu-id="a01f2-161">示例 1：向 servicePrincipal 添加新的密钥凭据</span><span class="sxs-lookup"><span data-stu-id="a01f2-161">Example 1: Adding a new key credential to a servicePrincipal</span></span>

#### <a name="request"></a><span data-ttu-id="a01f2-162">请求</span><span class="sxs-lookup"><span data-stu-id="a01f2-162">Request</span></span>

<span data-ttu-id="a01f2-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a01f2-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a01f2-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="a01f2-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "AsymmetricX509Cert",
        "usage": "Verify",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": null,
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[<span data-ttu-id="a01f2-165">C#</span><span class="sxs-lookup"><span data-stu-id="a01f2-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-addkey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a01f2-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a01f2-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-addkey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a01f2-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a01f2-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-addkey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a01f2-168">Java</span><span class="sxs-lookup"><span data-stu-id="a01f2-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-addkey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a01f2-169">响应</span><span class="sxs-lookup"><span data-stu-id="a01f2-169">Response</span></span>

<span data-ttu-id="a01f2-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a01f2-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-adding-a-key-credential-and-an-associated-password-for-the-key"></a><span data-ttu-id="a01f2-171">示例 2：为密钥添加密钥凭据和关联密码</span><span class="sxs-lookup"><span data-stu-id="a01f2-171">Example 2: Adding a key credential and an associated password for the key</span></span>

#### <a name="request"></a><span data-ttu-id="a01f2-172">请求</span><span class="sxs-lookup"><span data-stu-id="a01f2-172">Request</span></span>

<span data-ttu-id="a01f2-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a01f2-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_addkey"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/addKey
Content-type: application/json

{
    "keyCredential": {
        "type": "X509CertAndPassword",
        "usage": "Sign",
        "key": "MIIDYDCCAki..."
    },
    "passwordCredential": {
        "secretText": "MKTr0w1..."
    },
    "proof":"eyJ0eXAiOiJ..."
}
```

#### <a name="response"></a><span data-ttu-id="a01f2-174">响应</span><span class="sxs-lookup"><span data-stu-id="a01f2-174">Response</span></span>

<span data-ttu-id="a01f2-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a01f2-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.keyCredential"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

