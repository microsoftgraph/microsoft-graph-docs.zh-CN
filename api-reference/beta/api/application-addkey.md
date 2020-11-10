---
title: 应用程序： addKey
description: 向应用程序添加密钥凭据。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 498e848d2adb8d3ccf14df2744c1ed5ec05be692
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962289"
---
# <a name="application-addkey"></a><span data-ttu-id="b4995-103">应用程序： addKey</span><span class="sxs-lookup"><span data-stu-id="b4995-103">application: addKey</span></span>

<span data-ttu-id="b4995-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4995-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4995-105">将密钥凭据添加到 [应用程序](../resources/application.md)中。</span><span class="sxs-lookup"><span data-stu-id="b4995-105">Add a key credential to an [application](../resources/application.md).</span></span> <span data-ttu-id="b4995-106">应用程序可以使用此方法和 [removeKey](application-removekey.md)来自动滚动其过期密钥。</span><span class="sxs-lookup"><span data-stu-id="b4995-106">This method, along with [removeKey](application-removekey.md), can be used by an application to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="b4995-107">您可以继续使用 [创建应用](../api/application-post-applications.md) 程序和 [更新应用](../api/application-update.md) 程序应用程序操作来添加和更新具有或不具有用户上下文的任何应用程序的密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="b4995-107">You can continue to use the [Create application](../api/application-post-applications.md) and [Update application](../api/application-update.md) application operations to add and update key credentials for any application with or without a user's context.</span></span> 

<span data-ttu-id="b4995-108">作为此方法的请求验证的一部分，在可以执行操作之前，将验证已拥有现有密钥的证明。</span><span class="sxs-lookup"><span data-stu-id="b4995-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span> 

