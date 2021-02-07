---
title: 删除 tokenIssuancePolicy
description: 从应用程序中删除 tokenIssuancePolicy。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: e71c6a8e7083b6119d720188e9cda2342cd75814
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131787"
---
# <a name="remove-tokenissuancepolicy"></a><span data-ttu-id="bb283-103">删除 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="bb283-103">Remove tokenIssuancePolicy</span></span>

<span data-ttu-id="bb283-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb283-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="bb283-105">从应用程序[中删除 tokenIssuancePolicy。](../resources/tokenissuancepolicy.md) [](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="bb283-105">Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bb283-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="bb283-106">Permissions</span></span>

<span data-ttu-id="bb283-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb283-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bb283-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb283-109">Permission type</span></span>                        | <span data-ttu-id="bb283-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb283-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="bb283-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb283-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="bb283-112">Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb283-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="bb283-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb283-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb283-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb283-114">Not supported.</span></span> |
| <span data-ttu-id="bb283-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb283-115">Application</span></span>                            | <span data-ttu-id="bb283-116">Policy.Read.All 和 Application.ReadWrite.OwnedBy、Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.OwnedBy、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb283-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb283-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb283-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="bb283-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb283-118">Request headers</span></span>

| <span data-ttu-id="bb283-119">名称</span><span class="sxs-lookup"><span data-stu-id="bb283-119">Name</span></span>          | <span data-ttu-id="bb283-120">说明</span><span class="sxs-lookup"><span data-stu-id="bb283-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="bb283-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb283-121">Authorization</span></span> | <span data-ttu-id="bb283-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bb283-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb283-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb283-124">Request body</span></span>

<span data-ttu-id="bb283-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb283-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb283-126">响应</span><span class="sxs-lookup"><span data-stu-id="bb283-126">Response</span></span>

<span data-ttu-id="bb283-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bb283-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="bb283-128">示例</span><span class="sxs-lookup"><span data-stu-id="bb283-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bb283-129">请求</span><span class="sxs-lookup"><span data-stu-id="bb283-129">Request</span></span>

<span data-ttu-id="bb283-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bb283-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="bb283-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb283-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/tokenIssuancePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="bb283-132">C#</span><span class="sxs-lookup"><span data-stu-id="bb283-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenissuancepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb283-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb283-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenissuancepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb283-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb283-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenissuancepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bb283-135">Java</span><span class="sxs-lookup"><span data-stu-id="bb283-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenissuancepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bb283-136">响应</span><span class="sxs-lookup"><span data-stu-id="bb283-136">Response</span></span>

<span data-ttu-id="bb283-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bb283-137">The following is an example of the response.</span></span>

> <span data-ttu-id="bb283-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bb283-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

