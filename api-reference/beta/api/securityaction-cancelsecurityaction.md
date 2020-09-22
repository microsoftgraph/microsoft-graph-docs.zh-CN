---
title: 'securityAction: cancelSecurityAction'
description: 取消安全操作。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 87cb0eca08e1d8c1dce81440fbaed40d12b46fa8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046939"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="565d8-103">securityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="565d8-103">securityAction: cancelSecurityAction</span></span>

<span data-ttu-id="565d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="565d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="565d8-105">取消安全操作。</span><span class="sxs-lookup"><span data-stu-id="565d8-105">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="565d8-106">权限</span><span class="sxs-lookup"><span data-stu-id="565d8-106">Permissions</span></span>

<span data-ttu-id="565d8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="565d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="565d8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="565d8-109">Permission type</span></span>                        | <span data-ttu-id="565d8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="565d8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="565d8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="565d8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="565d8-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="565d8-112">Not supported.</span></span> |
| <span data-ttu-id="565d8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="565d8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="565d8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="565d8-114">Not supported.</span></span> |
| <span data-ttu-id="565d8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="565d8-115">Application</span></span>                            | <span data-ttu-id="565d8-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="565d8-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="565d8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="565d8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="565d8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="565d8-118">Request headers</span></span>

| <span data-ttu-id="565d8-119">名称</span><span class="sxs-lookup"><span data-stu-id="565d8-119">Name</span></span>          | <span data-ttu-id="565d8-120">说明</span><span class="sxs-lookup"><span data-stu-id="565d8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="565d8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="565d8-121">Authorization</span></span> | <span data-ttu-id="565d8-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="565d8-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="565d8-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="565d8-123">Request body</span></span>

<span data-ttu-id="565d8-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="565d8-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="565d8-125">响应</span><span class="sxs-lookup"><span data-stu-id="565d8-125">Response</span></span>

<span data-ttu-id="565d8-p102">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="565d8-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="565d8-128">示例</span><span class="sxs-lookup"><span data-stu-id="565d8-128">Examples</span></span>

<span data-ttu-id="565d8-129">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="565d8-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="565d8-130">请求</span><span class="sxs-lookup"><span data-stu-id="565d8-130">Request</span></span>

<span data-ttu-id="565d8-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="565d8-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="565d8-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="565d8-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="c"></a>[<span data-ttu-id="565d8-133">C#</span><span class="sxs-lookup"><span data-stu-id="565d8-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="565d8-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="565d8-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="565d8-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="565d8-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="565d8-136">响应</span><span class="sxs-lookup"><span data-stu-id="565d8-136">Response</span></span>

<span data-ttu-id="565d8-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="565d8-137">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction: cancelSecurityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


