---
title: 分配 claimsMappingPolicy
description: 将 claimsMappingPolicy 分配给 servicePrincipal。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b22afa1dd68f90bbae069055fb0999a90ed17a0b
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863546"
---
# <a name="assign-claimsmappingpolicy"></a><span data-ttu-id="5033d-103">分配 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="5033d-103">Assign claimsMappingPolicy</span></span>

<span data-ttu-id="5033d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5033d-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="5033d-105">将[claimsMappingPolicy](../resources/claimsmappingpolicy.md)分配给[servicePrincipal](../resources/serviceprincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="5033d-105">Assign a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5033d-106">权限</span><span class="sxs-lookup"><span data-stu-id="5033d-106">Permissions</span></span>

<span data-ttu-id="5033d-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5033d-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5033d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5033d-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5033d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5033d-109">Permission type</span></span>                        | <span data-ttu-id="5033d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5033d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5033d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5033d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5033d-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="5033d-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="5033d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5033d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5033d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5033d-114">Not supported.</span></span> |
| <span data-ttu-id="5033d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5033d-115">Application</span></span>                            | <span data-ttu-id="5033d-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="5033d-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5033d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5033d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/claimsMappingPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="5033d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5033d-118">Request headers</span></span>

| <span data-ttu-id="5033d-119">名称</span><span class="sxs-lookup"><span data-stu-id="5033d-119">Name</span></span>          | <span data-ttu-id="5033d-120">说明</span><span class="sxs-lookup"><span data-stu-id="5033d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5033d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5033d-121">Authorization</span></span> | <span data-ttu-id="5033d-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5033d-122">Bearer {token}.</span></span> <span data-ttu-id="5033d-123">Required.</span><span class="sxs-lookup"><span data-stu-id="5033d-123">Required.</span></span> |
| <span data-ttu-id="5033d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5033d-124">Content-Type</span></span> | <span data-ttu-id="5033d-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="5033d-125">application/json.</span></span> <span data-ttu-id="5033d-126">Required.</span><span class="sxs-lookup"><span data-stu-id="5033d-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5033d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5033d-127">Request body</span></span>

<span data-ttu-id="5033d-128">在请求正文中，提供应分配给服务主体的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的标识符（使用 `@odata.id` 属性）。</span><span class="sxs-lookup"><span data-stu-id="5033d-128">In the request body, supply the identifier of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="5033d-129">响应</span><span class="sxs-lookup"><span data-stu-id="5033d-129">Response</span></span>

<span data-ttu-id="5033d-130">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="5033d-130">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="5033d-131">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="5033d-131">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5033d-132">示例</span><span class="sxs-lookup"><span data-stu-id="5033d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5033d-133">请求</span><span class="sxs-lookup"><span data-stu-id="5033d-133">Request</span></span>

<span data-ttu-id="5033d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5033d-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5033d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5033d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_servicePrincipal"
}-->

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/claimsMappingPolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="c"></a>[<span data-ttu-id="5033d-136">C#</span><span class="sxs-lookup"><span data-stu-id="5033d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5033d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5033d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5033d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5033d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5033d-139">Java</span><span class="sxs-lookup"><span data-stu-id="5033d-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-claimsmappingpolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5033d-140">响应</span><span class="sxs-lookup"><span data-stu-id="5033d-140">Response</span></span>

<span data-ttu-id="5033d-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5033d-141">The following is an example of the response.</span></span>

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
