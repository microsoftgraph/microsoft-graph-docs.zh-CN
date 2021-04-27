---
title: 删除域
description: 从租户中删除域。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5f00627823d4a9cc571143c8e0e09ba297bd4902
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046536"
---
# <a name="delete-domain"></a><span data-ttu-id="29096-103">删除域</span><span class="sxs-lookup"><span data-stu-id="29096-103">Delete domain</span></span>

<span data-ttu-id="29096-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29096-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29096-105">从租户中删除域。</span><span class="sxs-lookup"><span data-stu-id="29096-105">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="29096-106">**重要提示：** 已删除的域不可恢复。</span><span class="sxs-lookup"><span data-stu-id="29096-106">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="29096-107">权限</span><span class="sxs-lookup"><span data-stu-id="29096-107">Permissions</span></span>

<span data-ttu-id="29096-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29096-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="29096-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="29096-110">Permission type</span></span>      | <span data-ttu-id="29096-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29096-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29096-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29096-112">Delegated (work or school account)</span></span> | <span data-ttu-id="29096-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="29096-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29096-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29096-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29096-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="29096-115">Not supported.</span></span>    |
|<span data-ttu-id="29096-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="29096-116">Application</span></span> | <span data-ttu-id="29096-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29096-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="29096-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29096-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="29096-119">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="29096-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="29096-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="29096-120">Request headers</span></span>

| <span data-ttu-id="29096-121">名称</span><span class="sxs-lookup"><span data-stu-id="29096-121">Name</span></span>       | <span data-ttu-id="29096-122">说明</span><span class="sxs-lookup"><span data-stu-id="29096-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="29096-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29096-123">Authorization</span></span>  | <span data-ttu-id="29096-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="29096-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="29096-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29096-126">Content-Type</span></span>  | <span data-ttu-id="29096-127">application/json</span><span class="sxs-lookup"><span data-stu-id="29096-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="29096-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="29096-128">Request body</span></span>

<span data-ttu-id="29096-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="29096-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29096-130">响应</span><span class="sxs-lookup"><span data-stu-id="29096-130">Response</span></span>

<span data-ttu-id="29096-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="29096-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="29096-133">示例</span><span class="sxs-lookup"><span data-stu-id="29096-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="29096-134">请求</span><span class="sxs-lookup"><span data-stu-id="29096-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="29096-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="29096-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="29096-136">C#</span><span class="sxs-lookup"><span data-stu-id="29096-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29096-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29096-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29096-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29096-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="29096-139">Java</span><span class="sxs-lookup"><span data-stu-id="29096-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="29096-140">响应</span><span class="sxs-lookup"><span data-stu-id="29096-140">Response</span></span>

<span data-ttu-id="29096-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="29096-141">Note: The response object shown here might be shortened for readability.</span></span>
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


