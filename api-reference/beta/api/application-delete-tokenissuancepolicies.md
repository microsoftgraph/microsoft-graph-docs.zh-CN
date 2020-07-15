---
title: 删除 tokenIssuancePolicy
description: 从应用程序中删除 tokenIssuancePolicy。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64d3a74ff0397a35b1cefa7943186918ecc0c23f
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142228"
---
# <a name="remove-tokenissuancepolicy"></a><span data-ttu-id="4700e-103">删除 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="4700e-103">Remove tokenIssuancePolicy</span></span>

<span data-ttu-id="4700e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4700e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4700e-105">从[应用程序](../resources/application.md)中删除[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) 。</span><span class="sxs-lookup"><span data-stu-id="4700e-105">Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4700e-106">权限</span><span class="sxs-lookup"><span data-stu-id="4700e-106">Permissions</span></span>

<span data-ttu-id="4700e-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4700e-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4700e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4700e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4700e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4700e-109">Permission type</span></span>                        | <span data-ttu-id="4700e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4700e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4700e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4700e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4700e-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="4700e-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="4700e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4700e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4700e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4700e-114">Not supported.</span></span> |
| <span data-ttu-id="4700e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4700e-115">Application</span></span>                            | <span data-ttu-id="4700e-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="4700e-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4700e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4700e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4700e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4700e-118">Request headers</span></span>

| <span data-ttu-id="4700e-119">名称</span><span class="sxs-lookup"><span data-stu-id="4700e-119">Name</span></span>          | <span data-ttu-id="4700e-120">说明</span><span class="sxs-lookup"><span data-stu-id="4700e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4700e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4700e-121">Authorization</span></span> | <span data-ttu-id="4700e-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="4700e-122">Bearer {token}.</span></span> <span data-ttu-id="4700e-123">Required.</span><span class="sxs-lookup"><span data-stu-id="4700e-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4700e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="4700e-124">Request body</span></span>

<span data-ttu-id="4700e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4700e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4700e-126">响应</span><span class="sxs-lookup"><span data-stu-id="4700e-126">Response</span></span>

<span data-ttu-id="4700e-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4700e-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4700e-128">示例</span><span class="sxs-lookup"><span data-stu-id="4700e-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4700e-129">请求</span><span class="sxs-lookup"><span data-stu-id="4700e-129">Request</span></span>

<span data-ttu-id="4700e-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4700e-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4700e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4700e-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="4700e-132">C#</span><span class="sxs-lookup"><span data-stu-id="4700e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenissuancepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4700e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4700e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenissuancepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4700e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4700e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenissuancepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4700e-135">响应</span><span class="sxs-lookup"><span data-stu-id="4700e-135">Response</span></span>

<span data-ttu-id="4700e-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4700e-136">The following is an example of the response.</span></span>

> <span data-ttu-id="4700e-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="4700e-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4700e-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="4700e-138">All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
