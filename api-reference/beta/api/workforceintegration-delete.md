---
title: 删除 workforceIntegration
description: 删除 workforceIntegration 的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 37ffb3e6153228963f8a0154f9f0c8708787ed98
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870513"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="b3d42-103">删除 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="b3d42-103">Delete workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3d42-104">删除[workforceIntegration](../resources/workforceintegration.md)的实例。</span><span class="sxs-lookup"><span data-stu-id="b3d42-104">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b3d42-105">权限</span><span class="sxs-lookup"><span data-stu-id="b3d42-105">Permissions</span></span>

<span data-ttu-id="b3d42-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3d42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b3d42-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3d42-108">Permission type</span></span>                        | <span data-ttu-id="b3d42-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3d42-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b3d42-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3d42-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b3d42-111">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="b3d42-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="b3d42-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3d42-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3d42-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3d42-113">Not supported.</span></span> |
| <span data-ttu-id="b3d42-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3d42-114">Application</span></span>                            | <span data-ttu-id="b3d42-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3d42-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3d42-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3d42-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="b3d42-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3d42-117">Request headers</span></span>

| <span data-ttu-id="b3d42-118">名称</span><span class="sxs-lookup"><span data-stu-id="b3d42-118">Name</span></span>          | <span data-ttu-id="b3d42-119">说明</span><span class="sxs-lookup"><span data-stu-id="b3d42-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b3d42-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3d42-120">Authorization</span></span> | <span data-ttu-id="b3d42-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="b3d42-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b3d42-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3d42-122">Request body</span></span>

<span data-ttu-id="b3d42-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3d42-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3d42-124">响应</span><span class="sxs-lookup"><span data-stu-id="b3d42-124">Response</span></span>

<span data-ttu-id="b3d42-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b3d42-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b3d42-127">示例</span><span class="sxs-lookup"><span data-stu-id="b3d42-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b3d42-128">请求</span><span class="sxs-lookup"><span data-stu-id="b3d42-128">Request</span></span>

<span data-ttu-id="b3d42-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b3d42-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b3d42-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3d42-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b3d42-131">C#</span><span class="sxs-lookup"><span data-stu-id="b3d42-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b3d42-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3d42-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b3d42-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3d42-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b3d42-134">响应</span><span class="sxs-lookup"><span data-stu-id="b3d42-134">Response</span></span>

<span data-ttu-id="b3d42-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b3d42-135">The following is an example of the response.</span></span>

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
