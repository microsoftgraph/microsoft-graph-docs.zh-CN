---
title: 'securityAction: cancelSecurityAction'
description: 取消安全操作。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: a12f902c3f2eeed89c40497c49d9bb1a78fe6123
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976701"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="7e672-103">securityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="7e672-103">securityAction: cancelSecurityAction</span></span>

<span data-ttu-id="7e672-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e672-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e672-105">取消安全操作。</span><span class="sxs-lookup"><span data-stu-id="7e672-105">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e672-106">权限</span><span class="sxs-lookup"><span data-stu-id="7e672-106">Permissions</span></span>

<span data-ttu-id="7e672-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e672-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7e672-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e672-109">Permission type</span></span>                        | <span data-ttu-id="7e672-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e672-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7e672-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e672-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7e672-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e672-112">Not supported.</span></span> |
| <span data-ttu-id="7e672-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e672-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e672-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e672-114">Not supported.</span></span> |
| <span data-ttu-id="7e672-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e672-115">Application</span></span>                            | <span data-ttu-id="7e672-116">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e672-116">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e672-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e672-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="7e672-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e672-118">Request headers</span></span>

| <span data-ttu-id="7e672-119">名称</span><span class="sxs-lookup"><span data-stu-id="7e672-119">Name</span></span>          | <span data-ttu-id="7e672-120">说明</span><span class="sxs-lookup"><span data-stu-id="7e672-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7e672-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e672-121">Authorization</span></span> | <span data-ttu-id="7e672-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7e672-122">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7e672-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e672-123">Request body</span></span>

<span data-ttu-id="7e672-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7e672-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e672-125">响应</span><span class="sxs-lookup"><span data-stu-id="7e672-125">Response</span></span>

<span data-ttu-id="7e672-p102">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7e672-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7e672-128">示例</span><span class="sxs-lookup"><span data-stu-id="7e672-128">Examples</span></span>

<span data-ttu-id="7e672-129">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7e672-129">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="7e672-130">请求</span><span class="sxs-lookup"><span data-stu-id="7e672-130">Request</span></span>

<span data-ttu-id="7e672-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e672-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7e672-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7e672-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="c"></a>[<span data-ttu-id="7e672-133">C#</span><span class="sxs-lookup"><span data-stu-id="7e672-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7e672-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7e672-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7e672-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7e672-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7e672-136">Java</span><span class="sxs-lookup"><span data-stu-id="7e672-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/securityaction-cancelsecurityaction-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7e672-137">响应</span><span class="sxs-lookup"><span data-stu-id="7e672-137">Response</span></span>

<span data-ttu-id="7e672-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7e672-138">The following is an example of the response.</span></span>
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


