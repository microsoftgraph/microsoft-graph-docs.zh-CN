---
title: 删除域
description: 从租户中删除域。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: abe6ca111236ba4c723882b7dcf63df630c22c28
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616996"
---
# <a name="delete-domain"></a><span data-ttu-id="3731d-103">删除域</span><span class="sxs-lookup"><span data-stu-id="3731d-103">Delete domain</span></span>

<span data-ttu-id="3731d-104">从租户中删除域。</span><span class="sxs-lookup"><span data-stu-id="3731d-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="3731d-105">**重要说明：**</span><span class="sxs-lookup"><span data-stu-id="3731d-105">**Important:**</span></span>
> - <span data-ttu-id="3731d-106">已删除的域不可恢复。</span><span class="sxs-lookup"><span data-stu-id="3731d-106">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="3731d-p101">如果存在任何仍旧依赖域的资源或对象，尝试删除会失败。可以通过使用此 [列出 domainNameReferences](domain-list-domainnamereferences.md) API 查找所有从属的资源。</span><span class="sxs-lookup"><span data-stu-id="3731d-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain-list-domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="3731d-109">权限</span><span class="sxs-lookup"><span data-stu-id="3731d-109">Permissions</span></span>

<span data-ttu-id="3731d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3731d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3731d-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="3731d-112">Permission type</span></span>      | <span data-ttu-id="3731d-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3731d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3731d-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3731d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="3731d-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3731d-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3731d-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3731d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3731d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3731d-117">Not supported.</span></span>    |
|<span data-ttu-id="3731d-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="3731d-118">Application</span></span> | <span data-ttu-id="3731d-119">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3731d-119">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3731d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3731d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="3731d-121">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="3731d-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3731d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="3731d-122">Request headers</span></span>

| <span data-ttu-id="3731d-123">名称</span><span class="sxs-lookup"><span data-stu-id="3731d-123">Name</span></span>       | <span data-ttu-id="3731d-124">说明</span><span class="sxs-lookup"><span data-stu-id="3731d-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3731d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3731d-125">Authorization</span></span>  | <span data-ttu-id="3731d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3731d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3731d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3731d-128">Content-Type</span></span>  | <span data-ttu-id="3731d-129">application/json</span><span class="sxs-lookup"><span data-stu-id="3731d-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3731d-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3731d-130">Request body</span></span>

<span data-ttu-id="3731d-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3731d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3731d-132">响应</span><span class="sxs-lookup"><span data-stu-id="3731d-132">Response</span></span>

<span data-ttu-id="3731d-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="3731d-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="3731d-135">示例</span><span class="sxs-lookup"><span data-stu-id="3731d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3731d-136">请求</span><span class="sxs-lookup"><span data-stu-id="3731d-136">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="3731d-137">响应</span><span class="sxs-lookup"><span data-stu-id="3731d-137">Response</span></span>

<span data-ttu-id="3731d-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3731d-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3731d-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3731d-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3731d-141">语言</span><span class="sxs-lookup"><span data-stu-id="3731d-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3731d-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="3731d-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_domain-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
