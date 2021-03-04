---
title: 删除 trustFrameworkKeySet
description: 删除 **trustFrameworkKeySet** 对象。
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 04527223a407724146b26b3319b527c7f7f97ba6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433656"
---
# <a name="delete-trustframeworkkeyset"></a><span data-ttu-id="8bbaf-103">删除 trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="8bbaf-103">Delete trustFrameworkKeySet</span></span>

<span data-ttu-id="8bbaf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bbaf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bbaf-105">删除 [trustFrameworkKeySet](../resources/trustframeworkkeyset.md)。</span><span class="sxs-lookup"><span data-stu-id="8bbaf-105">Delete a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8bbaf-106">权限</span><span class="sxs-lookup"><span data-stu-id="8bbaf-106">Permissions</span></span>

<span data-ttu-id="8bbaf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8bbaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8bbaf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8bbaf-109">Permission type</span></span>                        | <span data-ttu-id="8bbaf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8bbaf-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8bbaf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8bbaf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8bbaf-112">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bbaf-112">TrustFrameworkKeySet.ReadWrite.All</span></span> |
| <span data-ttu-id="8bbaf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8bbaf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bbaf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8bbaf-114">Not supported.</span></span> |
| <span data-ttu-id="8bbaf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8bbaf-115">Application</span></span>                            | <span data-ttu-id="8bbaf-116">TrustFrameworkKeySet.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bbaf-116">TrustFrameworkKeySet.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bbaf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8bbaf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /trustFramework/keySets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8bbaf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8bbaf-118">Request headers</span></span>

| <span data-ttu-id="8bbaf-119">名称</span><span class="sxs-lookup"><span data-stu-id="8bbaf-119">Name</span></span>          | <span data-ttu-id="8bbaf-120">说明</span><span class="sxs-lookup"><span data-stu-id="8bbaf-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8bbaf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bbaf-121">Authorization</span></span> | <span data-ttu-id="8bbaf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8bbaf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bbaf-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8bbaf-124">Request body</span></span>

<span data-ttu-id="8bbaf-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8bbaf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bbaf-126">响应</span><span class="sxs-lookup"><span data-stu-id="8bbaf-126">Response</span></span>

<span data-ttu-id="8bbaf-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8bbaf-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8bbaf-129">示例</span><span class="sxs-lookup"><span data-stu-id="8bbaf-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8bbaf-130">请求</span><span class="sxs-lookup"><span data-stu-id="8bbaf-130">Request</span></span>

<span data-ttu-id="8bbaf-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8bbaf-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8bbaf-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bbaf-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_trustframeworkkeyset"
}-->

```http
DELETE https://graph.microsoft.com/beta/trustFramework/keySets/{id}
```
# <a name="c"></a>[<span data-ttu-id="8bbaf-133">C#</span><span class="sxs-lookup"><span data-stu-id="8bbaf-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-trustframeworkkeyset-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bbaf-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bbaf-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-trustframeworkkeyset-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bbaf-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bbaf-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-trustframeworkkeyset-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8bbaf-136">Java</span><span class="sxs-lookup"><span data-stu-id="8bbaf-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-trustframeworkkeyset-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8bbaf-137">响应</span><span class="sxs-lookup"><span data-stu-id="8bbaf-137">Response</span></span>

<span data-ttu-id="8bbaf-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8bbaf-138">The following is an example of the response.</span></span>

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
  "description": "Delete trustFrameworkKeySet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


