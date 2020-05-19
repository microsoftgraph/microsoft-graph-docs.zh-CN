---
title: 应用程序： removeKey
description: 从应用程序中删除密钥凭据
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2395d2372b70d6ed3150c8186803d3d3226acaba
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289158"
---
# <a name="application-removekey"></a><span data-ttu-id="61cae-103">应用程序： removeKey</span><span class="sxs-lookup"><span data-stu-id="61cae-103">application: removeKey</span></span>

<span data-ttu-id="61cae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61cae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61cae-105">从[应用程序](../resources/application.md)中删除密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="61cae-105">Remove a key credential from an [application](../resources/application.md).</span></span> <span data-ttu-id="61cae-106">应用程序可以使用此方法和[addKey](application-addkey.md)自动滚动其过期密钥。</span><span class="sxs-lookup"><span data-stu-id="61cae-106">This method along with [addKey](application-addkey.md) can be used by an application to automate rolling its expiring keys.</span></span>

> [!NOTE]
> <span data-ttu-id="61cae-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) And [update servicePrincipal](../api/serviceprincipal-update.md)操作可继续用于添加和更新应用程序或用户上下文的任何应用程序的密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="61cae-107">[Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) and [Update servicePrincipal](../api/serviceprincipal-update.md) operations can continue to be used to add and update key credentials for any application with application or a user's context.</span></span>

<span data-ttu-id="61cae-108">作为此方法的请求验证的一部分，在可以执行操作之前，将验证已拥有现有密钥的证明。</span><span class="sxs-lookup"><span data-stu-id="61cae-108">As part of the request validation for this method, a proof of possession of an existing key is verified before the action can be performed.</span></span>

## <a name="permissions"></a><span data-ttu-id="61cae-109">权限</span><span class="sxs-lookup"><span data-stu-id="61cae-109">Permissions</span></span>

|<span data-ttu-id="61cae-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="61cae-110">Permission type</span></span>      | <span data-ttu-id="61cae-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61cae-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="61cae-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61cae-112">Delegated (work or school account)</span></span> | <span data-ttu-id="61cae-113">无。</span><span class="sxs-lookup"><span data-stu-id="61cae-113">None.</span></span>  |
|<span data-ttu-id="61cae-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61cae-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61cae-115">无。</span><span class="sxs-lookup"><span data-stu-id="61cae-115">None.</span></span>    |
|<span data-ttu-id="61cae-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="61cae-116">Application</span></span> | <span data-ttu-id="61cae-117">无。</span><span class="sxs-lookup"><span data-stu-id="61cae-117">None.</span></span> |

> [!NOTE] 
> <span data-ttu-id="61cae-118">应用程序不需要任何特定权限即可滚动其自己的键。</span><span class="sxs-lookup"><span data-stu-id="61cae-118">An application does not need any specific permission to roll its own keys.</span></span>

