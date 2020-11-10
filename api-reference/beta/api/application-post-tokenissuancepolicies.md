---
title: 分配 tokenIssuancePolicy
description: 将 tokenIssuancePolicy 分配给应用程序。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 441ff3f0371520b08aab3f3465d20b75aba7753d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961904"
---
# <a name="assign-tokenissuancepolicy"></a><span data-ttu-id="6de86-103">分配 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="6de86-103">Assign tokenIssuancePolicy</span></span>

<span data-ttu-id="6de86-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6de86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6de86-105">将 [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) 分配给 [应用程序](../resources/application.md)。</span><span class="sxs-lookup"><span data-stu-id="6de86-105">Assign a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6de86-106">权限</span><span class="sxs-lookup"><span data-stu-id="6de86-106">Permissions</span></span>

<span data-ttu-id="6de86-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6de86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6de86-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6de86-109">Permission type</span></span>                        | <span data-ttu-id="6de86-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6de86-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6de86-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6de86-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6de86-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="6de86-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="6de86-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6de86-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6de86-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6de86-114">Not supported.</span></span> |
| <span data-ttu-id="6de86-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6de86-115">Application</span></span>                            | <span data-ttu-id="6de86-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="6de86-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6de86-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6de86-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenIssuancePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6de86-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6de86-118">Request headers</span></span>

| <span data-ttu-id="6de86-119">名称</span><span class="sxs-lookup"><span data-stu-id="6de86-119">Name</span></span>          | <span data-ttu-id="6de86-120">说明</span><span class="sxs-lookup"><span data-stu-id="6de86-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6de86-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6de86-121">Authorization</span></span> | <span data-ttu-id="6de86-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6de86-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6de86-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6de86-124">Content-Type</span></span> | <span data-ttu-id="6de86-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6de86-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6de86-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6de86-127">Request body</span></span>

<span data-ttu-id="6de86-128">在请求正文中，使用[tokenIssuancePolicy](../resources/tokenissuancepolicy.md) `@odata.id` 应分配给应用程序的属性) 提供 tokenIssuancePolicy 对象 (的标识符。</span><span class="sxs-lookup"><span data-stu-id="6de86-128">In the request body, supply the identifier of the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object (using an `@odata.id` property) that should be assigned to the application.</span></span>

## <a name="response"></a><span data-ttu-id="6de86-129">响应</span><span class="sxs-lookup"><span data-stu-id="6de86-129">Response</span></span>

<span data-ttu-id="6de86-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6de86-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6de86-132">示例</span><span class="sxs-lookup"><span data-stu-id="6de86-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6de86-133">请求</span><span class="sxs-lookup"><span data-stu-id="6de86-133">Request</span></span>

<span data-ttu-id="6de86-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6de86-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6de86-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6de86-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenissuancepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies/$ref
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="c"></a>[<span data-ttu-id="6de86-136">C#</span><span class="sxs-lookup"><span data-stu-id="6de86-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenissuancepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6de86-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6de86-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenissuancepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6de86-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6de86-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenissuancepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6de86-139">Java</span><span class="sxs-lookup"><span data-stu-id="6de86-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenissuancepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6de86-140">响应</span><span class="sxs-lookup"><span data-stu-id="6de86-140">Response</span></span>

<span data-ttu-id="6de86-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6de86-141">The following is an example of the response.</span></span>

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
  "description": "Assign tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


