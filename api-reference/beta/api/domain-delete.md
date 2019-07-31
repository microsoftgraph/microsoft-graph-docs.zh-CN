---
title: 删除域
description: 从租户中删除域。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2bde386ffec0340a2aad66d20f4cedf0ee243e4d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957505"
---
# <a name="delete-domain"></a><span data-ttu-id="dd9d6-103">删除域</span><span class="sxs-lookup"><span data-stu-id="dd9d6-103">Delete domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd9d6-104">从租户中删除域。</span><span class="sxs-lookup"><span data-stu-id="dd9d6-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="dd9d6-105">**重要说明:** 删除的域不可恢复。</span><span class="sxs-lookup"><span data-stu-id="dd9d6-105">**Important:** Deleted domains are not recoverable.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd9d6-106">权限</span><span class="sxs-lookup"><span data-stu-id="dd9d6-106">Permissions</span></span>

<span data-ttu-id="dd9d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd9d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dd9d6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd9d6-109">Permission type</span></span>      | <span data-ttu-id="dd9d6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd9d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dd9d6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd9d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dd9d6-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dd9d6-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dd9d6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd9d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd9d6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd9d6-114">Not supported.</span></span>    |
|<span data-ttu-id="dd9d6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd9d6-115">Application</span></span> | <span data-ttu-id="dd9d6-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd9d6-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd9d6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd9d6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="dd9d6-118">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="dd9d6-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dd9d6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd9d6-119">Request headers</span></span>

| <span data-ttu-id="dd9d6-120">名称</span><span class="sxs-lookup"><span data-stu-id="dd9d6-120">Name</span></span>       | <span data-ttu-id="dd9d6-121">说明</span><span class="sxs-lookup"><span data-stu-id="dd9d6-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dd9d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd9d6-122">Authorization</span></span>  | <span data-ttu-id="dd9d6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd9d6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dd9d6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dd9d6-125">Content-Type</span></span>  | <span data-ttu-id="dd9d6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd9d6-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd9d6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd9d6-127">Request body</span></span>

<span data-ttu-id="dd9d6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd9d6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd9d6-129">响应</span><span class="sxs-lookup"><span data-stu-id="dd9d6-129">Response</span></span>

<span data-ttu-id="dd9d6-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="dd9d6-p103">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd9d6-132">示例</span><span class="sxs-lookup"><span data-stu-id="dd9d6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dd9d6-133">请求</span><span class="sxs-lookup"><span data-stu-id="dd9d6-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dd9d6-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="dd9d6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dd9d6-135">C#</span><span class="sxs-lookup"><span data-stu-id="dd9d6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dd9d6-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="dd9d6-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dd9d6-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="dd9d6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dd9d6-138">Java</span><span class="sxs-lookup"><span data-stu-id="dd9d6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dd9d6-139">响应</span><span class="sxs-lookup"><span data-stu-id="dd9d6-139">Response</span></span>

<span data-ttu-id="dd9d6-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd9d6-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
