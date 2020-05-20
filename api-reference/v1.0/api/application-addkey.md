---
title: 应用程序： addKey
description: 将密钥凭据添加到应用程序中。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 38f61f463e7071a168328781a8fbd4d990a5fdfd
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288695"
---
# <a name="application-addkey"></a><span data-ttu-id="1399a-103">应用程序： addKey</span><span class="sxs-lookup"><span data-stu-id="1399a-103">application: addKey</span></span>

<span data-ttu-id="1399a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1399a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1399a-105">将密钥凭据添加到[应用程序](../resources/application.md)中。</span><span class="sxs-lookup"><span data-stu-id="1399a-105">Add a key credential to an [application](../resources/application.md).</span></span> <span data-ttu-id="1399a-106">应用程序可以使用此方法和[removeKey](application-removekey.md)来自动滚动其过期密钥。</span><span class="sxs-lookup"><span data-stu-id="1399a-106">This method, along with [removeKey](application-removekey.md) can be used by an application to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="1399a-107">[创建应用程序](../api/application-post-applications.md)和[更新应用程序](../api/application-update.md)操作可继续用于添加和更新具有或不具有用户上下文的任何应用程序的密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="1399a-107">[Create application](../api/application-post-applications.md) and [Update application](../api/application-update.md) operations can continue to be used to add and update key credentials for any application with or without a user's context.</span></span>

<span data-ttu-id="1399a-108">作为此方法的请求验证的一部分，在可以执行操作之前，将验证已拥有现有密钥的证明。</span><span class="sxs-lookup"><span data-stu-id="1399a-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span> 

<span data-ttu-id="1399a-109">没有任何现有有效证书的应用程序（尚未添加任何证书，或所有证书已过期）将无法使用此服务操作。</span><span class="sxs-lookup"><span data-stu-id="1399a-109">Applications that don’t have any existing valid certificates (no certificates have been added yet, or all certificates have expired), won’t be able to use this service action.</span></span> <span data-ttu-id="1399a-110">可以使用[更新应用程序](../api/application-update.md)操作来改为执行更新。</span><span class="sxs-lookup"><span data-stu-id="1399a-110">You can use the [Update application](../api/application-update.md) operation to perform an update instead.</span></span>

## <a name="permissions"></a><span data-ttu-id="1399a-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="1399a-111">Permissions</span></span>

|<span data-ttu-id="1399a-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="1399a-112">Permission type</span></span>      | <span data-ttu-id="1399a-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1399a-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1399a-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1399a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1399a-115">无。</span><span class="sxs-lookup"><span data-stu-id="1399a-115">None.</span></span>  |
|<span data-ttu-id="1399a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1399a-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1399a-117">无。</span><span class="sxs-lookup"><span data-stu-id="1399a-117">None.</span></span>    |
|<span data-ttu-id="1399a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="1399a-118">Application</span></span> | <span data-ttu-id="1399a-119">无。</span><span class="sxs-lookup"><span data-stu-id="1399a-119">None.</span></span> |

