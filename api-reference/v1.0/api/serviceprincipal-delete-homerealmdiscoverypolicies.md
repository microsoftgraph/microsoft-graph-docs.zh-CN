---
title: 删除 homeRealmDiscoveryPolicy
description: 从 servicePrincipal 中删除 homeRealmDiscoveryPolicy。
localization_priority: Normal
author: hpsin
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: a4adb9428f9d70b98973707a014439042bdcf142
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038892"
---
# <a name="remove-homerealmdiscoverypolicy"></a><span data-ttu-id="0a5a4-103">删除 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="0a5a4-103">Remove homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="0a5a4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a5a4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0a5a4-105">从[servicePrincipal](../resources/serviceprincipal.md)中删除[homeRealmDiscoveryPolicy。](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="0a5a4-105">Remove a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) from a [servicePrincipal](../resources/serviceprincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0a5a4-106">权限</span><span class="sxs-lookup"><span data-stu-id="0a5a4-106">Permissions</span></span>

<span data-ttu-id="0a5a4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a5a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0a5a4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a5a4-109">Permission type</span></span>                        | <span data-ttu-id="0a5a4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a5a4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0a5a4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a5a4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a5a4-112">Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a5a4-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="0a5a4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a5a4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a5a4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a5a4-114">Not supported.</span></span> |
| <span data-ttu-id="0a5a4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a5a4-115">Application</span></span>                            | <span data-ttu-id="0a5a4-116">Policy.Read.All 和 Application.ReadWrite.OwnedBy、Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.OwnedBy、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a5a4-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a5a4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a5a4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="0a5a4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a5a4-118">Request headers</span></span>

| <span data-ttu-id="0a5a4-119">名称</span><span class="sxs-lookup"><span data-stu-id="0a5a4-119">Name</span></span>          | <span data-ttu-id="0a5a4-120">说明</span><span class="sxs-lookup"><span data-stu-id="0a5a4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0a5a4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a5a4-121">Authorization</span></span> | <span data-ttu-id="0a5a4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a5a4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a5a4-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a5a4-124">Request body</span></span>

<span data-ttu-id="0a5a4-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a5a4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a5a4-126">响应</span><span class="sxs-lookup"><span data-stu-id="0a5a4-126">Response</span></span>

<span data-ttu-id="0a5a4-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="0a5a4-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="0a5a4-128">示例</span><span class="sxs-lookup"><span data-stu-id="0a5a4-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0a5a4-129">请求</span><span class="sxs-lookup"><span data-stu-id="0a5a4-129">Request</span></span>

<span data-ttu-id="0a5a4-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0a5a4-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0a5a4-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a5a4-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy_from_servicePrincipal"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/homeRealmDiscoveryPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="0a5a4-132">C#</span><span class="sxs-lookup"><span data-stu-id="0a5a4-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a5a4-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a5a4-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a5a4-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a5a4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0a5a4-135">Java</span><span class="sxs-lookup"><span data-stu-id="0a5a4-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0a5a4-136">响应</span><span class="sxs-lookup"><span data-stu-id="0a5a4-136">Response</span></span>

<span data-ttu-id="0a5a4-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0a5a4-137">The following is an example of the response.</span></span>

> <span data-ttu-id="0a5a4-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0a5a4-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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

