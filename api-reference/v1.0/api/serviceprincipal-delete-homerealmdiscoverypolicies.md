---
title: 删除 homeRealmDiscoveryPolicy
description: 从 servicePrincipal 中删除 homeRealmDiscoveryPolicy。
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b8c5f152f8e44f31b0016b480019fb36d132d953
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846203"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="76645-103">删除 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="76645-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="76645-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76645-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="76645-105">从[servicePrincipal](../resources/serviceprincipal.md)中删除[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 。</span><span class="sxs-lookup"><span data-stu-id="76645-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="76645-106">权限</span><span class="sxs-lookup"><span data-stu-id="76645-106">Permissions</span></span>

<span data-ttu-id="76645-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="76645-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="76645-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76645-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="76645-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="76645-109">Permission type</span></span>                        | <span data-ttu-id="76645-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="76645-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="76645-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76645-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="76645-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="76645-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="76645-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76645-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76645-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="76645-114">Not supported.</span></span> |
| <span data-ttu-id="76645-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="76645-115">Application</span></span>                            | <span data-ttu-id="76645-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="76645-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76645-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76645-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="76645-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="76645-118">Request headers</span></span>

| <span data-ttu-id="76645-119">名称</span><span class="sxs-lookup"><span data-stu-id="76645-119">Name</span></span>          | <span data-ttu-id="76645-120">说明</span><span class="sxs-lookup"><span data-stu-id="76645-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="76645-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="76645-121">Authorization</span></span> | <span data-ttu-id="76645-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="76645-122">Bearer {token}.</span></span> <span data-ttu-id="76645-123">Required.</span><span class="sxs-lookup"><span data-stu-id="76645-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="76645-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="76645-124">Request body</span></span>

<span data-ttu-id="76645-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76645-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76645-126">响应</span><span class="sxs-lookup"><span data-stu-id="76645-126">Response</span></span>

<span data-ttu-id="76645-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="76645-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="76645-128">示例</span><span class="sxs-lookup"><span data-stu-id="76645-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="76645-129">请求</span><span class="sxs-lookup"><span data-stu-id="76645-129">Request</span></span>

<span data-ttu-id="76645-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="76645-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="76645-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="76645-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_servicePrincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="76645-132">响应</span><span class="sxs-lookup"><span data-stu-id="76645-132">Response</span></span>

<span data-ttu-id="76645-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="76645-133">The following is an example of the response.</span></span>

> <span data-ttu-id="76645-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="76645-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="76645-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="76645-135">All the properties will be returned from an actual call.</span></span>

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