> [!NOTE] 
> <span data-ttu-id="1399a-120">应用程序不需要任何特定权限即可滚动其自己的键。</span><span class="sxs-lookup"><span data-stu-id="1399a-120">An application does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="1399a-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1399a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/addKey
```

## <a name="request-headers"></a><span data-ttu-id="1399a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="1399a-122">Request headers</span></span>

| <span data-ttu-id="1399a-123">名称</span><span class="sxs-lookup"><span data-stu-id="1399a-123">Name</span></span>           | <span data-ttu-id="1399a-124">说明</span><span class="sxs-lookup"><span data-stu-id="1399a-124">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="1399a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1399a-125">Authorization</span></span>  | <span data-ttu-id="1399a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1399a-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1399a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1399a-128">Content-Type</span></span>   | <span data-ttu-id="1399a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1399a-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1399a-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="1399a-131">Request body</span></span>

<span data-ttu-id="1399a-132">在请求正文中，提供以下必需属性。</span><span class="sxs-lookup"><span data-stu-id="1399a-132">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="1399a-133">属性</span><span class="sxs-lookup"><span data-stu-id="1399a-133">Property</span></span>     | <span data-ttu-id="1399a-134">类型</span><span class="sxs-lookup"><span data-stu-id="1399a-134">Type</span></span>   |<span data-ttu-id="1399a-135">Description</span><span class="sxs-lookup"><span data-stu-id="1399a-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1399a-136">keyCredential</span><span class="sxs-lookup"><span data-stu-id="1399a-136">keyCredential</span></span> | [<span data-ttu-id="1399a-137">keyCredential</span><span class="sxs-lookup"><span data-stu-id="1399a-137">keyCredential</span></span>](../resources/keycredential.md) | <span data-ttu-id="1399a-138">要添加的新应用程序密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="1399a-138">The new application key credential to add.</span></span> <span data-ttu-id="1399a-139">__Type__、 __usage__和__key__是此用法的必需属性。</span><span class="sxs-lookup"><span data-stu-id="1399a-139">The __type__, __usage__ and __key__ are required properties for this usage.</span></span> <span data-ttu-id="1399a-140">受支持的密钥类型包括：</span><span class="sxs-lookup"><span data-stu-id="1399a-140">Supported key types are:</span></span><br><ul><li><span data-ttu-id="1399a-141">`AsymmetricX509Cert`：使用必须为 `Verify` 。</span><span class="sxs-lookup"><span data-stu-id="1399a-141">`AsymmetricX509Cert`: The usage must be `Verify`.</span></span></li><li><span data-ttu-id="1399a-142">`X509CertAndPassword`：使用必须`Sign`</span><span class="sxs-lookup"><span data-stu-id="1399a-142">`X509CertAndPassword`: The usage must be `Sign`</span></span></li></ul>|
| <span data-ttu-id="1399a-143">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="1399a-143">passwordCredential</span></span> | [<span data-ttu-id="1399a-144">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="1399a-144">passwordCredential</span></span>](../resources/passwordcredential.md) | <span data-ttu-id="1399a-145">仅需要设置应包含密钥密码的__secretText__ 。</span><span class="sxs-lookup"><span data-stu-id="1399a-145">Only __secretText__ is required to be set which should contain the password for the key.</span></span> <span data-ttu-id="1399a-146">仅对于类型的键，此属性是必需的 `X509CertAndPassword` 。</span><span class="sxs-lookup"><span data-stu-id="1399a-146">This property is required only for keys of type `X509CertAndPassword`.</span></span> <span data-ttu-id="1399a-147">将其设置为 `null` 其他。</span><span class="sxs-lookup"><span data-stu-id="1399a-147">Set it to `null` otherwise.</span></span>|
| <span data-ttu-id="1399a-148">证明</span><span class="sxs-lookup"><span data-stu-id="1399a-148">proof</span></span> | <span data-ttu-id="1399a-149">String</span><span class="sxs-lookup"><span data-stu-id="1399a-149">String</span></span> | <span data-ttu-id="1399a-150">自签名的 JWT 令牌，用作已有密钥的所有权证明。</span><span class="sxs-lookup"><span data-stu-id="1399a-150">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="1399a-151">必须使用应用程序的现有有效证书之一的私钥对此 JWT 令牌进行签名。</span><span class="sxs-lookup"><span data-stu-id="1399a-151">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="1399a-152">令牌应包含以下声明：</span><span class="sxs-lookup"><span data-stu-id="1399a-152">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="1399a-153">`aud`-需要访问群体 `00000002-0000-0000-c000-000000000000` 。</span><span class="sxs-lookup"><span data-stu-id="1399a-153">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="1399a-154">`iss`-颁发者必须是正在进行呼叫的应用程序的__id__ 。</span><span class="sxs-lookup"><span data-stu-id="1399a-154">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span></li><li><span data-ttu-id="1399a-155">`nbf`-不早时间。</span><span class="sxs-lookup"><span data-stu-id="1399a-155">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="1399a-156">`exp`-过期时间应为 "nbf" + 10 分钟。</span><span class="sxs-lookup"><span data-stu-id="1399a-156">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="1399a-157">下面是可用于生成此已占有令牌证明的代码[示例](/graph/application-rollkey-prooftoken)。</span><span class="sxs-lookup"><span data-stu-id="1399a-157">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="1399a-158">响应</span><span class="sxs-lookup"><span data-stu-id="1399a-158">Response</span></span>

<span data-ttu-id="1399a-159">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和新的[keyCredential](../resources/keycredential.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1399a-159">If successful, this method returns a `200 OK` response code and a new [keyCredential](../resources/keycredential.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1399a-160">示例</span><span class="sxs-lookup"><span data-stu-id="1399a-160">Examples</span></span>

### <a name="example-1-add-a-new-key-credential-to-an-application"></a><span data-ttu-id="1399a-161">示例1：将新的密钥凭据添加到应用程序</span><span class="sxs-lookup"><span data-stu-id="1399a-161">Example 1: Add a new key credential to an application</span></span>

#### <a name="request"></a><span data-ttu-id="1399a-162">请求</span><span class="sxs-lookup"><span data-stu-id="1399a-162">Request</span></span>

<span data-ttu-id="1399a-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1399a-163">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addKey
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

#### <a name="response"></a><span data-ttu-id="1399a-164">响应</span><span class="sxs-lookup"><span data-stu-id="1399a-164">Response</span></span>

<span data-ttu-id="1399a-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1399a-165">The following is an example of the response.</span></span>

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

### <a name="example-2-add-a-key-credential-and-an-associated-password-for-the-key"></a><span data-ttu-id="1399a-166">示例2：为密钥添加密钥凭据和关联密码</span><span class="sxs-lookup"><span data-stu-id="1399a-166">Example 2: Add a key credential and an associated password for the key</span></span>

#### <a name="request"></a><span data-ttu-id="1399a-167">请求</span><span class="sxs-lookup"><span data-stu-id="1399a-167">Request</span></span>

<span data-ttu-id="1399a-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1399a-168">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_addkey"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/addKey
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

#### <a name="response"></a><span data-ttu-id="1399a-169">响应</span><span class="sxs-lookup"><span data-stu-id="1399a-169">Response</span></span>

<span data-ttu-id="1399a-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1399a-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
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
  "description": "application: addKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: application_addkey:\r\n      Resource type was null or missing, so we assume there is no response to validate."
    ]
}-->
