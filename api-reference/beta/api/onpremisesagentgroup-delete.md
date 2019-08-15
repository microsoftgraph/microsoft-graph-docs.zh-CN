---
title: 删除 onPremisesAgentGroup
description: 删除**onPremisesAgentGroup**对象。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3e6a78a79c2eab50cdf035d2c17c4d11637e74b4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414532"
---
# <a name="delete-onpremisesagentgroup"></a><span data-ttu-id="fb915-103">删除 onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="fb915-103">Delete onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb915-104">删除[onPremisesAgentGroup](../resources/onpremisesagentgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fb915-104">Delete an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb915-105">权限</span><span class="sxs-lookup"><span data-stu-id="fb915-105">Permissions</span></span>

<span data-ttu-id="fb915-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fb915-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb915-108">Permission type</span></span>                        | <span data-ttu-id="fb915-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fb915-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb915-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb915-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="fb915-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="fb915-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="fb915-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb915-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb915-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb915-113">Not supported.</span></span> |
| <span data-ttu-id="fb915-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb915-114">Application</span></span>                            | <span data-ttu-id="fb915-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb915-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb915-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb915-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id1}
```

## <a name="request-headers"></a><span data-ttu-id="fb915-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb915-117">Request headers</span></span>

| <span data-ttu-id="fb915-118">名称</span><span class="sxs-lookup"><span data-stu-id="fb915-118">Name</span></span>          | <span data-ttu-id="fb915-119">说明</span><span class="sxs-lookup"><span data-stu-id="fb915-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fb915-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb915-120">Authorization</span></span> | <span data-ttu-id="fb915-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="fb915-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fb915-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb915-122">Request body</span></span>

<span data-ttu-id="fb915-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fb915-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fb915-124">响应</span><span class="sxs-lookup"><span data-stu-id="fb915-124">Response</span></span>

<span data-ttu-id="fb915-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fb915-p102">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb915-127">示例</span><span class="sxs-lookup"><span data-stu-id="fb915-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb915-128">请求</span><span class="sxs-lookup"><span data-stu-id="fb915-128">Request</span></span>

<span data-ttu-id="fb915-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fb915-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fb915-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fb915-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_onpremisesagentgroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fb915-131">C#</span><span class="sxs-lookup"><span data-stu-id="fb915-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-onpremisesagentgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fb915-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb915-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fb915-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="fb915-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fb915-134">响应</span><span class="sxs-lookup"><span data-stu-id="fb915-134">Response</span></span>

<span data-ttu-id="fb915-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fb915-135">The following is an example of the response.</span></span>

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
  "description": "Delete onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
