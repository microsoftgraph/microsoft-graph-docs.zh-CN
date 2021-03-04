---
title: 删除 userFlow
description: 删除 userFlow。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6185c79777772b461c562f831d1bb135f2a00aa0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435348"
---
# <a name="delete-userflow"></a><span data-ttu-id="db8c2-103">删除 userFlow</span><span class="sxs-lookup"><span data-stu-id="db8c2-103">Delete userFlow</span></span>

<span data-ttu-id="db8c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db8c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db8c2-105">删除现有 [userFlow](../resources/identityuserflow.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db8c2-105">Delete an existing [userFlow](../resources/identityuserflow.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="db8c2-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="db8c2-106">Permissions</span></span>

<span data-ttu-id="db8c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="db8c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="db8c2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db8c2-109">Permission type</span></span>                        | <span data-ttu-id="db8c2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="db8c2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="db8c2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db8c2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="db8c2-112">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db8c2-112">IdentityUserFlow.ReadWrite.All</span></span> |
| <span data-ttu-id="db8c2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db8c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db8c2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db8c2-114">Not supported.</span></span> |
| <span data-ttu-id="db8c2-115">Application</span><span class="sxs-lookup"><span data-stu-id="db8c2-115">Application</span></span>                            | <span data-ttu-id="db8c2-116">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db8c2-116">IdentityUserFlow.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db8c2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db8c2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /identity/userFlows/{id}
```

## <a name="request-headers"></a><span data-ttu-id="db8c2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="db8c2-118">Request headers</span></span>

| <span data-ttu-id="db8c2-119">名称</span><span class="sxs-lookup"><span data-stu-id="db8c2-119">Name</span></span>          | <span data-ttu-id="db8c2-120">说明</span><span class="sxs-lookup"><span data-stu-id="db8c2-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="db8c2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="db8c2-121">Authorization</span></span> | <span data-ttu-id="db8c2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="db8c2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db8c2-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="db8c2-124">Request body</span></span>

<span data-ttu-id="db8c2-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db8c2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db8c2-126">响应</span><span class="sxs-lookup"><span data-stu-id="db8c2-126">Response</span></span>

<span data-ttu-id="db8c2-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="db8c2-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="db8c2-129">示例</span><span class="sxs-lookup"><span data-stu-id="db8c2-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="db8c2-130">请求</span><span class="sxs-lookup"><span data-stu-id="db8c2-130">Request</span></span>

<span data-ttu-id="db8c2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="db8c2-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="db8c2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="db8c2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_identityuserflow"
}-->

```http
DELETE https://graph.microsoft.com/beta/identity/userFlows/{id}
```
# <a name="c"></a>[<span data-ttu-id="db8c2-133">C#</span><span class="sxs-lookup"><span data-stu-id="db8c2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-identityuserflow-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="db8c2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="db8c2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-identityuserflow-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="db8c2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="db8c2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-identityuserflow-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="db8c2-136">Java</span><span class="sxs-lookup"><span data-stu-id="db8c2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-identityuserflow-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="db8c2-137">响应</span><span class="sxs-lookup"><span data-stu-id="db8c2-137">Response</span></span>

<span data-ttu-id="db8c2-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="db8c2-138">The following is an example of the response.</span></span>

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
  "description": "Delete userFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


