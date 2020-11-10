---
title: 分配 tokenLifetimePolicy
description: 将 tokenLifetimePolicy 分配给应用程序或服务主体。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bfc07539e8f110f4a73a40bedb0a1c2ea635ef46
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961883"
---
# <a name="assign-tokenlifetimepolicy"></a><span data-ttu-id="025cc-103">分配 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="025cc-103">Assign tokenLifetimePolicy</span></span>

<span data-ttu-id="025cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="025cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="025cc-105">将 [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 分配给 [应用程序](../resources/application.md) 或 [servicePrincipal](../resources/servicePrincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="025cc-105">Assign a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="025cc-106">权限</span><span class="sxs-lookup"><span data-stu-id="025cc-106">Permissions</span></span>

<span data-ttu-id="025cc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="025cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="025cc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="025cc-109">Permission type</span></span>                        | <span data-ttu-id="025cc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="025cc-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="025cc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="025cc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="025cc-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="025cc-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="025cc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="025cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="025cc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="025cc-114">Not supported.</span></span> |
| <span data-ttu-id="025cc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="025cc-115">Application</span></span>                            | <span data-ttu-id="025cc-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="025cc-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="025cc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="025cc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
POST /servicePrincipals/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="025cc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="025cc-118">Request headers</span></span>

| <span data-ttu-id="025cc-119">名称</span><span class="sxs-lookup"><span data-stu-id="025cc-119">Name</span></span>          | <span data-ttu-id="025cc-120">说明</span><span class="sxs-lookup"><span data-stu-id="025cc-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="025cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="025cc-121">Authorization</span></span> | <span data-ttu-id="025cc-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="025cc-122">Bearer {token}</span></span> |
| <span data-ttu-id="025cc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="025cc-123">Content-Type</span></span> | <span data-ttu-id="025cc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="025cc-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="025cc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="025cc-125">Request body</span></span>

<span data-ttu-id="025cc-126">在请求正文中，提供 [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) 对象的标识符 (使用 `@odata.id` 应分配给应用程序或服务主体的属性) 。</span><span class="sxs-lookup"><span data-stu-id="025cc-126">In the request body, supply the identifier of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object (using an `@odata.id` property) that should be assigned to the application or service principal.</span></span>

## <a name="response"></a><span data-ttu-id="025cc-127">响应</span><span class="sxs-lookup"><span data-stu-id="025cc-127">Response</span></span>

<span data-ttu-id="025cc-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="025cc-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="025cc-130">示例</span><span class="sxs-lookup"><span data-stu-id="025cc-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="025cc-131">请求</span><span class="sxs-lookup"><span data-stu-id="025cc-131">Request</span></span>

<span data-ttu-id="025cc-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="025cc-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="025cc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="025cc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
}
```
# <a name="javascript"></a>[<span data-ttu-id="025cc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="025cc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="025cc-135">C#</span><span class="sxs-lookup"><span data-stu-id="025cc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="025cc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="025cc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="025cc-137">Java</span><span class="sxs-lookup"><span data-stu-id="025cc-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-tokenlifetimepolicy-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="025cc-138">响应</span><span class="sxs-lookup"><span data-stu-id="025cc-138">Response</span></span>

<span data-ttu-id="025cc-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="025cc-139">The following is an example of the response.</span></span>

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
  "description": "Assign tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


