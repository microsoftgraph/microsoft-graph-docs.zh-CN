---
title: 分配 claimsMappingPolicy
description: 将 claimsMappingPolicy 分配给 servicePrincipal。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 379c92cccbdd169e3b4104923737934a0648e81f
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846242"
---
# <a name="assign-claimsmappingpolicy"></a><span data-ttu-id="dc35c-103">分配 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="dc35c-103">Assign claimsMappingPolicy</span></span>

<span data-ttu-id="dc35c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc35c-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="dc35c-105">将[claimsMappingPolicy](../resources/claimsmappingpolicy.md)分配给[servicePrincipal](../resources/serviceprincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="dc35c-105">Assign a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="dc35c-106">权限</span><span class="sxs-lookup"><span data-stu-id="dc35c-106">Permissions</span></span>

<span data-ttu-id="dc35c-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="dc35c-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="dc35c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc35c-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dc35c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc35c-109">Permission type</span></span>                        | <span data-ttu-id="dc35c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc35c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dc35c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc35c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dc35c-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="dc35c-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="dc35c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc35c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc35c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc35c-114">Not supported.</span></span> |
| <span data-ttu-id="dc35c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc35c-115">Application</span></span>                            | <span data-ttu-id="dc35c-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="dc35c-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc35c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc35c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/claimsMappingPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="dc35c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc35c-118">Request headers</span></span>

| <span data-ttu-id="dc35c-119">名称</span><span class="sxs-lookup"><span data-stu-id="dc35c-119">Name</span></span>          | <span data-ttu-id="dc35c-120">说明</span><span class="sxs-lookup"><span data-stu-id="dc35c-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="dc35c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc35c-121">Authorization</span></span> | <span data-ttu-id="dc35c-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="dc35c-122">Bearer {token}.</span></span> <span data-ttu-id="dc35c-123">Required.</span><span class="sxs-lookup"><span data-stu-id="dc35c-123">Required.</span></span> |
| <span data-ttu-id="dc35c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dc35c-124">Content-Type</span></span> | <span data-ttu-id="dc35c-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="dc35c-125">application/json.</span></span> <span data-ttu-id="dc35c-126">Required.</span><span class="sxs-lookup"><span data-stu-id="dc35c-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc35c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc35c-127">Request body</span></span>

<span data-ttu-id="dc35c-128">在请求正文中，提供应分配给服务主体的[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象的标识符（使用 `@odata.id` 属性）。</span><span class="sxs-lookup"><span data-stu-id="dc35c-128">In the request body, supply the identifier of the [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="dc35c-129">响应</span><span class="sxs-lookup"><span data-stu-id="dc35c-129">Response</span></span>

<span data-ttu-id="dc35c-130">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="dc35c-130">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="dc35c-131">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="dc35c-131">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dc35c-132">示例</span><span class="sxs-lookup"><span data-stu-id="dc35c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dc35c-133">请求</span><span class="sxs-lookup"><span data-stu-id="dc35c-133">Request</span></span>

<span data-ttu-id="dc35c-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dc35c-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dc35c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc35c-135">HTTP</span></span>](#tab/http)
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

### <a name="response"></a><span data-ttu-id="dc35c-136">响应</span><span class="sxs-lookup"><span data-stu-id="dc35c-136">Response</span></span>

<span data-ttu-id="dc35c-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dc35c-137">The following is an example of the response.</span></span>

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
