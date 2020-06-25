---
title: 删除 claimsMappingPolicy
description: 删除 claimsMappingPolicy。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5749effbb234444cf3ba609df58a0af598c9b204
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863826"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="04214-103">删除 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="04214-103">Delete claimsMappingPolicy</span></span>

<span data-ttu-id="04214-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04214-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="04214-105">删除[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="04214-105">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="04214-106">权限</span><span class="sxs-lookup"><span data-stu-id="04214-106">Permissions</span></span>

<span data-ttu-id="04214-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="04214-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="04214-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04214-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04214-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="04214-109">Permission type</span></span>                        | <span data-ttu-id="04214-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04214-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="04214-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04214-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="04214-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="04214-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="04214-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04214-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04214-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="04214-114">Not supported.</span></span> |
| <span data-ttu-id="04214-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="04214-115">Application</span></span>                            | <span data-ttu-id="04214-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="04214-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="04214-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04214-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="04214-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="04214-118">Request headers</span></span>

| <span data-ttu-id="04214-119">名称</span><span class="sxs-lookup"><span data-stu-id="04214-119">Name</span></span>          | <span data-ttu-id="04214-120">说明</span><span class="sxs-lookup"><span data-stu-id="04214-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="04214-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="04214-121">Authorization</span></span> | <span data-ttu-id="04214-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="04214-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="04214-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="04214-123">Request body</span></span>

<span data-ttu-id="04214-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="04214-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04214-125">响应</span><span class="sxs-lookup"><span data-stu-id="04214-125">Response</span></span>

<span data-ttu-id="04214-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="04214-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="04214-127">示例</span><span class="sxs-lookup"><span data-stu-id="04214-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04214-128">请求</span><span class="sxs-lookup"><span data-stu-id="04214-128">Request</span></span>

<span data-ttu-id="04214-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="04214-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="04214-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="04214-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="04214-131">C#</span><span class="sxs-lookup"><span data-stu-id="04214-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="04214-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04214-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="04214-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="04214-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="04214-134">Java</span><span class="sxs-lookup"><span data-stu-id="04214-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="04214-135">响应</span><span class="sxs-lookup"><span data-stu-id="04214-135">Response</span></span>

<span data-ttu-id="04214-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="04214-136">The following is an example of the response.</span></span>

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
