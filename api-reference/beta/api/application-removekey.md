---
title: application： removeKey
description: 从应用程序中删除密钥凭据
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: a02d731866ef831d3e2e2208a4a0ee9f535e1ed8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129049"
---
# <a name="application-removekey"></a><span data-ttu-id="04956-103">application： removeKey</span><span class="sxs-lookup"><span data-stu-id="04956-103">application: removeKey</span></span>

<span data-ttu-id="04956-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04956-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04956-105">从应用程序中删除密钥 [凭据](../resources/application.md)。</span><span class="sxs-lookup"><span data-stu-id="04956-105">Remove a key credential from an [application](../resources/application.md).</span></span> <span data-ttu-id="04956-106">此方法和 [addKey](application-addkey.md) 可用于应用程序自动滚动其过期密钥。</span><span class="sxs-lookup"><span data-stu-id="04956-106">This method along with [addKey](application-addkey.md) can be used by an application to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="04956-107">[创建 servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) 和更新 [servicePrincipal](../api/serviceprincipal-update.md) 操作可以继续用于为具有应用程序或用户上下文的任何应用程序添加和更新密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="04956-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) and [Update servicePrincipal](../api/serviceprincipal-update.md) operations can continue to be used to add and update key credentials for any application with application or a user's context.</span></span>

<span data-ttu-id="04956-108">作为此方法的请求验证的一部分，先验证现有密钥的拥有证明，然后才能执行该操作。</span><span class="sxs-lookup"><span data-stu-id="04956-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span>

## <a name="permissions"></a><span data-ttu-id="04956-109">权限</span><span class="sxs-lookup"><span data-stu-id="04956-109">Permissions</span></span>

|<span data-ttu-id="04956-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="04956-110">Permission type</span></span>      | <span data-ttu-id="04956-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04956-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04956-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04956-112">Delegated (work or school account)</span></span> | <span data-ttu-id="04956-113">无。</span><span class="sxs-lookup"><span data-stu-id="04956-113">None.</span></span>  |
|<span data-ttu-id="04956-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04956-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04956-115">无。</span><span class="sxs-lookup"><span data-stu-id="04956-115">None.</span></span>    |
|<span data-ttu-id="04956-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="04956-116">Application</span></span> | <span data-ttu-id="04956-117">无。</span><span class="sxs-lookup"><span data-stu-id="04956-117">None.</span></span> |

> [!NOTE] 
> <span data-ttu-id="04956-118">应用程序不需要任何特定权限来滚动自己的密钥。</span><span class="sxs-lookup"><span data-stu-id="04956-118">An application does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="04956-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04956-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removeKey
```

## <a name="request-headers"></a><span data-ttu-id="04956-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="04956-120">Request headers</span></span>

| <span data-ttu-id="04956-121">名称</span><span class="sxs-lookup"><span data-stu-id="04956-121">Name</span></span>           | <span data-ttu-id="04956-122">说明</span><span class="sxs-lookup"><span data-stu-id="04956-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="04956-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04956-123">Authorization</span></span>  | <span data-ttu-id="04956-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="04956-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="04956-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04956-126">Content-Type</span></span>   | <span data-ttu-id="04956-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="04956-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="04956-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="04956-129">Request body</span></span>

<span data-ttu-id="04956-130">在请求正文中，提供以下必需属性。</span><span class="sxs-lookup"><span data-stu-id="04956-130">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="04956-131">属性</span><span class="sxs-lookup"><span data-stu-id="04956-131">Property</span></span>  | <span data-ttu-id="04956-132">类型</span><span class="sxs-lookup"><span data-stu-id="04956-132">Type</span></span> | <span data-ttu-id="04956-133">说明</span><span class="sxs-lookup"><span data-stu-id="04956-133">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="04956-134">keyId</span><span class="sxs-lookup"><span data-stu-id="04956-134">keyId</span></span>     | <span data-ttu-id="04956-135">GUID</span><span class="sxs-lookup"><span data-stu-id="04956-135">GUID</span></span> | <span data-ttu-id="04956-136">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="04956-136">The unique identifier for the password.</span></span>|
| <span data-ttu-id="04956-137">proof</span><span class="sxs-lookup"><span data-stu-id="04956-137">proof</span></span> | <span data-ttu-id="04956-138">字符串</span><span class="sxs-lookup"><span data-stu-id="04956-138">String</span></span> | <span data-ttu-id="04956-139">自签名 JWT 令牌，用作现有密钥的拥有证明。</span><span class="sxs-lookup"><span data-stu-id="04956-139">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="04956-140">此 JWT 令牌必须使用应用程序现有有效证书之一的私钥进行签名。</span><span class="sxs-lookup"><span data-stu-id="04956-140">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="04956-141">令牌应包含以下声明：</span><span class="sxs-lookup"><span data-stu-id="04956-141">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="04956-142">`aud` - 受众需要是 `00000002-0000-0000-c000-000000000000`。</span><span class="sxs-lookup"><span data-stu-id="04956-142">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="04956-143">`iss` -颁发者必须是正在进行呼叫的应用程序的 __ID__。</span><span class="sxs-lookup"><span data-stu-id="04956-143">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span></li><li><span data-ttu-id="04956-144">`nbf` -“不早于”时间。</span><span class="sxs-lookup"><span data-stu-id="04956-144">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="04956-145">`exp` - 过期时间应该是“不早于”+ 10 分钟。</span><span class="sxs-lookup"><span data-stu-id="04956-145">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="04956-146">下面是可用于 [生成](/graph/application-rollkey-prooftoken) 此拥有令牌证明的代码示例。</span><span class="sxs-lookup"><span data-stu-id="04956-146">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="04956-147">响应</span><span class="sxs-lookup"><span data-stu-id="04956-147">Response</span></span>

<span data-ttu-id="04956-148">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="04956-148">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="04956-149">示例</span><span class="sxs-lookup"><span data-stu-id="04956-149">Examples</span></span>

<span data-ttu-id="04956-150">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="04956-150">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="04956-151">请求</span><span class="sxs-lookup"><span data-stu-id="04956-151">Request</span></span>

<span data-ttu-id="04956-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="04956-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="04956-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="04956-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_removekey"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="c"></a>[<span data-ttu-id="04956-154">C#</span><span class="sxs-lookup"><span data-stu-id="04956-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/application-removekey-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04956-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04956-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-removekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04956-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04956-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-removekey-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04956-157">Java</span><span class="sxs-lookup"><span data-stu-id="04956-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/application-removekey-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="04956-158">响应</span><span class="sxs-lookup"><span data-stu-id="04956-158">Response</span></span>

<span data-ttu-id="04956-159">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="04956-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: removeKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



