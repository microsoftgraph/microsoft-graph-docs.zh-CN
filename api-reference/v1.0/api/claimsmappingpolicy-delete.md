---
title: 删除 claimsMappingPolicy
description: 删除 claimsMappingPolicy。
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 036865e9ab85407dd000c40252837de46be9fd52
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50432954"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="034aa-103">删除 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="034aa-103">Delete claimsMappingPolicy</span></span>

<span data-ttu-id="034aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="034aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="034aa-105">删除 [claimsMappingPolicy](../resources/claimsmappingpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="034aa-105">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="034aa-106">权限</span><span class="sxs-lookup"><span data-stu-id="034aa-106">Permissions</span></span>

<span data-ttu-id="034aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="034aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="034aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="034aa-109">Permission type</span></span>                        | <span data-ttu-id="034aa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="034aa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="034aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="034aa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="034aa-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="034aa-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="034aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="034aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="034aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="034aa-114">Not supported.</span></span> |
| <span data-ttu-id="034aa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="034aa-115">Application</span></span>                            | <span data-ttu-id="034aa-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="034aa-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="034aa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="034aa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="034aa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="034aa-118">Request headers</span></span>

| <span data-ttu-id="034aa-119">名称</span><span class="sxs-lookup"><span data-stu-id="034aa-119">Name</span></span>          | <span data-ttu-id="034aa-120">说明</span><span class="sxs-lookup"><span data-stu-id="034aa-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="034aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="034aa-121">Authorization</span></span> | <span data-ttu-id="034aa-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="034aa-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="034aa-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="034aa-123">Request body</span></span>

<span data-ttu-id="034aa-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="034aa-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="034aa-125">响应</span><span class="sxs-lookup"><span data-stu-id="034aa-125">Response</span></span>

<span data-ttu-id="034aa-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="034aa-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="034aa-127">示例</span><span class="sxs-lookup"><span data-stu-id="034aa-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="034aa-128">请求</span><span class="sxs-lookup"><span data-stu-id="034aa-128">Request</span></span>

<span data-ttu-id="034aa-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="034aa-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="034aa-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="034aa-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="034aa-131">C#</span><span class="sxs-lookup"><span data-stu-id="034aa-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="034aa-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="034aa-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="034aa-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="034aa-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="034aa-134">Java</span><span class="sxs-lookup"><span data-stu-id="034aa-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="034aa-135">响应</span><span class="sxs-lookup"><span data-stu-id="034aa-135">Response</span></span>

<span data-ttu-id="034aa-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="034aa-136">The following is an example of the response.</span></span>

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
  "description": "Delete claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