<span data-ttu-id="b4995-109">如果应用程序没有任何现有的有效证书 (尚未添加任何证书，或者所有证书已过期) ，将无法使用此服务操作。</span><span class="sxs-lookup"><span data-stu-id="b4995-109">Applications that don’t have any existing valid certificates (no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="b4995-110">可改用[更新应用程序](../api/application-update.md)操作来执行更新。</span><span class="sxs-lookup"><span data-stu-id="b4995-110">You can use the [Update application](../api/application-update.md) operation to perform an update instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4995-111">权限</span><span class="sxs-lookup"><span data-stu-id="b4995-111">Permissions</span></span>

|<span data-ttu-id="b4995-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4995-112">Permission type</span></span>      | <span data-ttu-id="b4995-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4995-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4995-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4995-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b4995-115">无。</span><span class="sxs-lookup"><span data-stu-id="b4995-115">None.</span></span>  |
|<span data-ttu-id="b4995-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4995-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4995-117">无。</span><span class="sxs-lookup"><span data-stu-id="b4995-117">None.</span></span>    |
|<span data-ttu-id="b4995-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4995-118">Application</span></span> | <span data-ttu-id="b4995-119">无。</span><span class="sxs-lookup"><span data-stu-id="b4995-119">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="b4995-120">应用程序不需要任何特定权限即可滚动其自己的键。</span><span class="sxs-lookup"><span data-stu-id="b4995-120">An application does not need any specific permission to roll its own keys.</span></span> 

## <a name="http-request"></a><span data-ttu-id="b4995-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4995-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addKey
```

## <a name="request-headers"></a><span data-ttu-id="b4995-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4995-122">Request headers</span></span>

| <span data-ttu-id="b4995-123">名称</span><span class="sxs-lookup"><span data-stu-id="b4995-123">Name</span></span>           | <span data-ttu-id="b4995-124">说明</span><span class="sxs-lookup"><span data-stu-id="b4995-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b4995-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4995-125">Authorization</span></span>  | <span data-ttu-id="b4995-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4995-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b4995-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4995-128">Content-Type</span></span>   | <span data-ttu-id="b4995-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b4995-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4995-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4995-131">Request body</span></span>

<span data-ttu-id="b4995-132">在请求正文中，提供以下必需属性。</span><span class="sxs-lookup"><span data-stu-id="b4995-132">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="b4995-133">属性</span><span class="sxs-lookup"><span data-stu-id="b4995-133">Property</span></span>     | <span data-ttu-id="b4995-134">类型</span><span class="sxs-lookup"><span data-stu-id="b4995-134">Type</span></span>   |<span data-ttu-id="b4995-135">说明</span><span class="sxs-lookup"><span data-stu-id="b4995-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b4995-136">keyCredential</span><span class="sxs-lookup"><span data-stu-id="b4995-136">keyCredential</span></span> | [<span data-ttu-id="b4995-137">keyCredential</span><span class="sxs-lookup"><span data-stu-id="b4995-137">keyCredential</span></span>](../resources/keycredential.md) | <span data-ttu-id="b4995-138">要添加的新应用程序密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="b4995-138">The new application key credential to add.</span></span> <span data-ttu-id="b4995-139">__Type__ 、 __usage__ 和 __key__ 是此用法的必需属性。</span><span class="sxs-lookup"><span data-stu-id="b4995-139">The __type__ , __usage__ and __key__ are required properties for this usage.</span></span> <span data-ttu-id="b4995-140">受支持的密钥类型包括：</span><span class="sxs-lookup"><span data-stu-id="b4995-140">Supported key types are:</span></span><br><ul><li><span data-ttu-id="b4995-141">`AsymmetricX509Cert`：使用必须为 `Verify` 。</span><span class="sxs-lookup"><span data-stu-id="b4995-141">`AsymmetricX509Cert`: The usage must be `Verify`.</span></span></li><li><span data-ttu-id="b4995-142">`X509CertAndPassword`：使用必须 `Sign`</span><span class="sxs-lookup"><span data-stu-id="b4995-142">`X509CertAndPassword`: The usage must be `Sign`</span></span></li></ul>|
| <span data-ttu-id="b4995-143">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="b4995-143">passwordCredential</span></span> | [<span data-ttu-id="b4995-144">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="b4995-144">passwordCredential</span></span>](../resources/passwordcredential.md) | <span data-ttu-id="b4995-145">仅需要设置应包含密钥密码的 __secretText__ 。</span><span class="sxs-lookup"><span data-stu-id="b4995-145">Only __secretText__ is required to be set which should contain the password for the key.</span></span> <span data-ttu-id="b4995-146">仅对于类型的键，此属性是必需的 `X509CertAndPassword` 。</span><span class="sxs-lookup"><span data-stu-id="b4995-146">This property is required only for keys of type `X509CertAndPassword`.</span></span> <span data-ttu-id="b4995-147">将其设置为 `null` 其他。</span><span class="sxs-lookup"><span data-stu-id="b4995-147">Set it to `null` otherwise.</span></span>|
| <span data-ttu-id="b4995-148">证明</span><span class="sxs-lookup"><span data-stu-id="b4995-148">proof</span></span> | <span data-ttu-id="b4995-149">String</span><span class="sxs-lookup"><span data-stu-id="b4995-149">String</span></span> | <span data-ttu-id="b4995-150">自签名的 JWT 令牌，用作已有密钥的所有权证明。</span><span class="sxs-lookup"><span data-stu-id="b4995-150">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="b4995-151">此 JWT 令牌必须使用应用程序现有有效证书之一的私钥进行签名。</span><span class="sxs-lookup"><span data-stu-id="b4995-151">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="b4995-152">令牌应包含以下声明：</span><span class="sxs-lookup"><span data-stu-id="b4995-152">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="b4995-153">`aud` - 受众需要是 `00000002-0000-0000-c000-000000000000`。</span><span class="sxs-lookup"><span data-stu-id="b4995-153">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="b4995-154">`iss` -颁发者必须是正在进行呼叫的应用程序的 __ID__ 。</span><span class="sxs-lookup"><span data-stu-id="b4995-154">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span></li><li><span data-ttu-id="b4995-155">`nbf` -“不早于”时间。</span><span class="sxs-lookup"><span data-stu-id="b4995-155">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="b4995-156">`exp` - 过期时间应该是“不早于”+ 10 分钟。</span><span class="sxs-lookup"><span data-stu-id="b4995-156">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="b4995-157">下面是可用于生成此已占有令牌证明的代码 [示例](/graph/application-rollkey-prooftoken) 。</span><span class="sxs-lookup"><span data-stu-id="b4995-157">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="b4995-158">响应</span><span class="sxs-lookup"><span data-stu-id="b4995-158">Response</span></span>

<span data-ttu-id="b4995-159">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和新的 [keyCredential](../resources/keycredential.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b4995-159">If successful, this method returns a `200 OK` response code and a new [keyCredential](../resources/keycredential.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b4995-160">示例</span><span class="sxs-lookup"><span data-stu-id="b4995-160">Examples</span></span>

### <a name="example-1-add-a-new-key-credential-to-an-application"></a><span data-ttu-id="b4995-161">示例1：将新的密钥凭据添加到应用程序</span><span class="sxs-lookup"><span data-stu-id="b4995-161">Example 1: Add a new key credential to an application</span></span>

#### <a name="request"></a><span data-ttu-id="b4995-162">请求</span><span class="sxs-lookup"><span data-stu-id="b4995-162">Request</span></span>

<span data-ttu-id="b4995-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b4995-163">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b4995-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4995-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_addkey"
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
# <a name="c"></a>[<span data-ttu-id="b4995-165">C#</span><span class="sxs-lookup"><span data-stu-id="b4995-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-addkey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4995-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4995-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-addkey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4995-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4995-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-addkey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4995-168">Java</span><span class="sxs-lookup"><span data-stu-id="b4995-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-addkey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b4995-169">响应</span><span class="sxs-lookup"><span data-stu-id="b4995-169">Response</span></span>

<span data-ttu-id="b4995-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b4995-170">The following is an example of the response.</span></span>

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

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a><span data-ttu-id="b4995-171">示例2：为密钥添加密钥凭据和关联密码</span><span class="sxs-lookup"><span data-stu-id="b4995-171">Example 2: Add a key credential and an associated password for the key</span></span>

#### <a name="request"></a><span data-ttu-id="b4995-172">请求</span><span class="sxs-lookup"><span data-stu-id="b4995-172">Request</span></span>

<span data-ttu-id="b4995-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b4995-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_addkey"
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

#### <a name="response"></a><span data-ttu-id="b4995-174">响应</span><span class="sxs-lookup"><span data-stu-id="b4995-174">Response</span></span>

<span data-ttu-id="b4995-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b4995-175">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
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
    "Error: application_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->


