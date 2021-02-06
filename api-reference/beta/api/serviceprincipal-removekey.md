---
title: servicePrincipal： removeKey
description: 从 servicePrincipal 中删除密钥凭据
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: f82140ff1710d9da7c646d2b84f1d83ac4a66150
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134146"
---
# <a name="serviceprincipal-removekey"></a><span data-ttu-id="b2866-103">servicePrincipal： removeKey</span><span class="sxs-lookup"><span data-stu-id="b2866-103">servicePrincipal: removeKey</span></span>

<span data-ttu-id="b2866-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2866-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2866-105">从 [servicePrincipal 中删除密钥凭据](../resources/serviceprincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="b2866-105">Remove a key credential from a [servicePrincipal](../resources/serviceprincipal.md).</span></span> <span data-ttu-id="b2866-106">servicePrincipal 可以使用此方法 [和 addKey](serviceprincipal-addkey.md) 自动滚动即将过期的密钥。</span><span class="sxs-lookup"><span data-stu-id="b2866-106">This method along with [addKey](serviceprincipal-addkey.md) can be used by a servicePrincipal to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="b2866-107">[创建 servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) 和更新 [servicePrincipal](../api/serviceprincipal-update.md) 操作可以继续用于添加和更新具有或不带用户上下文的任何 servicePrincipal 的密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="b2866-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) and [Update servicePrincipal](../api/serviceprincipal-update.md) operations can continue to be used to add and update key credentials for any servicePrincipal with or without a user's context.</span></span>

<span data-ttu-id="b2866-108">作为此方法的请求验证的一部分，先验证现有密钥的拥有证明，然后才能执行该操作。</span><span class="sxs-lookup"><span data-stu-id="b2866-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2866-109">权限</span><span class="sxs-lookup"><span data-stu-id="b2866-109">Permissions</span></span>

|<span data-ttu-id="b2866-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2866-110">Permission type</span></span>      | <span data-ttu-id="b2866-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2866-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2866-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2866-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b2866-113">无。</span><span class="sxs-lookup"><span data-stu-id="b2866-113">None.</span></span>  |
|<span data-ttu-id="b2866-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2866-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2866-115">无。</span><span class="sxs-lookup"><span data-stu-id="b2866-115">None.</span></span>    |
|<span data-ttu-id="b2866-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2866-116">Application</span></span> | <span data-ttu-id="b2866-117">无。</span><span class="sxs-lookup"><span data-stu-id="b2866-117">None.</span></span> |

> [!NOTE]
> <span data-ttu-id="b2866-118">servicePrincipal 不需要任何特定权限来滚动自己的密钥。</span><span class="sxs-lookup"><span data-stu-id="b2866-118">A servicePrincipal does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="b2866-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2866-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /serviceprincipals/{id}/removeKey
```

## <a name="request-headers"></a><span data-ttu-id="b2866-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2866-120">Request headers</span></span>

| <span data-ttu-id="b2866-121">名称</span><span class="sxs-lookup"><span data-stu-id="b2866-121">Name</span></span>           | <span data-ttu-id="b2866-122">说明</span><span class="sxs-lookup"><span data-stu-id="b2866-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b2866-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2866-123">Authorization</span></span>  | <span data-ttu-id="b2866-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2866-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b2866-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b2866-126">Content-Type</span></span>   | <span data-ttu-id="b2866-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b2866-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2866-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2866-129">Request body</span></span>

<span data-ttu-id="b2866-130">在请求正文中，提供以下必需属性。</span><span class="sxs-lookup"><span data-stu-id="b2866-130">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="b2866-131">属性</span><span class="sxs-lookup"><span data-stu-id="b2866-131">Property</span></span>  | <span data-ttu-id="b2866-132">类型</span><span class="sxs-lookup"><span data-stu-id="b2866-132">Type</span></span> | <span data-ttu-id="b2866-133">说明</span><span class="sxs-lookup"><span data-stu-id="b2866-133">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="b2866-134">keyId</span><span class="sxs-lookup"><span data-stu-id="b2866-134">keyId</span></span>     | <span data-ttu-id="b2866-135">GUID</span><span class="sxs-lookup"><span data-stu-id="b2866-135">GUID</span></span> | <span data-ttu-id="b2866-136">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b2866-136">The unique identifier for the password.</span></span>|
| <span data-ttu-id="b2866-137">proof</span><span class="sxs-lookup"><span data-stu-id="b2866-137">proof</span></span> | <span data-ttu-id="b2866-138">字符串</span><span class="sxs-lookup"><span data-stu-id="b2866-138">String</span></span> | <span data-ttu-id="b2866-139">自签名 JWT 令牌，用作现有密钥的拥有证明。</span><span class="sxs-lookup"><span data-stu-id="b2866-139">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="b2866-140">必须使用 servicePrincipal 的现有有效证书之一的私钥对此 JWT 令牌进行签名。</span><span class="sxs-lookup"><span data-stu-id="b2866-140">This JWT token must be signed using the private key of one of the servicePrincipal's existing valid certificates.</span></span> <span data-ttu-id="b2866-141">令牌应包含以下声明：</span><span class="sxs-lookup"><span data-stu-id="b2866-141">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="b2866-142">`aud` - 受众需要是 `00000002-0000-0000-c000-000000000000`。</span><span class="sxs-lookup"><span data-stu-id="b2866-142">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="b2866-143">`iss`- 颁发者需要是发出调用的 servicePrincipal 的 ID。</span><span class="sxs-lookup"><span data-stu-id="b2866-143">`iss` - Issuer needs to be the __id__  of the servicePrincipal that is making the call.</span></span></li><li><span data-ttu-id="b2866-144">`nbf` -“不早于”时间。</span><span class="sxs-lookup"><span data-stu-id="b2866-144">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="b2866-145">`exp` - 过期时间应该是“不早于”+ 10 分钟。</span><span class="sxs-lookup"><span data-stu-id="b2866-145">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="b2866-146">下面是可用于 [生成](/graph/application-rollkey-prooftoken) 此拥有令牌证明的代码示例。</span><span class="sxs-lookup"><span data-stu-id="b2866-146">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="b2866-147">响应</span><span class="sxs-lookup"><span data-stu-id="b2866-147">Response</span></span>

<span data-ttu-id="b2866-148">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b2866-148">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b2866-149">示例</span><span class="sxs-lookup"><span data-stu-id="b2866-149">Examples</span></span>

<span data-ttu-id="b2866-150">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b2866-150">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b2866-151">请求</span><span class="sxs-lookup"><span data-stu-id="b2866-151">Request</span></span>

<span data-ttu-id="b2866-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b2866-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b2866-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="b2866-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_removekey"
}-->

```http
POST https://graph.microsoft.com/beta/serviceprincipals/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
}
```
# <a name="javascript"></a>[<span data-ttu-id="b2866-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b2866-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removekey-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b2866-155">响应</span><span class="sxs-lookup"><span data-stu-id="b2866-155">Response</span></span>

<span data-ttu-id="b2866-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b2866-156">The following is an example of the response.</span></span>

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
  "description": "servicePrincipal: removeKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



