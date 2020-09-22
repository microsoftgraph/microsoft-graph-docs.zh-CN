---
title: 删除域
description: 从租户中删除域。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6d6e3505ce0dc57ad29ae5dd7d440a4169e7a7c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008594"
---
# <a name="delete-domain"></a><span data-ttu-id="6d73f-103">删除域</span><span class="sxs-lookup"><span data-stu-id="6d73f-103">Delete domain</span></span>

<span data-ttu-id="6d73f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d73f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d73f-105">从租户中删除域。</span><span class="sxs-lookup"><span data-stu-id="6d73f-105">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="6d73f-106">**重要说明：** 删除的域不可恢复。</span><span class="sxs-lookup"><span data-stu-id="6d73f-106">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d73f-107">权限</span><span class="sxs-lookup"><span data-stu-id="6d73f-107">Permissions</span></span>

<span data-ttu-id="6d73f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d73f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6d73f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d73f-110">Permission type</span></span>      | <span data-ttu-id="6d73f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d73f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d73f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d73f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6d73f-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6d73f-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6d73f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d73f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d73f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d73f-115">Not supported.</span></span>    |
|<span data-ttu-id="6d73f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d73f-116">Application</span></span> | <span data-ttu-id="6d73f-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d73f-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d73f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d73f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="6d73f-119">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="6d73f-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d73f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d73f-120">Request headers</span></span>

| <span data-ttu-id="6d73f-121">名称</span><span class="sxs-lookup"><span data-stu-id="6d73f-121">Name</span></span>       | <span data-ttu-id="6d73f-122">说明</span><span class="sxs-lookup"><span data-stu-id="6d73f-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6d73f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d73f-123">Authorization</span></span>  | <span data-ttu-id="6d73f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6d73f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6d73f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d73f-126">Content-Type</span></span>  | <span data-ttu-id="6d73f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6d73f-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d73f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d73f-128">Request body</span></span>

<span data-ttu-id="6d73f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6d73f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d73f-130">响应</span><span class="sxs-lookup"><span data-stu-id="6d73f-130">Response</span></span>

<span data-ttu-id="6d73f-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="6d73f-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d73f-133">示例</span><span class="sxs-lookup"><span data-stu-id="6d73f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d73f-134">请求</span><span class="sxs-lookup"><span data-stu-id="6d73f-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6d73f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="6d73f-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="6d73f-136">C#</span><span class="sxs-lookup"><span data-stu-id="6d73f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6d73f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d73f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6d73f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6d73f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6d73f-139">响应</span><span class="sxs-lookup"><span data-stu-id="6d73f-139">Response</span></span>

<span data-ttu-id="6d73f-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6d73f-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->