## <a name="http-request"></a><span data-ttu-id="61cae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61cae-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/removeKey
```

## <a name="request-headers"></a><span data-ttu-id="61cae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="61cae-120">Request headers</span></span>

| <span data-ttu-id="61cae-121">名称</span><span class="sxs-lookup"><span data-stu-id="61cae-121">Name</span></span>           | <span data-ttu-id="61cae-122">说明</span><span class="sxs-lookup"><span data-stu-id="61cae-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="61cae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="61cae-123">Authorization</span></span>  | <span data-ttu-id="61cae-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="61cae-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="61cae-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61cae-126">Content-Type</span></span>   | <span data-ttu-id="61cae-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="61cae-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61cae-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="61cae-129">Request body</span></span>

<span data-ttu-id="61cae-130">在请求正文中，提供以下必需属性。</span><span class="sxs-lookup"><span data-stu-id="61cae-130">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="61cae-131">属性</span><span class="sxs-lookup"><span data-stu-id="61cae-131">Property</span></span>  | <span data-ttu-id="61cae-132">类型</span><span class="sxs-lookup"><span data-stu-id="61cae-132">Type</span></span> | <span data-ttu-id="61cae-133">说明</span><span class="sxs-lookup"><span data-stu-id="61cae-133">Description</span></span>|
|:----------|:-----|:-----------|
| <span data-ttu-id="61cae-134">keyId</span><span class="sxs-lookup"><span data-stu-id="61cae-134">keyId</span></span>     | <span data-ttu-id="61cae-135">GUID</span><span class="sxs-lookup"><span data-stu-id="61cae-135">GUID</span></span> | <span data-ttu-id="61cae-136">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="61cae-136">The unique identifier for the password.</span></span>|
| <span data-ttu-id="61cae-137">证明</span><span class="sxs-lookup"><span data-stu-id="61cae-137">proof</span></span> | <span data-ttu-id="61cae-138">String</span><span class="sxs-lookup"><span data-stu-id="61cae-138">String</span></span> | <span data-ttu-id="61cae-139">自签名的 JWT 令牌，用作已有密钥的所有权证明。</span><span class="sxs-lookup"><span data-stu-id="61cae-139">A self-signed JWT token used as a proof of possession of the existing keys.</span></span> <span data-ttu-id="61cae-140">必须使用应用程序的现有有效证书之一的私钥对此 JWT 令牌进行签名。</span><span class="sxs-lookup"><span data-stu-id="61cae-140">This JWT token must be signed using the private key of one of the application's existing valid certificates.</span></span> <span data-ttu-id="61cae-141">令牌应包含以下声明：</span><span class="sxs-lookup"><span data-stu-id="61cae-141">The token should contain the following claims:</span></span><ul><li><span data-ttu-id="61cae-142">`aud`-需要访问群体 `00000002-0000-0000-c000-000000000000` 。</span><span class="sxs-lookup"><span data-stu-id="61cae-142">`aud` - Audience needs to be `00000002-0000-0000-c000-000000000000`.</span></span></li><li><span data-ttu-id="61cae-143">`iss`-颁发者必须是正在进行呼叫的应用程序的__id__ 。</span><span class="sxs-lookup"><span data-stu-id="61cae-143">`iss` - Issuer needs to be the __id__  of the application that is making the call.</span></span></li><li><span data-ttu-id="61cae-144">`nbf`-不早时间。</span><span class="sxs-lookup"><span data-stu-id="61cae-144">`nbf` - Not before time.</span></span></li><li><span data-ttu-id="61cae-145">`exp`-过期时间应为 "nbf" + 10 分钟。</span><span class="sxs-lookup"><span data-stu-id="61cae-145">`exp` - Expiration time should be "nbf" + 10 mins.</span></span></li></ul><br><span data-ttu-id="61cae-146">下面是可用于生成此已占有令牌证明的代码[示例](/graph/application-rollkey-prooftoken)。</span><span class="sxs-lookup"><span data-stu-id="61cae-146">Here is a code [sample](/graph/application-rollkey-prooftoken) that can be used to generate this proof of possession token.</span></span>|

## <a name="response"></a><span data-ttu-id="61cae-147">响应</span><span class="sxs-lookup"><span data-stu-id="61cae-147">Response</span></span>

<span data-ttu-id="61cae-148">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="61cae-148">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="61cae-149">示例</span><span class="sxs-lookup"><span data-stu-id="61cae-149">Examples</span></span>

<span data-ttu-id="61cae-150">下面的示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="61cae-150">The following is example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="61cae-151">请求</span><span class="sxs-lookup"><span data-stu-id="61cae-151">Request</span></span>

<span data-ttu-id="61cae-152">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="61cae-152">The following is an example of the request.</span></span>

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

### <a name="response"></a><span data-ttu-id="61cae-153">响应</span><span class="sxs-lookup"><span data-stu-id="61cae-153">Response</span></span>

<span data-ttu-id="61cae-154">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="61cae-154">The following is an example of the response.</span></span>

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