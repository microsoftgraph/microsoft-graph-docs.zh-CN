---
title: 删除 claimsMappingPolicy
description: 从 servicePrincipal 中删除 claimsMappingPolicy。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: fed2bd63c3b944c6a32affbd3fc49edd994f0cd7
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051954"
---
# <a name="remove-claimsmappingpolicy"></a><span data-ttu-id="f759b-103">删除 claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="f759b-103">Remove claimsMappingPolicy</span></span>

<span data-ttu-id="f759b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f759b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f759b-105">从[servicePrincipal](../resources/servicePrincipal.md)中删除[claimsMappingPolicy。](../resources/claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f759b-105">Remove a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) from a [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f759b-106">权限</span><span class="sxs-lookup"><span data-stu-id="f759b-106">Permissions</span></span>

<span data-ttu-id="f759b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f759b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f759b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f759b-109">Permission type</span></span>                        | <span data-ttu-id="f759b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f759b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f759b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f759b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f759b-112">Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f759b-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span>  |
| <span data-ttu-id="f759b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f759b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f759b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f759b-114">Not supported.</span></span> |
| <span data-ttu-id="f759b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f759b-115">Application</span></span>                            | <span data-ttu-id="f759b-116">Policy.Read.All 和 Application.ReadWrite.OwnedBy、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.OwnedBy、Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f759b-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f759b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f759b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="f759b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f759b-118">Request headers</span></span>

| <span data-ttu-id="f759b-119">名称</span><span class="sxs-lookup"><span data-stu-id="f759b-119">Name</span></span>          | <span data-ttu-id="f759b-120">说明</span><span class="sxs-lookup"><span data-stu-id="f759b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f759b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f759b-121">Authorization</span></span> | <span data-ttu-id="f759b-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="f759b-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f759b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f759b-123">Request body</span></span>

<span data-ttu-id="f759b-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f759b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f759b-125">响应</span><span class="sxs-lookup"><span data-stu-id="f759b-125">Response</span></span>

<span data-ttu-id="f759b-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f759b-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f759b-127">示例</span><span class="sxs-lookup"><span data-stu-id="f759b-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f759b-128">请求</span><span class="sxs-lookup"><span data-stu-id="f759b-128">Request</span></span>

<span data-ttu-id="f759b-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f759b-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f759b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="f759b-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy_from_serviceprincipal"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/claimsMappingPolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="f759b-131">C#</span><span class="sxs-lookup"><span data-stu-id="f759b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f759b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f759b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f759b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f759b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f759b-134">Java</span><span class="sxs-lookup"><span data-stu-id="f759b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-from-serviceprincipal-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f759b-135">响应</span><span class="sxs-lookup"><span data-stu-id="f759b-135">Response</span></span>

<span data-ttu-id="f759b-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f759b-136">The following is an example of the response.</span></span>

> <span data-ttu-id="f759b-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f759b-137">**Note:** The response object shown here might be shortened for readability.</span></span>

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



