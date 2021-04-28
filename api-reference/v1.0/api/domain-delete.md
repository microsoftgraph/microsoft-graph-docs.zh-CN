---
title: 删除域
description: 从租户中删除域。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0ecaf2cd5c1f8f0ed0281be585a85008e6870a8f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050505"
---
# <a name="delete-domain"></a><span data-ttu-id="ada1d-103">删除域</span><span class="sxs-lookup"><span data-stu-id="ada1d-103">Delete domain</span></span>

<span data-ttu-id="ada1d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ada1d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ada1d-105">从租户中删除域。</span><span class="sxs-lookup"><span data-stu-id="ada1d-105">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="ada1d-106">**重要说明：**</span><span class="sxs-lookup"><span data-stu-id="ada1d-106">**Important:**</span></span>
> - <span data-ttu-id="ada1d-107">已删除的域不可恢复。</span><span class="sxs-lookup"><span data-stu-id="ada1d-107">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="ada1d-p101">如果存在任何仍旧依赖域的资源或对象，尝试删除会失败。可以通过使用此 [列出 domainNameReferences](domain-list-domainnamereferences.md) API 查找所有从属的资源。</span><span class="sxs-lookup"><span data-stu-id="ada1d-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain-list-domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="ada1d-110">权限</span><span class="sxs-lookup"><span data-stu-id="ada1d-110">Permissions</span></span>

<span data-ttu-id="ada1d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ada1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ada1d-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="ada1d-113">Permission type</span></span>      | <span data-ttu-id="ada1d-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ada1d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ada1d-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ada1d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="ada1d-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ada1d-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ada1d-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ada1d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ada1d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ada1d-118">Not supported.</span></span>    |
|<span data-ttu-id="ada1d-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="ada1d-119">Application</span></span> | <span data-ttu-id="ada1d-120">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ada1d-120">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ada1d-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ada1d-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="ada1d-122">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="ada1d-122">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ada1d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ada1d-123">Request headers</span></span>

| <span data-ttu-id="ada1d-124">名称</span><span class="sxs-lookup"><span data-stu-id="ada1d-124">Name</span></span>       | <span data-ttu-id="ada1d-125">说明</span><span class="sxs-lookup"><span data-stu-id="ada1d-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ada1d-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="ada1d-126">Authorization</span></span>  | <span data-ttu-id="ada1d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ada1d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ada1d-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ada1d-129">Content-Type</span></span>  | <span data-ttu-id="ada1d-130">application/json</span><span class="sxs-lookup"><span data-stu-id="ada1d-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ada1d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ada1d-131">Request body</span></span>

<span data-ttu-id="ada1d-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ada1d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ada1d-133">响应</span><span class="sxs-lookup"><span data-stu-id="ada1d-133">Response</span></span>

<span data-ttu-id="ada1d-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="ada1d-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="ada1d-136">示例</span><span class="sxs-lookup"><span data-stu-id="ada1d-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ada1d-137">请求</span><span class="sxs-lookup"><span data-stu-id="ada1d-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ada1d-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="ada1d-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="ada1d-139">C#</span><span class="sxs-lookup"><span data-stu-id="ada1d-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ada1d-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ada1d-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ada1d-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ada1d-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ada1d-142">Java</span><span class="sxs-lookup"><span data-stu-id="ada1d-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ada1d-143">响应</span><span class="sxs-lookup"><span data-stu-id="ada1d-143">Response</span></span>

<span data-ttu-id="ada1d-144">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ada1d-144">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

