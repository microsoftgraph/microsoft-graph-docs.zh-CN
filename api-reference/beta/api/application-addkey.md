---
title: application： addKey
description: 向应用程序添加密钥凭据。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8951e72c9135ed9d21141c7c5172adf06c31926d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942755"
---
# <a name="application-addkey"></a><span data-ttu-id="64c40-103">application： addKey</span><span class="sxs-lookup"><span data-stu-id="64c40-103">application: addKey</span></span>

<span data-ttu-id="64c40-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64c40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64c40-105">将密钥凭据添加到 [应用程序](../resources/application.md)。</span><span class="sxs-lookup"><span data-stu-id="64c40-105">Add a key credential to an [application](../resources/application.md).</span></span> <span data-ttu-id="64c40-106">此方法和 [removeKey](application-removekey.md)可用于应用程序自动滚动其过期密钥。</span><span class="sxs-lookup"><span data-stu-id="64c40-106">This method, along with [removeKey](application-removekey.md), can be used by an application to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="64c40-107">您可以继续使用"创建应用程序"[](../api/application-post-applications.md)和"更新[](../api/application-update.md)应用程序应用程序"操作来添加和更新具有或没有用户上下文的任何应用程序的密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="64c40-107">You can continue to use the [Create application](../api/application-post-applications.md) and [Update application](../api/application-update.md) application operations to add and update key credentials for any application with or without a user's context.</span></span> 

<span data-ttu-id="64c40-108">作为此方法的请求验证的一部分，将先验证现有密钥的证明，然后才能执行该操作。</span><span class="sxs-lookup"><span data-stu-id="64c40-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span> 

