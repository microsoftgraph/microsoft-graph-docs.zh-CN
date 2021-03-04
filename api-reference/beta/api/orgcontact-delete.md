---
title: 删除 orgContact
description: 删除 orgContact。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1b853a153afea17bae86a7e0d4215f9ae0ac39db
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434020"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="f9985-103">删除 orgContact</span><span class="sxs-lookup"><span data-stu-id="f9985-103">Delete orgContact</span></span>

<span data-ttu-id="f9985-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9985-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9985-105">删除 orgContact。</span><span class="sxs-lookup"><span data-stu-id="f9985-105">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="f9985-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f9985-106">Permissions</span></span>
<span data-ttu-id="f9985-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9985-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9985-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9985-109">Permission type</span></span>      | <span data-ttu-id="f9985-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9985-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9985-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9985-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f9985-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f9985-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f9985-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9985-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9985-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9985-114">Not supported.</span></span>    |
|<span data-ttu-id="f9985-115">Application</span><span class="sxs-lookup"><span data-stu-id="f9985-115">Application</span></span> | <span data-ttu-id="f9985-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9985-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9985-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9985-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="f9985-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9985-118">Request headers</span></span>
| <span data-ttu-id="f9985-119">名称</span><span class="sxs-lookup"><span data-stu-id="f9985-119">Name</span></span>       | <span data-ttu-id="f9985-120">类型</span><span class="sxs-lookup"><span data-stu-id="f9985-120">Type</span></span> | <span data-ttu-id="f9985-121">说明</span><span class="sxs-lookup"><span data-stu-id="f9985-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f9985-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9985-122">Authorization</span></span>  | <span data-ttu-id="f9985-123">string</span><span class="sxs-lookup"><span data-stu-id="f9985-123">string</span></span>  | <span data-ttu-id="f9985-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9985-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9985-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9985-126">Request body</span></span>
<span data-ttu-id="f9985-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f9985-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9985-128">响应</span><span class="sxs-lookup"><span data-stu-id="f9985-128">Response</span></span>

<span data-ttu-id="f9985-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f9985-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9985-131">示例</span><span class="sxs-lookup"><span data-stu-id="f9985-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f9985-132">请求</span><span class="sxs-lookup"><span data-stu-id="f9985-132">Request</span></span>
<span data-ttu-id="f9985-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9985-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f9985-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9985-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="f9985-135">C#</span><span class="sxs-lookup"><span data-stu-id="f9985-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9985-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9985-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9985-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9985-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9985-138">Java</span><span class="sxs-lookup"><span data-stu-id="f9985-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-orgcontact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f9985-139">响应</span><span class="sxs-lookup"><span data-stu-id="f9985-139">Response</span></span>
<span data-ttu-id="f9985-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f9985-140">Here is an example of the response.</span></span> 
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
  "description": "Delete orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


