---
title: 分配 claimsMappingPolicy
description: 将 claimsMappingPolicy 分配给服务主体。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 476e2cff0c2fe519ce99b1157df5a27c013b6a04
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218631"
---
# <a name="assign-claimsmappingpolicy"></a><span data-ttu-id="76e75-103">分配 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="76e75-103">Assign claimsMappingPolicy</span></span>

<span data-ttu-id="76e75-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76e75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76e75-105">将[claimsMappingPolicy](../resources/claimsmappingpolicy.md)分配给[servicePrincipal](../resources/servicePrincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="76e75-105">Assign a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) to a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="76e75-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="76e75-106">Permissions</span></span>

<span data-ttu-id="76e75-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76e75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76e75-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="76e75-109">Permission type</span></span>                        | <span data-ttu-id="76e75-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76e75-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="76e75-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76e75-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="76e75-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="76e75-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="76e75-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76e75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76e75-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="76e75-114">Not supported.</span></span> |
| <span data-ttu-id="76e75-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="76e75-115">Application</span></span>                            | <span data-ttu-id="76e75-116">Application.readwrite.ownedby、ApplicationConfiguration 和应用程序的 Application.readwrite.ownedby、、ApplicationConfiguration 和应用程序的、和。 all，all。和和应用程序的所有写读。</span><span class="sxs-lookup"><span data-stu-id="76e75-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76e75-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76e75-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/claimsMappingPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="76e75-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="76e75-118">Request headers</span></span>

| <span data-ttu-id="76e75-119">名称</span><span class="sxs-lookup"><span data-stu-id="76e75-119">Name</span></span>          | <span data-ttu-id="76e75-120">说明</span><span class="sxs-lookup"><span data-stu-id="76e75-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="76e75-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="76e75-121">Authorization</span></span> | <span data-ttu-id="76e75-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="76e75-122">Bearer {token}</span></span> |
| <span data-ttu-id="76e75-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76e75-123">Content-Type</span></span> | <span data-ttu-id="76e75-124">application/json</span><span class="sxs-lookup"><span data-stu-id="76e75-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="76e75-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="76e75-125">Request body</span></span>

<span data-ttu-id="76e75-126">在请求正文中，提供应分配给服务主体的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的`@odata.id`标识符（使用属性）。</span><span class="sxs-lookup"><span data-stu-id="76e75-126">In the request body, supply the identifier of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="76e75-127">响应</span><span class="sxs-lookup"><span data-stu-id="76e75-127">Response</span></span>

<span data-ttu-id="76e75-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="76e75-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="76e75-130">示例</span><span class="sxs-lookup"><span data-stu-id="76e75-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76e75-131">请求</span><span class="sxs-lookup"><span data-stu-id="76e75-131">Request</span></span>

<span data-ttu-id="76e75-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="76e75-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="76e75-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="76e75-133">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="76e75-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="76e75-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="76e75-135">C#</span><span class="sxs-lookup"><span data-stu-id="76e75-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="76e75-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="76e75-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="76e75-137">响应</span><span class="sxs-lookup"><span data-stu-id="76e75-137">Response</span></span>

<span data-ttu-id="76e75-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="76e75-138">The following is an example of the response.</span></span>

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
