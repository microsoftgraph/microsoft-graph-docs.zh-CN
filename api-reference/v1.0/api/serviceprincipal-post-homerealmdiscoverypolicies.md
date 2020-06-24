---
title: 分配 homeRealmDiscoveryPolicy
description: 将 homeRealmDiscoveryPolicy 分配给 servicePrincipal。
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 387c8a1535ed040040475ef5c0c2e9a7d6cbb258
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846240"
---
# <a name="assign-homerealmdiscoverypolicy"></a><span data-ttu-id="53525-103">分配 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="53525-103">Assign homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="53525-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53525-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="53525-105">将[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)分配给[servicePrincipal](../resources/serviceprincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="53525-105">Assign a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) to a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="53525-106">权限</span><span class="sxs-lookup"><span data-stu-id="53525-106">Permissions</span></span>

<span data-ttu-id="53525-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="53525-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="53525-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53525-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53525-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="53525-109">Permission type</span></span>                        | <span data-ttu-id="53525-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53525-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="53525-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53525-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="53525-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="53525-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="53525-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53525-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53525-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="53525-114">Not supported.</span></span> |
| <span data-ttu-id="53525-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="53525-115">Application</span></span>                            | <span data-ttu-id="53525-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="53525-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53525-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53525-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="53525-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="53525-118">Request headers</span></span>

| <span data-ttu-id="53525-119">名称</span><span class="sxs-lookup"><span data-stu-id="53525-119">Name</span></span>          | <span data-ttu-id="53525-120">说明</span><span class="sxs-lookup"><span data-stu-id="53525-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="53525-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="53525-121">Authorization</span></span> | <span data-ttu-id="53525-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="53525-122">Bearer {token}.</span></span> <span data-ttu-id="53525-123">Required.</span><span class="sxs-lookup"><span data-stu-id="53525-123">Required.</span></span> |
| <span data-ttu-id="53525-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53525-124">Content-Type</span></span> | <span data-ttu-id="53525-125">application/json.</span><span class="sxs-lookup"><span data-stu-id="53525-125">application/json.</span></span> <span data-ttu-id="53525-126">Required.</span><span class="sxs-lookup"><span data-stu-id="53525-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53525-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="53525-127">Request body</span></span>

<span data-ttu-id="53525-128">在请求正文中，提供应分配给服务主体的[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象的标识符（使用 `@odata.id` 属性）。</span><span class="sxs-lookup"><span data-stu-id="53525-128">In the request body, supply the identifier of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object (using an `@odata.id` property) that should be assigned to the service principal.</span></span>

## <a name="response"></a><span data-ttu-id="53525-129">响应</span><span class="sxs-lookup"><span data-stu-id="53525-129">Response</span></span>

<span data-ttu-id="53525-130">If successful, this method returns a `204 No Content` response code.</span><span class="sxs-lookup"><span data-stu-id="53525-130">If successful, this method returns a `204 No Content` response code.</span></span> <span data-ttu-id="53525-131">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="53525-131">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53525-132">示例</span><span class="sxs-lookup"><span data-stu-id="53525-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53525-133">请求</span><span class="sxs-lookup"><span data-stu-id="53525-133">Request</span></span>

<span data-ttu-id="53525-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53525-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="53525-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="53525-135">HTTP</span></span>](#tab/http)
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

### <a name="response"></a><span data-ttu-id="53525-136">响应</span><span class="sxs-lookup"><span data-stu-id="53525-136">Response</span></span>

<span data-ttu-id="53525-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53525-137">The following is an example of the response.</span></span>

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
