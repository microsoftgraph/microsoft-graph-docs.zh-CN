---
title: 分配 tokenLifetimePolicy
description: 将 tokenLifetimePolicy 分配给应用程序或服务主体。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fca668417d52914194ef087a32b28478101a32d7
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475615"
---
# <a name="assign-tokenlifetimepolicy"></a><span data-ttu-id="2f51f-103">分配 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="2f51f-103">Assign tokenLifetimePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f51f-104">将[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)分配给[应用程序](../resources/application.md)或[servicePrincipal](../resources/servicePrincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="2f51f-104">Assign a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f51f-105">权限</span><span class="sxs-lookup"><span data-stu-id="2f51f-105">Permissions</span></span>

<span data-ttu-id="2f51f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f51f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2f51f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f51f-108">Permission type</span></span>                        | <span data-ttu-id="2f51f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f51f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2f51f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f51f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2f51f-111">Policy. All 和 Application。所有读写。</span><span class="sxs-lookup"><span data-stu-id="2f51f-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="2f51f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f51f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f51f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f51f-113">Not supported.</span></span> |
| <span data-ttu-id="2f51f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f51f-114">Application</span></span>                            | <span data-ttu-id="2f51f-115">Policy. All 和 Application.readwrite.ownedby，all 和应用程序的 Read. all</span><span class="sxs-lookup"><span data-stu-id="2f51f-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2f51f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f51f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
POST /servicePrincipals/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2f51f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f51f-117">Request headers</span></span>

| <span data-ttu-id="2f51f-118">名称</span><span class="sxs-lookup"><span data-stu-id="2f51f-118">Name</span></span>          | <span data-ttu-id="2f51f-119">说明</span><span class="sxs-lookup"><span data-stu-id="2f51f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2f51f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f51f-120">Authorization</span></span> | <span data-ttu-id="2f51f-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="2f51f-121">Bearer {token}</span></span> |
| <span data-ttu-id="2f51f-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f51f-122">Content-Type</span></span> | <span data-ttu-id="2f51f-123">application/json</span><span class="sxs-lookup"><span data-stu-id="2f51f-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2f51f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f51f-124">Request body</span></span>

<span data-ttu-id="2f51f-125">在请求正文中，提供应分配给应用[](../resources/tokenlifetimepolicy.md)程序或服务主体的`@odata.id` tokenLifetimePolicy 对象的标识符（使用属性）。</span><span class="sxs-lookup"><span data-stu-id="2f51f-125">In the request body, supply the identifier of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object (using an `@odata.id` property) that should be assigned to the application or service principal.</span></span>

## <a name="response"></a><span data-ttu-id="2f51f-126">响应</span><span class="sxs-lookup"><span data-stu-id="2f51f-126">Response</span></span>

<span data-ttu-id="2f51f-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2f51f-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2f51f-129">示例</span><span class="sxs-lookup"><span data-stu-id="2f51f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2f51f-130">请求</span><span class="sxs-lookup"><span data-stu-id="2f51f-130">Request</span></span>

<span data-ttu-id="2f51f-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2f51f-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2f51f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f51f-132">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f51f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f51f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2f51f-134">响应</span><span class="sxs-lookup"><span data-stu-id="2f51f-134">Response</span></span>

<span data-ttu-id="2f51f-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2f51f-135">The following is an example of the response.</span></span>

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