<span data-ttu-id="64c40-109">如果没有任何现有有效证书 (尚未添加任何证书，或者所有证书) ，将无法使用此服务操作。</span><span class="sxs-lookup"><span data-stu-id="64c40-109">Applications that don’t have any existing valid certificates (no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="64c40-110">可改用[更新应用程序](../api/application-update.md)操作来执行更新。</span><span class="sxs-lookup"><span data-stu-id="64c40-110">You can use the [Update application](../api/application-update.md) operation to perform an update instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="64c40-111">权限</span><span class="sxs-lookup"><span data-stu-id="64c40-111">Permissions</span></span>

|<span data-ttu-id="64c40-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="64c40-112">Permission type</span></span>      | <span data-ttu-id="64c40-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64c40-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64c40-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64c40-114">Delegated (work or school account)</span></span> | <span data-ttu-id="64c40-115">无。</span><span class="sxs-lookup"><span data-stu-id="64c40-115">None.</span></span>  |
|<span data-ttu-id="64c40-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64c40-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64c40-117">无。</span><span class="sxs-lookup"><span data-stu-id="64c40-117">None.</span></span>    |
|<span data-ttu-id="64c40-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="64c40-118">Application</span></span> | <span data-ttu-id="64c40-119">无。</span><span class="sxs-lookup"><span data-stu-id="64c40-119">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="64c40-120">应用程序不需要任何特定权限来滚动自己的密钥。</span><span class="sxs-lookup"><span data-stu-id="64c40-120">An application does not need any specific permission to roll its own keys.</span></span> 

## <a name="http-request"></a><span data-ttu-id="64c40-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64c40-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addKey
```

## <a name="request-headers"></a><span data-ttu-id="64c40-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="64c40-122">Request headers</span></span>

| <span data-ttu-id="64c40-123">名称</span><span class="sxs-lookup"><span data-stu-id="64c40-123">Name</span></span>           | <span data-ttu-id="64c40-124">说明</span><span class="sxs-lookup"><span data-stu-id="64c40-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="64c40-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="64c40-125">Authorization</span></span>  | <span data-ttu-id="64c40-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64c40-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="64c40-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="64c40-128">Content-Type</span></span>   | <span data-ttu-id="64c40-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="64c40-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64c40-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="64c40-131">Request body</span></span>

<span data-ttu-id="64c40-132">在请求正文中，提供以下必需属性。</span><span class="sxs-lookup"><span data-stu-id="64c40-132">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="64c40-133">属性</span><span class="sxs-lookup"><span data-stu-id="64c40-133">Property</span></span>     | <span data-ttu-id="64c40-134">类型</span><span class="sxs-lookup"><span data-stu-id="64c40-134">Type</span></span>   |<span data-ttu-id="64c40-135">说明</span><span class="sxs-lookup"><span data-stu-id="64c40-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="64c40-136">keyCredential</span><span class="sxs-lookup"><span data-stu-id="64c40-136">keyCredential</span></span> | [<span data-ttu-id="64c40-137">keyCredential</span><span class="sxs-lookup"><span data-stu-id="64c40-137">keyCredential</span></span>](../resources/keycredential.md) | <span data-ttu-id="64c40-138">要添加的新应用程序密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="64c40-138">The new application key credential to add.</span></span> <span data-ttu-id="64c40-139">__type、usage__ 和 __key__ 是此用法的必需属性。 </span><span class="sxs-lookup"><span data-stu-id="64c40-139">The __type__, __usage__ and __key__ are required properties for this usage.</span></span> <span data-ttu-id="64c40-140">受支持的密钥类型包括：</span><span class="sxs-lookup"><span data-stu-id="64c40-140">Supported key types are:</span></span><br><ul><li><span data-ttu-id="64c40-141">`AsymmetricX509Cert`：用法必须为 `Verify` 。</span><span class="sxs-lookup"><span data-stu-id="64c40-141">`AsymmetricX509Cert`: The usage must be `Verify`.</span></span></li><li><span data-ttu-id="64c40-142">`X509CertAndPassword`：用法必须为 `Sign`</span><span class="sxs-lookup"><span data-stu-id="64c40-142">`X509CertAndPassword`: The usage must be `Sign`</span></span></li></ul>|
| <span data-ttu-id="64c40-143">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="64c40-143">passwordCredential</span></span> | [<span data-ttu-id="64c40-144">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="64c40-144">passwordCredential</span></span>](../resources/passwordcredential.md) | <span data-ttu-id="64c40-145">仅需要设置应包含密钥密码的 __secretText。__</span><span class="sxs-lookup"><span data-stu-id="64c40-145">Only __secretText__ is required to be set which should contain the password for the key.</span></span> <span data-ttu-id="64c40-146">此属性仅对类型 为 的键是必需的 `X509CertAndPassword` 。</span><span class="sxs-lookup"><span data-stu-id="64c40-146">This property is required only for keys of type `X509CertAndPassword`.</span></span> <span data-ttu-id="64c40-147">否则， `null` 设置为 。</span><span class="sxs-lookup"><span data-stu-id="64c40-147">Set it to `null` otherwise.</span></span>|
| <span data-ttu-id="64c40-148">proof</span><span class="sxs-lookup"><span data-stu-id="64c40-148">proof</span></span> | <span data-ttu-id="64c40-149">String</span><span class="sxs-lookup"><span data-stu-id="64c40-149">String</span></span> | <span data-ttu-id="64c40-150">用作现有密钥拥有证明的自签名 JWT 令牌。</span><span class="sxs-lookup"><span data-stu-id="64c40-150">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="64c40-151">此 JWT 令牌必须使用应用程序现有有效证书之一的私钥进行签名。</span><span class="sxs-lookup"><span data-stu-id="64c40-151">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="64c40-152">令牌应包含以下声明：</span><span class="sxs-lookup"><span data-stu-id="64c40-152">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="64c40-153">`aud` - 受众需要是 `00000002-0000-0000-c000-000000000000`。</span><span class="sxs-lookup"><span data-stu-id="64c40-153">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="64c40-154">`iss` -颁发者必须是正在进行呼叫的应用程序的 __ID__。</span><span class="sxs-lookup"><span data-stu-id="64c40-154">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span></li><li><span data-ttu-id="64c40-155">`nbf` -“不早于”时间。</span><span class="sxs-lookup"><span data-stu-id="64c40-155">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="64c40-156">`exp` - 过期时间应该是“不早于”+ 10 分钟。</span><span class="sxs-lookup"><span data-stu-id="64c40-156">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="64c40-157">下面是可用于 [生成](/graph/application-rollkey-prooftoken) 此拥有令牌证明的代码示例。</span><span class="sxs-lookup"><span data-stu-id="64c40-157">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="64c40-158">响应</span><span class="sxs-lookup"><span data-stu-id="64c40-158">Response</span></span>

<span data-ttu-id="64c40-159">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和新 [keyCredential](../resources/keycredential.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64c40-159">If successful, this method returns a `200 OK` response code and a new [keyCredential](../resources/keycredential.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="64c40-160">示例</span><span class="sxs-lookup"><span data-stu-id="64c40-160">Examples</span></span>

### <a name="example-1-add-a-new-key-credential-to-an-application"></a><span data-ttu-id="64c40-161">示例 1：向应用程序添加新密钥凭据</span><span class="sxs-lookup"><span data-stu-id="64c40-161">Example 1: Add a new key credential to an application</span></span>

#### <a name="request"></a><span data-ttu-id="64c40-162">请求</span><span class="sxs-lookup"><span data-stu-id="64c40-162">Request</span></span>

<span data-ttu-id="64c40-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="64c40-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="64c40-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="64c40-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addkey_1"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/addKey
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
# <a name="c"></a>[<span data-ttu-id="64c40-165">C#</span><span class="sxs-lookup"><span data-stu-id="64c40-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addkey-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64c40-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64c40-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addkey-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64c40-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64c40-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addkey-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64c40-168">Java</span><span class="sxs-lookup"><span data-stu-id="64c40-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addkey-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="64c40-169">响应</span><span class="sxs-lookup"><span data-stu-id="64c40-169">Response</span></span>

<span data-ttu-id="64c40-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="64c40-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
}
```

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a><span data-ttu-id="64c40-171">示例 2：为密钥添加密钥凭据和关联密码</span><span class="sxs-lookup"><span data-stu-id="64c40-171">Example 2: Add a key credential and an associated password for the key</span></span>

#### <a name="request"></a><span data-ttu-id="64c40-172">请求</span><span class="sxs-lookup"><span data-stu-id="64c40-172">Request</span></span>

<span data-ttu-id="64c40-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="64c40-173">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="64c40-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="64c40-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addkey_2"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/addKey
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
# <a name="c"></a>[<span data-ttu-id="64c40-175">C#</span><span class="sxs-lookup"><span data-stu-id="64c40-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addkey-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64c40-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64c40-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addkey-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64c40-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64c40-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addkey-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64c40-178">Java</span><span class="sxs-lookup"><span data-stu-id="64c40-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addkey-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="64c40-179">响应</span><span class="sxs-lookup"><span data-stu-id="64c40-179">Response</span></span>

<span data-ttu-id="64c40-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="64c40-180">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.keyCredential"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.keyCredential"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->



