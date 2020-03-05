---
title: servicePrincipal： removePassword
description: 从 servicePrincipal 中删除密码
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 57c7c225ba2b5475f141c23abdef39e8a08a542b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453343"
---
# <a name="serviceprincipal-removepassword"></a><span data-ttu-id="2fc82-103">servicePrincipal： removePassword</span><span class="sxs-lookup"><span data-stu-id="2fc82-103">servicePrincipal: removePassword</span></span>

<span data-ttu-id="2fc82-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2fc82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fc82-105">从[servicePrincipal](../resources/serviceprincipal.md)对象中删除密码。</span><span class="sxs-lookup"><span data-stu-id="2fc82-105">Remove a password from a [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fc82-106">权限</span><span class="sxs-lookup"><span data-stu-id="2fc82-106">Permissions</span></span>

<span data-ttu-id="2fc82-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2fc82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2fc82-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2fc82-109">Permission type</span></span>                        | <span data-ttu-id="2fc82-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2fc82-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2fc82-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2fc82-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2fc82-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2fc82-112">Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="2fc82-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2fc82-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fc82-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fc82-114">Not supported.</span></span> |
| <span data-ttu-id="2fc82-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2fc82-115">Application</span></span>                            | <span data-ttu-id="2fc82-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2fc82-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fc82-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2fc82-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/removePassword
```

## <a name="request-headers"></a><span data-ttu-id="2fc82-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2fc82-118">Request headers</span></span>

| <span data-ttu-id="2fc82-119">名称</span><span class="sxs-lookup"><span data-stu-id="2fc82-119">Name</span></span>           | <span data-ttu-id="2fc82-120">说明</span><span class="sxs-lookup"><span data-stu-id="2fc82-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="2fc82-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fc82-121">Authorization</span></span>  | <span data-ttu-id="2fc82-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2fc82-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2fc82-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="2fc82-124">Content-type</span></span>   | <span data-ttu-id="2fc82-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2fc82-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fc82-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2fc82-127">Request body</span></span>

| <span data-ttu-id="2fc82-128">属性</span><span class="sxs-lookup"><span data-stu-id="2fc82-128">Property</span></span>     | <span data-ttu-id="2fc82-129">类型</span><span class="sxs-lookup"><span data-stu-id="2fc82-129">Type</span></span>   |<span data-ttu-id="2fc82-130">说明</span><span class="sxs-lookup"><span data-stu-id="2fc82-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2fc82-131">keyId</span><span class="sxs-lookup"><span data-stu-id="2fc82-131">keyId</span></span> | <span data-ttu-id="2fc82-132">GUID</span><span class="sxs-lookup"><span data-stu-id="2fc82-132">GUID</span></span> | <span data-ttu-id="2fc82-133">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2fc82-133">The unique identifier for the password.</span></span> <span data-ttu-id="2fc82-134">必需。</span><span class="sxs-lookup"><span data-stu-id="2fc82-134">Required.</span></span> |

## <a name="response"></a><span data-ttu-id="2fc82-135">响应</span><span class="sxs-lookup"><span data-stu-id="2fc82-135">Response</span></span>

<span data-ttu-id="2fc82-136">如果成功，此方法返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2fc82-136">If successful, this method returns a `204 No content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2fc82-137">示例</span><span class="sxs-lookup"><span data-stu-id="2fc82-137">Examples</span></span>

<span data-ttu-id="2fc82-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="2fc82-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2fc82-139">请求</span><span class="sxs-lookup"><span data-stu-id="2fc82-139">Request</span></span>

<span data-ttu-id="2fc82-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2fc82-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2fc82-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="2fc82-141">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="2fc82-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2fc82-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-removepassword-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2fc82-143">响应</span><span class="sxs-lookup"><span data-stu-id="2fc82-143">Response</span></span>

<span data-ttu-id="2fc82-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2fc82-144">The following is an example of the response.</span></span>

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
