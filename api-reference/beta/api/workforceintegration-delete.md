---
title: 删除 workforceIntegration
description: 删除 workforceIntegration 的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bb9d7a4259f4420971b9341e01acedd9da7049f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451281"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="85b5b-103">删除 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="85b5b-103">Delete workforceIntegration</span></span>

<span data-ttu-id="85b5b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="85b5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85b5b-105">删除[workforceIntegration](../resources/workforceintegration.md)的实例。</span><span class="sxs-lookup"><span data-stu-id="85b5b-105">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="85b5b-106">权限</span><span class="sxs-lookup"><span data-stu-id="85b5b-106">Permissions</span></span>

<span data-ttu-id="85b5b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85b5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85b5b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="85b5b-109">Permission type</span></span>                        | <span data-ttu-id="85b5b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85b5b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="85b5b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85b5b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="85b5b-112">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="85b5b-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="85b5b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85b5b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85b5b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="85b5b-114">Not supported.</span></span> |
| <span data-ttu-id="85b5b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="85b5b-115">Application</span></span>                            | <span data-ttu-id="85b5b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="85b5b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85b5b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85b5b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="85b5b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="85b5b-118">Request headers</span></span>

| <span data-ttu-id="85b5b-119">名称</span><span class="sxs-lookup"><span data-stu-id="85b5b-119">Name</span></span>          | <span data-ttu-id="85b5b-120">说明</span><span class="sxs-lookup"><span data-stu-id="85b5b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="85b5b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="85b5b-121">Authorization</span></span> | <span data-ttu-id="85b5b-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="85b5b-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="85b5b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="85b5b-123">Request body</span></span>

<span data-ttu-id="85b5b-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="85b5b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85b5b-125">响应</span><span class="sxs-lookup"><span data-stu-id="85b5b-125">Response</span></span>

<span data-ttu-id="85b5b-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="85b5b-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85b5b-128">示例</span><span class="sxs-lookup"><span data-stu-id="85b5b-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85b5b-129">请求</span><span class="sxs-lookup"><span data-stu-id="85b5b-129">Request</span></span>

<span data-ttu-id="85b5b-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="85b5b-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85b5b-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="85b5b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```
# <a name="c"></a>[<span data-ttu-id="85b5b-132">C#</span><span class="sxs-lookup"><span data-stu-id="85b5b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85b5b-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85b5b-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85b5b-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85b5b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="85b5b-135">响应</span><span class="sxs-lookup"><span data-stu-id="85b5b-135">Response</span></span>

<span data-ttu-id="85b5b-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="85b5b-136">The following is an example of the response.</span></span>

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
