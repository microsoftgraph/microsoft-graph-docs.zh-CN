---
title: 删除 claimsMappingPolicy
description: 从 servicePrincipal 中删除 claimsMappingPolicy。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cd159f8efd7cf0789be143034f5edce073d23398
ms.sourcegitcommit: 24092bd1e38e8adfd314dfe8dfea9b24a5c21da6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2020
ms.locfileid: "43581663"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="7be06-103">删除 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="7be06-103">Remove claimsMappingPolicy</span></span>

<span data-ttu-id="7be06-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7be06-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7be06-105">从[servicePrincipal](../resources/servicePrincipal.md)中删除[claimsMappingPolicy](../resources/claimsmappingpolicy.md) 。</span><span class="sxs-lookup"><span data-stu-id="7be06-105">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7be06-106">权限</span><span class="sxs-lookup"><span data-stu-id="7be06-106">Permissions</span></span>

<span data-ttu-id="7be06-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7be06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7be06-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7be06-109">Permission type</span></span>                        | <span data-ttu-id="7be06-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7be06-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7be06-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7be06-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7be06-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="7be06-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="7be06-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7be06-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7be06-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7be06-114">Not supported.</span></span> |
| <span data-ttu-id="7be06-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7be06-115">Application</span></span>                            | <span data-ttu-id="7be06-116">Application.readwrite.ownedby、ApplicationConfiguration 和应用程序的 Application.readwrite.ownedby、、ApplicationConfiguration 和应用程序的、和。 all，all。和和应用程序的所有写读。</span><span class="sxs-lookup"><span data-stu-id="7be06-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7be06-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7be06-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="7be06-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7be06-118">Request headers</span></span>

| <span data-ttu-id="7be06-119">名称</span><span class="sxs-lookup"><span data-stu-id="7be06-119">Name</span></span>          | <span data-ttu-id="7be06-120">说明</span><span class="sxs-lookup"><span data-stu-id="7be06-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7be06-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7be06-121">Authorization</span></span> | <span data-ttu-id="7be06-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7be06-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7be06-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7be06-123">Request body</span></span>

<span data-ttu-id="7be06-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7be06-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7be06-125">响应</span><span class="sxs-lookup"><span data-stu-id="7be06-125">Response</span></span>

<span data-ttu-id="7be06-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7be06-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7be06-127">示例</span><span class="sxs-lookup"><span data-stu-id="7be06-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7be06-128">请求</span><span class="sxs-lookup"><span data-stu-id="7be06-128">Request</span></span>

<span data-ttu-id="7be06-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7be06-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7be06-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="7be06-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="7be06-131">C#</span><span class="sxs-lookup"><span data-stu-id="7be06-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7be06-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7be06-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7be06-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7be06-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7be06-134">响应</span><span class="sxs-lookup"><span data-stu-id="7be06-134">Response</span></span>

<span data-ttu-id="7be06-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7be06-135">The following is an example of the response.</span></span>

> <span data-ttu-id="7be06-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7be06-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
