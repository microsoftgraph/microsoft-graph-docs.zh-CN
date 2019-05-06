---
title: 删除域
description: 从租户中删除域。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f249c17fc296b85bc45c8d8eed620b1742b1b55b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589384"
---
# <a name="delete-domain"></a><span data-ttu-id="d4943-103">删除域</span><span class="sxs-lookup"><span data-stu-id="d4943-103">Delete domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4943-104">从租户中删除域。</span><span class="sxs-lookup"><span data-stu-id="d4943-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="d4943-105">**重要说明:** 删除的域不可恢复。</span><span class="sxs-lookup"><span data-stu-id="d4943-105">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4943-106">权限</span><span class="sxs-lookup"><span data-stu-id="d4943-106">Permissions</span></span>

<span data-ttu-id="d4943-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4943-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d4943-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4943-109">Permission type</span></span>      | <span data-ttu-id="d4943-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4943-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4943-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4943-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d4943-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4943-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4943-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4943-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4943-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4943-114">Not supported.</span></span>    |
|<span data-ttu-id="d4943-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4943-115">Application</span></span> | <span data-ttu-id="d4943-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4943-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4943-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4943-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="d4943-118">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="d4943-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4943-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4943-119">Request headers</span></span>

| <span data-ttu-id="d4943-120">名称</span><span class="sxs-lookup"><span data-stu-id="d4943-120">Name</span></span>       | <span data-ttu-id="d4943-121">说明</span><span class="sxs-lookup"><span data-stu-id="d4943-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d4943-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4943-122">Authorization</span></span>  | <span data-ttu-id="d4943-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4943-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d4943-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d4943-125">Content-Type</span></span>  | <span data-ttu-id="d4943-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4943-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4943-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4943-127">Request body</span></span>

<span data-ttu-id="d4943-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d4943-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4943-129">响应</span><span class="sxs-lookup"><span data-stu-id="d4943-129">Response</span></span>

<span data-ttu-id="d4943-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="d4943-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4943-132">示例</span><span class="sxs-lookup"><span data-stu-id="d4943-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4943-133">请求</span><span class="sxs-lookup"><span data-stu-id="d4943-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="d4943-134">响应</span><span class="sxs-lookup"><span data-stu-id="d4943-134">Response</span></span>

<span data-ttu-id="d4943-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4943-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d4943-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d4943-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d4943-138">语言</span><span class="sxs-lookup"><span data-stu-id="d4943-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4943-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="d4943-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_domain-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
