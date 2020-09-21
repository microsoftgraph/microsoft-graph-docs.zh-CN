---
title: 删除 workforceIntegration
description: 删除 workforceIntegration 的实例。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 216ebcdf7bd22cac6724c7e7b86132bb9784f159
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989777"
---
# <a name="delete-workforceintegration"></a><span data-ttu-id="d4392-103">删除 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="d4392-103">Delete workforceIntegration</span></span>

<span data-ttu-id="d4392-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4392-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4392-105">删除 [workforceIntegration](../resources/workforceintegration.md)的实例。</span><span class="sxs-lookup"><span data-stu-id="d4392-105">Delete an instance of a [workforceIntegration](../resources/workforceintegration.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d4392-106">权限</span><span class="sxs-lookup"><span data-stu-id="d4392-106">Permissions</span></span>

<span data-ttu-id="d4392-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4392-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d4392-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4392-109">Permission type</span></span>                        | <span data-ttu-id="d4392-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4392-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d4392-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4392-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d4392-112">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="d4392-112">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="d4392-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4392-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4392-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4392-114">Not supported.</span></span> |
| <span data-ttu-id="d4392-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4392-115">Application</span></span>                            | <span data-ttu-id="d4392-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4392-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4392-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4392-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teamwork/workforceIntegrations/{workforceIntegrationId}
```

## <a name="request-headers"></a><span data-ttu-id="d4392-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4392-118">Request headers</span></span>

| <span data-ttu-id="d4392-119">名称</span><span class="sxs-lookup"><span data-stu-id="d4392-119">Name</span></span>          | <span data-ttu-id="d4392-120">说明</span><span class="sxs-lookup"><span data-stu-id="d4392-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d4392-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4392-121">Authorization</span></span> | <span data-ttu-id="d4392-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="d4392-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4392-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4392-123">Request body</span></span>

<span data-ttu-id="d4392-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d4392-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4392-125">响应</span><span class="sxs-lookup"><span data-stu-id="d4392-125">Response</span></span>

<span data-ttu-id="d4392-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d4392-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d4392-128">示例</span><span class="sxs-lookup"><span data-stu-id="d4392-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d4392-129">请求</span><span class="sxs-lookup"><span data-stu-id="d4392-129">Request</span></span>

<span data-ttu-id="d4392-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d4392-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d4392-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="d4392-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_workforceintegration"
}-->

```http
DELETE https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceIntegrationId}
```
# <a name="c"></a>[<span data-ttu-id="d4392-132">C#</span><span class="sxs-lookup"><span data-stu-id="d4392-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-workforceintegration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d4392-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d4392-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-workforceintegration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d4392-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d4392-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-workforceintegration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d4392-135">响应</span><span class="sxs-lookup"><span data-stu-id="d4392-135">Response</span></span>

<span data-ttu-id="d4392-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d4392-136">The following is an example of the response.</span></span>

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


