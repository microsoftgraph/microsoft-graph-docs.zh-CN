---
title: 删除域
description: 从租户中删除域。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 55387156e1931f851afa88ac4c33a9e100985e2a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260485"
---
# <a name="delete-domain"></a><span data-ttu-id="9a99d-103">删除域</span><span class="sxs-lookup"><span data-stu-id="9a99d-103">Delete domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a99d-104">从租户中删除域。</span><span class="sxs-lookup"><span data-stu-id="9a99d-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="9a99d-105">**重要说明:** 删除的域不可恢复。</span><span class="sxs-lookup"><span data-stu-id="9a99d-105">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a99d-106">权限</span><span class="sxs-lookup"><span data-stu-id="9a99d-106">Permissions</span></span>

<span data-ttu-id="9a99d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a99d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9a99d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a99d-109">Permission type</span></span>      | <span data-ttu-id="9a99d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a99d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a99d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a99d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a99d-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a99d-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a99d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a99d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a99d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a99d-114">Not supported.</span></span>    |
|<span data-ttu-id="9a99d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a99d-115">Application</span></span> | <span data-ttu-id="9a99d-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a99d-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a99d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a99d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="9a99d-118">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="9a99d-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a99d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a99d-119">Request headers</span></span>

| <span data-ttu-id="9a99d-120">名称</span><span class="sxs-lookup"><span data-stu-id="9a99d-120">Name</span></span>       | <span data-ttu-id="9a99d-121">说明</span><span class="sxs-lookup"><span data-stu-id="9a99d-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9a99d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a99d-122">Authorization</span></span>  | <span data-ttu-id="9a99d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9a99d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9a99d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a99d-125">Content-Type</span></span>  | <span data-ttu-id="9a99d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a99d-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9a99d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a99d-127">Request body</span></span>

<span data-ttu-id="9a99d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9a99d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a99d-129">响应</span><span class="sxs-lookup"><span data-stu-id="9a99d-129">Response</span></span>

<span data-ttu-id="9a99d-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="9a99d-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a99d-132">示例</span><span class="sxs-lookup"><span data-stu-id="9a99d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a99d-133">请求</span><span class="sxs-lookup"><span data-stu-id="9a99d-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="9a99d-134">响应</span><span class="sxs-lookup"><span data-stu-id="9a99d-134">Response</span></span>

<span data-ttu-id="9a99d-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a99d-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9a99d-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="9a99d-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9a99d-138">C#</span><span class="sxs-lookup"><span data-stu-id="9a99d-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a99d-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="9a99d-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_domain-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9a99d-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="9a99d-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_domain-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
