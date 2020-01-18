---
title: 分配 tokenLifetimePolicy
description: 将 tokenLifetimePolicy 分配给应用程序或服务主体。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5c68600b713d220468853bf56eaa6a136b647f8a
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234144"
---
# <a name="assign-tokenlifetimepolicy"></a><span data-ttu-id="c1ffc-103">分配 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="c1ffc-103">Assign tokenLifetimePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1ffc-104">将[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)分配给[应用程序](../resources/application.md)或[servicePrincipal](../resources/servicePrincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="c1ffc-104">Assign a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) to an [application](../resources/application.md) or [servicePrincipal](../resources/servicePrincipal.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1ffc-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="c1ffc-105">Permissions</span></span>

<span data-ttu-id="c1ffc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1ffc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c1ffc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1ffc-108">Permission type</span></span>                        | <span data-ttu-id="c1ffc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1ffc-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c1ffc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1ffc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c1ffc-111">Policy. All 和 Application。所有读写。</span><span class="sxs-lookup"><span data-stu-id="c1ffc-111">Policy.Read.All and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="c1ffc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1ffc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1ffc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1ffc-113">Not supported.</span></span> |
| <span data-ttu-id="c1ffc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1ffc-114">Application</span></span>                            | <span data-ttu-id="c1ffc-115">Policy. All 和 Application.readwrite.ownedby，all 和应用程序的 Read. all</span><span class="sxs-lookup"><span data-stu-id="c1ffc-115">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1ffc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1ffc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
POST /servicePrincipals/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c1ffc-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1ffc-117">Request headers</span></span>

| <span data-ttu-id="c1ffc-118">名称</span><span class="sxs-lookup"><span data-stu-id="c1ffc-118">Name</span></span>          | <span data-ttu-id="c1ffc-119">说明</span><span class="sxs-lookup"><span data-stu-id="c1ffc-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c1ffc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1ffc-120">Authorization</span></span> | <span data-ttu-id="c1ffc-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="c1ffc-121">Bearer {token}</span></span> |
| <span data-ttu-id="c1ffc-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c1ffc-122">Content-Type</span></span> | <span data-ttu-id="c1ffc-123">application/json</span><span class="sxs-lookup"><span data-stu-id="c1ffc-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1ffc-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1ffc-124">Request body</span></span>

<span data-ttu-id="c1ffc-125">在请求正文中，提供应分配给应用[](../resources/tokenlifetimepolicy.md)程序或服务主体的`@odata.id` tokenLifetimePolicy 对象的标识符（使用属性）。</span><span class="sxs-lookup"><span data-stu-id="c1ffc-125">In the request body, supply the identifier of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object (using an `@odata.id` property) that should be assigned to the application or service principal.</span></span>

## <a name="response"></a><span data-ttu-id="c1ffc-126">响应</span><span class="sxs-lookup"><span data-stu-id="c1ffc-126">Response</span></span>

<span data-ttu-id="c1ffc-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c1ffc-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c1ffc-129">示例</span><span class="sxs-lookup"><span data-stu-id="c1ffc-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c1ffc-130">请求</span><span class="sxs-lookup"><span data-stu-id="c1ffc-130">Request</span></span>

<span data-ttu-id="c1ffc-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1ffc-131">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c1ffc-132">响应</span><span class="sxs-lookup"><span data-stu-id="c1ffc-132">Response</span></span>

<span data-ttu-id="c1ffc-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1ffc-133">The following is an example of the response.</span></span>

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