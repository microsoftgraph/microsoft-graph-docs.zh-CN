---
title: 删除 homeRealmDiscoveryPolicy
description: 删除 homeRealmDiscoveryPolicy。
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 803b770daa1a1e8f4aa073a83fc6214e2a862991
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434354"
---
# <a name="delete-homerealmdiscoverypolicy"></a><span data-ttu-id="47664-103">删除 homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="47664-103">Delete homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="47664-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47664-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="47664-105">删除 [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="47664-105">Delete a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="47664-106">权限</span><span class="sxs-lookup"><span data-stu-id="47664-106">Permissions</span></span>

<span data-ttu-id="47664-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="47664-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="47664-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="47664-109">Permission type</span></span>                        | <span data-ttu-id="47664-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="47664-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="47664-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47664-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="47664-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="47664-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="47664-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47664-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47664-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="47664-114">Not supported.</span></span> |
| <span data-ttu-id="47664-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="47664-115">Application</span></span>                            | <span data-ttu-id="47664-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="47664-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="47664-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47664-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="47664-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="47664-118">Request headers</span></span>

| <span data-ttu-id="47664-119">名称</span><span class="sxs-lookup"><span data-stu-id="47664-119">Name</span></span>          | <span data-ttu-id="47664-120">说明</span><span class="sxs-lookup"><span data-stu-id="47664-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="47664-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="47664-121">Authorization</span></span> | <span data-ttu-id="47664-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="47664-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47664-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="47664-124">Request body</span></span>

<span data-ttu-id="47664-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="47664-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47664-126">响应</span><span class="sxs-lookup"><span data-stu-id="47664-126">Response</span></span>

<span data-ttu-id="47664-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="47664-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="47664-128">示例</span><span class="sxs-lookup"><span data-stu-id="47664-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47664-129">请求</span><span class="sxs-lookup"><span data-stu-id="47664-129">Request</span></span>

<span data-ttu-id="47664-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="47664-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="47664-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="47664-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="47664-132">C#</span><span class="sxs-lookup"><span data-stu-id="47664-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-homerealmdiscoverypolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="47664-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47664-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-homerealmdiscoverypolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="47664-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="47664-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-homerealmdiscoverypolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="47664-135">Java</span><span class="sxs-lookup"><span data-stu-id="47664-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-homerealmdiscoverypolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="47664-136">响应</span><span class="sxs-lookup"><span data-stu-id="47664-136">Response</span></span>

<span data-ttu-id="47664-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="47664-137">The following is an example of the response.</span></span>

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
  "description": "Delete homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

