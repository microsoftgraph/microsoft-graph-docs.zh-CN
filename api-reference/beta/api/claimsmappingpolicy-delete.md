---
title: 删除 claimsMappingPolicy
description: 删除 claimsMappingPolicy。
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4f1075d4f9cdd2ac8f9635566fbccc3d49921d80
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916684"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="62468-103">删除 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="62468-103">Delete claimsMappingPolicy</span></span>

<span data-ttu-id="62468-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62468-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62468-105">删除[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="62468-105">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="62468-106">权限</span><span class="sxs-lookup"><span data-stu-id="62468-106">Permissions</span></span>

<span data-ttu-id="62468-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62468-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="62468-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="62468-109">Permission type</span></span>                        | <span data-ttu-id="62468-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="62468-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="62468-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62468-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="62468-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="62468-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="62468-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62468-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="62468-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="62468-114">Not supported.</span></span> |
| <span data-ttu-id="62468-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="62468-115">Application</span></span>                            | <span data-ttu-id="62468-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="62468-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="62468-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62468-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="62468-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="62468-118">Request headers</span></span>

| <span data-ttu-id="62468-119">名称</span><span class="sxs-lookup"><span data-stu-id="62468-119">Name</span></span>          | <span data-ttu-id="62468-120">说明</span><span class="sxs-lookup"><span data-stu-id="62468-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="62468-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="62468-121">Authorization</span></span> | <span data-ttu-id="62468-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="62468-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="62468-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="62468-123">Request body</span></span>

<span data-ttu-id="62468-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="62468-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="62468-125">响应</span><span class="sxs-lookup"><span data-stu-id="62468-125">Response</span></span>

<span data-ttu-id="62468-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="62468-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="62468-127">示例</span><span class="sxs-lookup"><span data-stu-id="62468-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="62468-128">请求</span><span class="sxs-lookup"><span data-stu-id="62468-128">Request</span></span>

<span data-ttu-id="62468-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="62468-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="62468-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="62468-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="62468-131">C#</span><span class="sxs-lookup"><span data-stu-id="62468-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="62468-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="62468-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="62468-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="62468-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="62468-134">响应</span><span class="sxs-lookup"><span data-stu-id="62468-134">Response</span></span>

<span data-ttu-id="62468-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="62468-135">The following is an example of the response.</span></span>

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
