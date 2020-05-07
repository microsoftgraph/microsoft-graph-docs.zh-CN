---
title: 删除 workforceIntegration
description: 删除 workforceIntegration 的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ff8bf2197232110fea356f951d62aa5a511e3f50
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154106"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="877df-103">删除 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="877df-103">Delete workforceIntegration</span></span>

<span data-ttu-id="877df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="877df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="877df-105">删除[workforceIntegration](../resources/workforceintegration.md)的实例。</span><span class="sxs-lookup"><span data-stu-id="877df-105">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="877df-106">权限</span><span class="sxs-lookup"><span data-stu-id="877df-106">Permissions</span></span>

<span data-ttu-id="877df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="877df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="877df-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="877df-109">Permission type</span></span>                        | <span data-ttu-id="877df-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="877df-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="877df-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="877df-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="877df-112">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="877df-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="877df-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="877df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="877df-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="877df-114">Not supported.</span></span> |
| <span data-ttu-id="877df-115">Application</span><span class="sxs-lookup"><span data-stu-id="877df-115">Application</span></span>                            | <span data-ttu-id="877df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="877df-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="877df-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="877df-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="877df-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="877df-118">Request headers</span></span>

| <span data-ttu-id="877df-119">名称</span><span class="sxs-lookup"><span data-stu-id="877df-119">Name</span></span>          | <span data-ttu-id="877df-120">说明</span><span class="sxs-lookup"><span data-stu-id="877df-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="877df-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="877df-121">Authorization</span></span> | <span data-ttu-id="877df-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="877df-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="877df-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="877df-123">Request body</span></span>

<span data-ttu-id="877df-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="877df-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="877df-125">响应</span><span class="sxs-lookup"><span data-stu-id="877df-125">Response</span></span>

<span data-ttu-id="877df-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="877df-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="877df-128">示例</span><span class="sxs-lookup"><span data-stu-id="877df-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="877df-129">请求</span><span class="sxs-lookup"><span data-stu-id="877df-129">Request</span></span>

<span data-ttu-id="877df-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="877df-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="877df-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="877df-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceIntegrationId}
```
# <a name="c"></a>[<span data-ttu-id="877df-132">C#</span><span class="sxs-lookup"><span data-stu-id="877df-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="877df-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="877df-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="877df-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="877df-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="877df-135">响应</span><span class="sxs-lookup"><span data-stu-id="877df-135">Response</span></span>

<span data-ttu-id="877df-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="877df-136">The following is an example of the response.</span></span>

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
  "description": "Delete workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
