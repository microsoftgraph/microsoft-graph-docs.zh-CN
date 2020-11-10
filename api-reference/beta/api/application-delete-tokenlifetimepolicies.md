---
title: 删除 tokenLifetimePolicy
description: 从应用程序或 servicePrincipal 中删除 tokenLifetimePolicy。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 73d4b89f8de917937a957dcc6459fe2971342783
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962226"
---
# <a name="remove-tokenlifetimepolicy"></a><span data-ttu-id="d0e2f-103">删除 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="d0e2f-103">Remove tokenLifetimePolicy</span></span>

<span data-ttu-id="d0e2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0e2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0e2f-105">从[应用程序](../resources/application.md)或[ServicePrincipal](../resources/servicePrincipal.md)中删除[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 。</span><span class="sxs-lookup"><span data-stu-id="d0e2f-105">Remove a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) from an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d0e2f-106">权限</span><span class="sxs-lookup"><span data-stu-id="d0e2f-106">Permissions</span></span>

<span data-ttu-id="d0e2f-107">若要调用此 API，需要以下权限集之一。</span><span class="sxs-lookup"><span data-stu-id="d0e2f-107">One of the following sets of permissions is required to call this API.</span></span> <span data-ttu-id="d0e2f-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0e2f-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d0e2f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0e2f-109">Permission type</span></span>                        | <span data-ttu-id="d0e2f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0e2f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d0e2f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0e2f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d0e2f-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="d0e2f-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="d0e2f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0e2f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0e2f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0e2f-114">Not supported.</span></span> |
| <span data-ttu-id="d0e2f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0e2f-115">Application</span></span>                            | <span data-ttu-id="d0e2f-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="d0e2f-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0e2f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0e2f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenLifetimePolicies/{id}/$ref
DELETE /servicePrincipals/{id}/tokenLifetimePolicies/{id}$ref
```

## <a name="request-headers"></a><span data-ttu-id="d0e2f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0e2f-118">Request headers</span></span>

| <span data-ttu-id="d0e2f-119">名称</span><span class="sxs-lookup"><span data-stu-id="d0e2f-119">Name</span></span>          | <span data-ttu-id="d0e2f-120">说明</span><span class="sxs-lookup"><span data-stu-id="d0e2f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d0e2f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0e2f-121">Authorization</span></span> | <span data-ttu-id="d0e2f-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d0e2f-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0e2f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0e2f-123">Request body</span></span>

<span data-ttu-id="d0e2f-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0e2f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0e2f-125">响应</span><span class="sxs-lookup"><span data-stu-id="d0e2f-125">Response</span></span>

<span data-ttu-id="d0e2f-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d0e2f-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="d0e2f-127">示例</span><span class="sxs-lookup"><span data-stu-id="d0e2f-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d0e2f-128">请求</span><span class="sxs-lookup"><span data-stu-id="d0e2f-128">Request</span></span>

<span data-ttu-id="d0e2f-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d0e2f-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d0e2f-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0e2f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenlifetimepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="d0e2f-131">C#</span><span class="sxs-lookup"><span data-stu-id="d0e2f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0e2f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0e2f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0e2f-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0e2f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0e2f-134">Java</span><span class="sxs-lookup"><span data-stu-id="d0e2f-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenlifetimepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d0e2f-135">响应</span><span class="sxs-lookup"><span data-stu-id="d0e2f-135">Response</span></span>

<span data-ttu-id="d0e2f-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d0e2f-136">The following is an example of the response.</span></span>

> <span data-ttu-id="d0e2f-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d0e2f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "Remove tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


