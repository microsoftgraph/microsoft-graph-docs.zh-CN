---
title: 删除 homeRealmDiscoveryPolicy
description: 从 servicePrincipal 中删除 homeRealmDiscoveryPolicy。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 65c208e572962677ea8f8e4c3d75f9f55ce51b36
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133348"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="6a1b8-103">删除 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="6a1b8-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="6a1b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a1b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a1b8-105">从[servicePrincipal](../resources/servicePrincipal.md)中删除[homeRealmDiscoveryPolicy。](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6a1b8-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a1b8-106">权限</span><span class="sxs-lookup"><span data-stu-id="6a1b8-106">Permissions</span></span>

<span data-ttu-id="6a1b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a1b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a1b8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a1b8-109">Permission type</span></span>                        | <span data-ttu-id="6a1b8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a1b8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6a1b8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a1b8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a1b8-112">Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a1b8-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="6a1b8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a1b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a1b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a1b8-114">Not supported.</span></span> |
| <span data-ttu-id="6a1b8-115">Application</span><span class="sxs-lookup"><span data-stu-id="6a1b8-115">Application</span></span>                            | <span data-ttu-id="6a1b8-116">Policy.Read.All 和 Application.ReadWrite.OwnedBy、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.OwnedBy、Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a1b8-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a1b8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a1b8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{servicePrincipalId}/homeRealmDiscoveryPolicies/{policyId}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6a1b8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a1b8-118">Request headers</span></span>

| <span data-ttu-id="6a1b8-119">名称</span><span class="sxs-lookup"><span data-stu-id="6a1b8-119">Name</span></span>          | <span data-ttu-id="6a1b8-120">说明</span><span class="sxs-lookup"><span data-stu-id="6a1b8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6a1b8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a1b8-121">Authorization</span></span> | <span data-ttu-id="6a1b8-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="6a1b8-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a1b8-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a1b8-123">Request body</span></span>

<span data-ttu-id="6a1b8-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a1b8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a1b8-125">响应</span><span class="sxs-lookup"><span data-stu-id="6a1b8-125">Response</span></span>

<span data-ttu-id="6a1b8-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6a1b8-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="6a1b8-127">示例</span><span class="sxs-lookup"><span data-stu-id="6a1b8-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a1b8-128">请求</span><span class="sxs-lookup"><span data-stu-id="6a1b8-128">Request</span></span>

<span data-ttu-id="6a1b8-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6a1b8-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6a1b8-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a1b8-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalId}/homeRealmDiscoveryPolicies/{policyId}/$ref
```
# <a name="c"></a>[<span data-ttu-id="6a1b8-131">C#</span><span class="sxs-lookup"><span data-stu-id="6a1b8-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6a1b8-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a1b8-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6a1b8-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a1b8-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6a1b8-134">Java</span><span class="sxs-lookup"><span data-stu-id="6a1b8-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6a1b8-135">响应</span><span class="sxs-lookup"><span data-stu-id="6a1b8-135">Response</span></span>

<span data-ttu-id="6a1b8-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6a1b8-136">The following is an example of the response.</span></span>

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



