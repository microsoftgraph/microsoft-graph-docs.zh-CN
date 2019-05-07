---
title: 'securityAction: cancelSecurityAction'
description: 取消安全操作。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 33fa78176dcb32bad889c7d3336177ef96aaa0b6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638905"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="1f544-103">securityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="1f544-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f544-104">取消安全操作。</span><span class="sxs-lookup"><span data-stu-id="1f544-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f544-105">权限</span><span class="sxs-lookup"><span data-stu-id="1f544-105">Permissions</span></span>

<span data-ttu-id="1f544-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1f544-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1f544-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f544-108">Permission type</span></span>                        | <span data-ttu-id="1f544-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1f544-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1f544-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f544-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f544-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f544-111">Not supported.</span></span> |
| <span data-ttu-id="1f544-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f544-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f544-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f544-113">Not supported.</span></span> |
| <span data-ttu-id="1f544-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f544-114">Application</span></span>                            | <span data-ttu-id="1f544-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f544-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f544-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f544-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="1f544-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f544-117">Request headers</span></span>

| <span data-ttu-id="1f544-118">名称</span><span class="sxs-lookup"><span data-stu-id="1f544-118">Name</span></span>          | <span data-ttu-id="1f544-119">说明</span><span class="sxs-lookup"><span data-stu-id="1f544-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="1f544-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f544-120">Authorization</span></span> | <span data-ttu-id="1f544-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1f544-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f544-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f544-122">Request body</span></span>

<span data-ttu-id="1f544-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1f544-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f544-124">响应</span><span class="sxs-lookup"><span data-stu-id="1f544-124">Response</span></span>

<span data-ttu-id="1f544-p102">如果成功，此方法返回 `200, OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1f544-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1f544-127">示例</span><span class="sxs-lookup"><span data-stu-id="1f544-127">Examples</span></span>

<span data-ttu-id="1f544-128">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1f544-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="1f544-129">请求</span><span class="sxs-lookup"><span data-stu-id="1f544-129">Request</span></span>

<span data-ttu-id="1f544-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1f544-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```

### <a name="response"></a><span data-ttu-id="1f544-131">响应</span><span class="sxs-lookup"><span data-stu-id="1f544-131">Response</span></span>

<span data-ttu-id="1f544-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1f544-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1f544-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1f544-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1f544-134">语言</span><span class="sxs-lookup"><span data-stu-id="1f544-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/securityaction_cancelsecurityaction-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1f544-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="1f544-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/securityaction_cancelsecurityaction-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction: cancelSecurityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/securityaction-cancelsecurityaction.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/securityaction-cancelsecurityaction.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
