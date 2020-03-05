---
title: 分配 tokenLifetimePolicy
description: 将 tokenLifetimePolicy 分配给应用程序或服务主体。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e260db74d65b2afd3bab2fabc20aba8f55f4c2fc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441432"
---
# <a name="assign-tokenlifetimepolicy"></a><span data-ttu-id="db12e-103">分配 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="db12e-103">Assign tokenLifetimePolicy</span></span>

<span data-ttu-id="db12e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="db12e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db12e-105">将[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)分配给[应用程序](../resources/application.md)或[servicePrincipal](../resources/servicePrincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="db12e-105">Assign a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="db12e-106">权限</span><span class="sxs-lookup"><span data-stu-id="db12e-106">Permissions</span></span>

<span data-ttu-id="db12e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db12e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db12e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db12e-109">Permission type</span></span>                        | <span data-ttu-id="db12e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db12e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db12e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db12e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db12e-112">Policy. All 和 Application。所有读写。</span><span class="sxs-lookup"><span data-stu-id="db12e-112">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="db12e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db12e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db12e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db12e-114">Not supported.</span></span> |
| <span data-ttu-id="db12e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db12e-115">Application</span></span>                            | <span data-ttu-id="db12e-116">Policy. All 和 Application.readwrite.ownedby，all 和应用程序的 Read. all</span><span class="sxs-lookup"><span data-stu-id="db12e-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db12e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db12e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
POST /servicePrincipals/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="db12e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="db12e-118">Request headers</span></span>

| <span data-ttu-id="db12e-119">名称</span><span class="sxs-lookup"><span data-stu-id="db12e-119">Name</span></span>          | <span data-ttu-id="db12e-120">说明</span><span class="sxs-lookup"><span data-stu-id="db12e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="db12e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="db12e-121">Authorization</span></span> | <span data-ttu-id="db12e-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="db12e-122">Bearer {token}</span></span> |
| <span data-ttu-id="db12e-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="db12e-123">Content-Type</span></span> | <span data-ttu-id="db12e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="db12e-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="db12e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="db12e-125">Request body</span></span>

<span data-ttu-id="db12e-126">在请求正文中，提供应分配给应用[](../resources/tokenlifetimepolicy.md)程序或服务主体的`@odata.id` tokenLifetimePolicy 对象的标识符（使用属性）。</span><span class="sxs-lookup"><span data-stu-id="db12e-126">In the request body, supply the identifier of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object (using an `@odata.id` property) that should be assigned to the application or service principal.</span></span>

## <a name="response"></a><span data-ttu-id="db12e-127">响应</span><span class="sxs-lookup"><span data-stu-id="db12e-127">Response</span></span>

<span data-ttu-id="db12e-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="db12e-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db12e-130">示例</span><span class="sxs-lookup"><span data-stu-id="db12e-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db12e-131">请求</span><span class="sxs-lookup"><span data-stu-id="db12e-131">Request</span></span>

<span data-ttu-id="db12e-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db12e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db12e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="db12e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="db12e-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db12e-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db12e-135">响应</span><span class="sxs-lookup"><span data-stu-id="db12e-135">Response</span></span>

<span data-ttu-id="db12e-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="db12e-136">The following is an example of the response.</span></span>

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
  "description": "Assign tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
