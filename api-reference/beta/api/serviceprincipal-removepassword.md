---
title: servicePrincipal： removePassword
description: 从 servicePrincipal 中删除密码
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f32642e87602545720574b60db42cdf3993079f5
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997644"
---
# <a name="serviceprincipal-removepassword"></a><span data-ttu-id="afe7c-103">servicePrincipal： removePassword</span><span class="sxs-lookup"><span data-stu-id="afe7c-103">servicePrincipal: removePassword</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afe7c-104">从[servicePrincipal](../resources/serviceprincipal.md)对象中删除密码。</span><span class="sxs-lookup"><span data-stu-id="afe7c-104">Remove a password from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="afe7c-105">权限</span><span class="sxs-lookup"><span data-stu-id="afe7c-105">Permissions</span></span>

<span data-ttu-id="afe7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afe7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="afe7c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="afe7c-108">Permission type</span></span>                        | <span data-ttu-id="afe7c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="afe7c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="afe7c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afe7c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="afe7c-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="afe7c-111">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="afe7c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afe7c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afe7c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="afe7c-113">Not supported.</span></span> |
| <span data-ttu-id="afe7c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="afe7c-114">Application</span></span>                            | <span data-ttu-id="afe7c-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="afe7c-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="afe7c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afe7c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="afe7c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="afe7c-117">Request headers</span></span>

| <span data-ttu-id="afe7c-118">名称</span><span class="sxs-lookup"><span data-stu-id="afe7c-118">Name</span></span>           | <span data-ttu-id="afe7c-119">说明</span><span class="sxs-lookup"><span data-stu-id="afe7c-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="afe7c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="afe7c-120">Authorization</span></span>  | <span data-ttu-id="afe7c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="afe7c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="afe7c-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="afe7c-123">Content-type</span></span>   | <span data-ttu-id="afe7c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="afe7c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="afe7c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="afe7c-126">Request body</span></span>

| <span data-ttu-id="afe7c-127">属性</span><span class="sxs-lookup"><span data-stu-id="afe7c-127">Property</span></span>     | <span data-ttu-id="afe7c-128">类型</span><span class="sxs-lookup"><span data-stu-id="afe7c-128">Type</span></span>   |<span data-ttu-id="afe7c-129">说明</span><span class="sxs-lookup"><span data-stu-id="afe7c-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="afe7c-130">keyId</span><span class="sxs-lookup"><span data-stu-id="afe7c-130">keyId</span></span> | <span data-ttu-id="afe7c-131">GUID</span><span class="sxs-lookup"><span data-stu-id="afe7c-131">GUID</span></span> | <span data-ttu-id="afe7c-132">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="afe7c-132">The unique identifier for the password.</span></span> <span data-ttu-id="afe7c-133">必需。</span><span class="sxs-lookup"><span data-stu-id="afe7c-133">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="afe7c-134">响应</span><span class="sxs-lookup"><span data-stu-id="afe7c-134">Response</span></span>

<span data-ttu-id="afe7c-135">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="afe7c-135">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="afe7c-136">示例</span><span class="sxs-lookup"><span data-stu-id="afe7c-136">Examples</span></span>

<span data-ttu-id="afe7c-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="afe7c-137">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="afe7c-138">请求</span><span class="sxs-lookup"><span data-stu-id="afe7c-138">Request</span></span>

<span data-ttu-id="afe7c-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="afe7c-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="afe7c-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="afe7c-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipal_removepassword"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/removePassword
Content-type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="afe7c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afe7c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="afe7c-142">响应</span><span class="sxs-lookup"><span data-stu-id="afe7c-142">Response</span></span>

<span data-ttu-id="afe7c-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="afe7c-143">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordCredential"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: removePassword",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
