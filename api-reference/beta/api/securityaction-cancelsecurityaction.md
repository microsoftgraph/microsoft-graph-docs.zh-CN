---
title: 'securityAction: cancelSecurityAction'
description: 取消安全操作。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 3a4c71441b4d1af381057ea14fdce1a27512d69a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457350"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="4cbc4-103">securityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="4cbc4-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cbc4-104">取消安全操作。</span><span class="sxs-lookup"><span data-stu-id="4cbc4-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cbc4-105">权限</span><span class="sxs-lookup"><span data-stu-id="4cbc4-105">Permissions</span></span>

<span data-ttu-id="4cbc4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4cbc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4cbc4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4cbc4-108">Permission type</span></span>                        | <span data-ttu-id="4cbc4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4cbc4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4cbc4-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4cbc4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4cbc4-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cbc4-111">Not supported.</span></span> |
| <span data-ttu-id="4cbc4-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4cbc4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cbc4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cbc4-113">Not supported.</span></span> |
| <span data-ttu-id="4cbc4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4cbc4-114">Application</span></span>                            | <span data-ttu-id="4cbc4-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cbc4-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cbc4-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4cbc4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="4cbc4-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="4cbc4-117">Request headers</span></span>

| <span data-ttu-id="4cbc4-118">名称</span><span class="sxs-lookup"><span data-stu-id="4cbc4-118">Name</span></span>          | <span data-ttu-id="4cbc4-119">说明</span><span class="sxs-lookup"><span data-stu-id="4cbc4-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4cbc4-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cbc4-120">Authorization</span></span> | <span data-ttu-id="4cbc4-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4cbc4-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="4cbc4-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="4cbc4-122">Request body</span></span>

<span data-ttu-id="4cbc4-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4cbc4-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cbc4-124">响应</span><span class="sxs-lookup"><span data-stu-id="4cbc4-124">Response</span></span>

<span data-ttu-id="4cbc4-p102">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4cbc4-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4cbc4-127">示例</span><span class="sxs-lookup"><span data-stu-id="4cbc4-127">Examples</span></span>

<span data-ttu-id="4cbc4-128">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="4cbc4-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="4cbc4-129">请求</span><span class="sxs-lookup"><span data-stu-id="4cbc4-129">Request</span></span>

<span data-ttu-id="4cbc4-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4cbc4-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4cbc4-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4cbc4-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4cbc4-132">C#</span><span class="sxs-lookup"><span data-stu-id="4cbc4-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/securityaction-cancelsecurityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4cbc4-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="4cbc4-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/securityaction-cancelsecurityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4cbc4-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="4cbc4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/securityaction-cancelsecurityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4cbc4-135">响应</span><span class="sxs-lookup"><span data-stu-id="4cbc4-135">Response</span></span>

<span data-ttu-id="4cbc4-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4cbc4-136">The following is an example of the response.</span></span>
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
