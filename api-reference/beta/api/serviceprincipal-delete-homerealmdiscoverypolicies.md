---
title: 删除 homeRealmDiscoveryPolicy
description: 从 servicePrincipal 中删除 homeRealmDiscoveryPolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 421fb9be650ab22c07e940ab2eac2fcf20abf5a7
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234188"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="d5065-103">删除 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="d5065-103">Remove homeRealmDiscoveryPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5065-104">从[servicePrincipal](../resources/servicePrincipal.md)中删除[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 。</span><span class="sxs-lookup"><span data-stu-id="d5065-104">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5065-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="d5065-105">Permissions</span></span>

<span data-ttu-id="d5065-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5065-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d5065-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5065-108">Permission type</span></span>                        | <span data-ttu-id="d5065-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5065-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d5065-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5065-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5065-111">Policy. All 和 Application。所有读写。</span><span class="sxs-lookup"><span data-stu-id="d5065-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="d5065-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5065-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5065-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5065-113">Not supported.</span></span> |
| <span data-ttu-id="d5065-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5065-114">Application</span></span>                            | <span data-ttu-id="d5065-115">Policy. All 和 Application.readwrite.ownedby，all 和应用程序的 Read. all</span><span class="sxs-lookup"><span data-stu-id="d5065-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5065-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5065-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="d5065-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5065-117">Request headers</span></span>

| <span data-ttu-id="d5065-118">名称</span><span class="sxs-lookup"><span data-stu-id="d5065-118">Name</span></span>          | <span data-ttu-id="d5065-119">说明</span><span class="sxs-lookup"><span data-stu-id="d5065-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d5065-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5065-120">Authorization</span></span> | <span data-ttu-id="d5065-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d5065-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5065-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5065-122">Request body</span></span>

<span data-ttu-id="d5065-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5065-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5065-124">响应</span><span class="sxs-lookup"><span data-stu-id="d5065-124">Response</span></span>

<span data-ttu-id="d5065-125">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d5065-125">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d5065-126">示例</span><span class="sxs-lookup"><span data-stu-id="d5065-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d5065-127">请求</span><span class="sxs-lookup"><span data-stu-id="d5065-127">Request</span></span>

<span data-ttu-id="d5065-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d5065-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="d5065-129">响应</span><span class="sxs-lookup"><span data-stu-id="d5065-129">Response</span></span>

<span data-ttu-id="d5065-130">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d5065-130">The following is an example of the response.</span></span>

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
  "description": "Remove homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->