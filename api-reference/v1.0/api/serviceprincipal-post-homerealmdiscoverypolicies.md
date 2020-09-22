---
title: 分配 homeRealmDiscoveryPolicy
description: 将 homeRealmDiscoveryPolicy 分配给 servicePrincipal。
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 506a71ca270a50bbbd4ff8ad90b59800073357b5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48045528"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="ce1eb-103">分配 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="ce1eb-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="ce1eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce1eb-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="ce1eb-105">将 [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 分配给 [servicePrincipal](../resources/serviceprincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="ce1eb-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce1eb-106">权限</span><span class="sxs-lookup"><span data-stu-id="ce1eb-106">Permissions</span></span>

<span data-ttu-id="ce1eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ce1eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce1eb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ce1eb-109">Permission type</span></span>                        | <span data-ttu-id="ce1eb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ce1eb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ce1eb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ce1eb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ce1eb-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="ce1eb-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="ce1eb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ce1eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce1eb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ce1eb-114">Not supported.</span></span> |
| <span data-ttu-id="ce1eb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ce1eb-115">Application</span></span>                            | <span data-ttu-id="ce1eb-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="ce1eb-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ce1eb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ce1eb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ce1eb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ce1eb-118">Request headers</span></span>

| <span data-ttu-id="ce1eb-119">名称</span><span class="sxs-lookup"><span data-stu-id="ce1eb-119">Name</span></span>          | <span data-ttu-id="ce1eb-120">说明</span><span class="sxs-lookup"><span data-stu-id="ce1eb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ce1eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce1eb-121">Authorization</span></span> | <span data-ttu-id="ce1eb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ce1eb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ce1eb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ce1eb-124">Content-Type</span></span> | <span data-ttu-id="ce1eb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ce1eb-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce1eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ce1eb-127">Request body</span></span>

<span data-ttu-id="ce1eb-128">在请求正文中，使用[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) `@odata.id` 应分配给服务主体的属性) 提供 homeRealmDiscoveryPolicy 对象 (的标识符。</span><span class="sxs-lookup"><span data-stu-id="ce1eb-128">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="ce1eb-129">响应</span><span class="sxs-lookup"><span data-stu-id="ce1eb-129">Response</span></span>

<span data-ttu-id="ce1eb-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ce1eb-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce1eb-132">示例</span><span class="sxs-lookup"><span data-stu-id="ce1eb-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce1eb-133">请求</span><span class="sxs-lookup"><span data-stu-id="ce1eb-133">Request</span></span>

<span data-ttu-id="ce1eb-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ce1eb-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ce1eb-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce1eb-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_servicePrincipal"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="c"></a>[<span data-ttu-id="ce1eb-136">C#</span><span class="sxs-lookup"><span data-stu-id="ce1eb-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce1eb-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce1eb-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce1eb-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce1eb-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce1eb-139">Java</span><span class="sxs-lookup"><span data-stu-id="ce1eb-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ce1eb-140">响应</span><span class="sxs-lookup"><span data-stu-id="ce1eb-140">Response</span></span>

<span data-ttu-id="ce1eb-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ce1eb-141">The following is an example of the response.</span></span>

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

