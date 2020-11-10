---
title: 分配 homeRealmDiscoveryPolicy
description: 将 homeRealmDiscoveryPolicy 分配给服务主体。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: eecb6ddb41e7f64788e8fea83be4ac18b9771421
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979640"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="7c14a-103">分配 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="7c14a-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="7c14a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c14a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c14a-105">将 [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 分配给 [servicePrincipal](../resources/servicePrincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="7c14a-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7c14a-106">权限</span><span class="sxs-lookup"><span data-stu-id="7c14a-106">Permissions</span></span>

<span data-ttu-id="7c14a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c14a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7c14a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c14a-109">Permission type</span></span>                        | <span data-ttu-id="7c14a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c14a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7c14a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c14a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7c14a-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="7c14a-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="7c14a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c14a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c14a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c14a-114">Not supported.</span></span> |
| <span data-ttu-id="7c14a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c14a-115">Application</span></span>                            | <span data-ttu-id="7c14a-116">Application.readwrite.ownedby、ApplicationConfiguration 和应用程序的 Application.readwrite.ownedby、、ApplicationConfiguration 和应用程序的、和。 all，all。和和应用程序的所有写读。</span><span class="sxs-lookup"><span data-stu-id="7c14a-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c14a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c14a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7c14a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c14a-118">Request headers</span></span>

| <span data-ttu-id="7c14a-119">名称</span><span class="sxs-lookup"><span data-stu-id="7c14a-119">Name</span></span>          | <span data-ttu-id="7c14a-120">说明</span><span class="sxs-lookup"><span data-stu-id="7c14a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7c14a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c14a-121">Authorization</span></span> | <span data-ttu-id="7c14a-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7c14a-122">Bearer {token}</span></span> |
| <span data-ttu-id="7c14a-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7c14a-123">Content-Type</span></span> | <span data-ttu-id="7c14a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7c14a-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7c14a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c14a-125">Request body</span></span>

<span data-ttu-id="7c14a-126">在请求正文中，使用[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) `@odata.id` 应分配给服务主体的属性) 提供 homeRealmDiscoveryPolicy 对象 (的标识符。</span><span class="sxs-lookup"><span data-stu-id="7c14a-126">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="7c14a-127">响应</span><span class="sxs-lookup"><span data-stu-id="7c14a-127">Response</span></span>

<span data-ttu-id="7c14a-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7c14a-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7c14a-130">示例</span><span class="sxs-lookup"><span data-stu-id="7c14a-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7c14a-131">请求</span><span class="sxs-lookup"><span data-stu-id="7c14a-131">Request</span></span>

<span data-ttu-id="7c14a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7c14a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7c14a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c14a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="7c14a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c14a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="7c14a-135">C#</span><span class="sxs-lookup"><span data-stu-id="7c14a-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c14a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c14a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c14a-137">Java</span><span class="sxs-lookup"><span data-stu-id="7c14a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7c14a-138">响应</span><span class="sxs-lookup"><span data-stu-id="7c14a-138">Response</span></span>

<span data-ttu-id="7c14a-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7c14a-139">The following is an example of the response.</span></span>

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
  "description": "Assign homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


