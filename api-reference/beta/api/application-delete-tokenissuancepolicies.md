---
title: 删除 tokenIssuancePolicy
description: 从应用程序中删除 tokenIssuancePolicy。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b40d3045690920e0e00bfa9543aa17263e804ede
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48962239"
---
# <a name="remove-tokenissuancepolicy"></a><span data-ttu-id="df385-103">删除 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="df385-103">Remove tokenIssuancePolicy</span></span>

<span data-ttu-id="df385-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df385-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df385-105">从[应用程序](../resources/application.md)中删除[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) 。</span><span class="sxs-lookup"><span data-stu-id="df385-105">Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df385-106">权限</span><span class="sxs-lookup"><span data-stu-id="df385-106">Permissions</span></span>

<span data-ttu-id="df385-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df385-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="df385-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="df385-109">Permission type</span></span>                        | <span data-ttu-id="df385-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df385-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="df385-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df385-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="df385-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="df385-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="df385-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df385-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df385-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="df385-114">Not supported.</span></span> |
| <span data-ttu-id="df385-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="df385-115">Application</span></span>                            | <span data-ttu-id="df385-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="df385-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="df385-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df385-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="df385-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="df385-118">Request headers</span></span>

| <span data-ttu-id="df385-119">名称</span><span class="sxs-lookup"><span data-stu-id="df385-119">Name</span></span>          | <span data-ttu-id="df385-120">说明</span><span class="sxs-lookup"><span data-stu-id="df385-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="df385-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="df385-121">Authorization</span></span> | <span data-ttu-id="df385-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df385-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="df385-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="df385-124">Request body</span></span>

<span data-ttu-id="df385-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="df385-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df385-126">响应</span><span class="sxs-lookup"><span data-stu-id="df385-126">Response</span></span>

<span data-ttu-id="df385-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="df385-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="df385-128">示例</span><span class="sxs-lookup"><span data-stu-id="df385-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df385-129">请求</span><span class="sxs-lookup"><span data-stu-id="df385-129">Request</span></span>

<span data-ttu-id="df385-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="df385-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="df385-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="df385-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="df385-132">C#</span><span class="sxs-lookup"><span data-stu-id="df385-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenissuancepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df385-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df385-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenissuancepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df385-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df385-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenissuancepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df385-135">Java</span><span class="sxs-lookup"><span data-stu-id="df385-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenissuancepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df385-136">响应</span><span class="sxs-lookup"><span data-stu-id="df385-136">Response</span></span>

<span data-ttu-id="df385-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="df385-137">The following is an example of the response.</span></span>

> <span data-ttu-id="df385-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="df385-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


