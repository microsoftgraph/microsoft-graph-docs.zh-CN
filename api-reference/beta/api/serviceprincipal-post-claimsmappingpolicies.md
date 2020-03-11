---
title: 分配 claimsMappingPolicy
description: 将 claimsMappingPolicy 分配给服务主体。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7742908d0aec8dbdfa1d3d145dcb330138541bae
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589321"
---
# <a name="assign-claimsmappingpolicy"></a><span data-ttu-id="deb6d-103">分配 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="deb6d-103">Assign claimsMappingPolicy</span></span>

<span data-ttu-id="deb6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deb6d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deb6d-105">将[claimsMappingPolicy](../resources/claimsmappingpolicy.md)分配给[servicePrincipal](../resources/servicePrincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="deb6d-105">Assign a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="deb6d-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="deb6d-106">Permissions</span></span>

<span data-ttu-id="deb6d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="deb6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="deb6d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="deb6d-109">Permission type</span></span>                        | <span data-ttu-id="deb6d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="deb6d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="deb6d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="deb6d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="deb6d-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="deb6d-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="deb6d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="deb6d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deb6d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="deb6d-114">Not supported.</span></span> |
| <span data-ttu-id="deb6d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="deb6d-115">Application</span></span>                            | <span data-ttu-id="deb6d-116">Application.readwrite.ownedby、ApplicationConfiguration 和 Application.readwrite.ownedby、、、和 ApplicationConfiguration 中的所有、和 and and and and and and and and and应用程序的读写。</span><span class="sxs-lookup"><span data-stu-id="deb6d-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="deb6d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="deb6d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/claimsMappingPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="deb6d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="deb6d-118">Request headers</span></span>

| <span data-ttu-id="deb6d-119">名称</span><span class="sxs-lookup"><span data-stu-id="deb6d-119">Name</span></span>          | <span data-ttu-id="deb6d-120">说明</span><span class="sxs-lookup"><span data-stu-id="deb6d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="deb6d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="deb6d-121">Authorization</span></span> | <span data-ttu-id="deb6d-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="deb6d-122">Bearer {token}</span></span> |
| <span data-ttu-id="deb6d-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="deb6d-123">Content-Type</span></span> | <span data-ttu-id="deb6d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="deb6d-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="deb6d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="deb6d-125">Request body</span></span>

<span data-ttu-id="deb6d-126">在请求正文中，提供应分配给服务主体的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的`@odata.id`标识符（使用属性）。</span><span class="sxs-lookup"><span data-stu-id="deb6d-126">In the request body, supply the identifier of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="deb6d-127">响应</span><span class="sxs-lookup"><span data-stu-id="deb6d-127">Response</span></span>

<span data-ttu-id="deb6d-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="deb6d-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="deb6d-130">示例</span><span class="sxs-lookup"><span data-stu-id="deb6d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="deb6d-131">请求</span><span class="sxs-lookup"><span data-stu-id="deb6d-131">Request</span></span>

<span data-ttu-id="deb6d-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="deb6d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="deb6d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="deb6d-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="deb6d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="deb6d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="deb6d-135">C#</span><span class="sxs-lookup"><span data-stu-id="deb6d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="deb6d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="deb6d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="deb6d-137">响应</span><span class="sxs-lookup"><span data-stu-id="deb6d-137">Response</span></span>

<span data-ttu-id="deb6d-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="deb6d-138">The following is an example of the response.</span></span>

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
  "description": "Assign claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
