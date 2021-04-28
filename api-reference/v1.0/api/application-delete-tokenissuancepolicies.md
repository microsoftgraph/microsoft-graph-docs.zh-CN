---
title: 删除 tokenIssuancePolicy
description: 从应用程序中删除 tokenIssuancePolicy。
localization_priority: Normal
author: sureshja
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ff9761354f1d47e1cfafcf144fea8cb1f1e912e2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050617"
---
# <a name="remove-tokenissuancepolicy"></a><span data-ttu-id="36bc2-103">删除 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="36bc2-103">Remove tokenIssuancePolicy</span></span>

<span data-ttu-id="36bc2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36bc2-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="36bc2-105">从应用程序[中删除 tokenIssuancePolicy。](../resources/tokenissuancepolicy.md) [](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="36bc2-105">Remove a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) from an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="36bc2-106">权限</span><span class="sxs-lookup"><span data-stu-id="36bc2-106">Permissions</span></span>

<span data-ttu-id="36bc2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="36bc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="36bc2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="36bc2-109">Permission type</span></span>                        | <span data-ttu-id="36bc2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="36bc2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="36bc2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="36bc2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="36bc2-112">Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36bc2-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="36bc2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="36bc2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36bc2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="36bc2-114">Not supported.</span></span> |
| <span data-ttu-id="36bc2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="36bc2-115">Application</span></span>                            | <span data-ttu-id="36bc2-116">Policy.Read.All 和 Application.ReadWrite.OwnedBy、Policy.Read.All 和 Application.ReadWrite.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.OwnedBy、Policy.ReadWrite.ApplicationConfiguration 和 Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="36bc2-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="36bc2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="36bc2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /applications/{id}/tokenIssuancePolicies/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="36bc2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="36bc2-118">Request headers</span></span>

| <span data-ttu-id="36bc2-119">名称</span><span class="sxs-lookup"><span data-stu-id="36bc2-119">Name</span></span>          | <span data-ttu-id="36bc2-120">说明</span><span class="sxs-lookup"><span data-stu-id="36bc2-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="36bc2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="36bc2-121">Authorization</span></span> | <span data-ttu-id="36bc2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="36bc2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="36bc2-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="36bc2-124">Request body</span></span>

<span data-ttu-id="36bc2-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="36bc2-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36bc2-126">响应</span><span class="sxs-lookup"><span data-stu-id="36bc2-126">Response</span></span>

<span data-ttu-id="36bc2-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="36bc2-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="36bc2-128">示例</span><span class="sxs-lookup"><span data-stu-id="36bc2-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="36bc2-129">请求</span><span class="sxs-lookup"><span data-stu-id="36bc2-129">Request</span></span>

<span data-ttu-id="36bc2-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="36bc2-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="36bc2-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="36bc2-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tokenissuancepolicy_from_application"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/applications/{id}/tokenIssuancePolicies/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="36bc2-132">C#</span><span class="sxs-lookup"><span data-stu-id="36bc2-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tokenissuancepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="36bc2-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="36bc2-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tokenissuancepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="36bc2-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="36bc2-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tokenissuancepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="36bc2-135">Java</span><span class="sxs-lookup"><span data-stu-id="36bc2-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tokenissuancepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="36bc2-136">响应</span><span class="sxs-lookup"><span data-stu-id="36bc2-136">Response</span></span>

<span data-ttu-id="36bc2-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="36bc2-137">The following is an example of the response.</span></span>

> <span data-ttu-id="36bc2-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="36bc2-138">**Note:** The response object shown here might be shortened for readability.</span></span>

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

