---
title: 删除 orgContact
description: 删除 orgContact。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 23101ca0c47d09afbefccc2efe506f1137cf2bf4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456297"
---
# <a name="delete-orgcontact"></a><span data-ttu-id="f80f2-103">删除 orgContact</span><span class="sxs-lookup"><span data-stu-id="f80f2-103">Delete orgContact</span></span>

<span data-ttu-id="f80f2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f80f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f80f2-105">删除 orgContact。</span><span class="sxs-lookup"><span data-stu-id="f80f2-105">Delete orgContact.</span></span>
## <a name="permissions"></a><span data-ttu-id="f80f2-106">权限</span><span class="sxs-lookup"><span data-stu-id="f80f2-106">Permissions</span></span>
<span data-ttu-id="f80f2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f80f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f80f2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f80f2-109">Permission type</span></span>      | <span data-ttu-id="f80f2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f80f2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f80f2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f80f2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f80f2-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f80f2-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f80f2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f80f2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f80f2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f80f2-114">Not supported.</span></span>    |
|<span data-ttu-id="f80f2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f80f2-115">Application</span></span> | <span data-ttu-id="f80f2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f80f2-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f80f2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f80f2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /contacts/{id}

```
## <a name="request-headers"></a><span data-ttu-id="f80f2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f80f2-118">Request headers</span></span>
| <span data-ttu-id="f80f2-119">名称</span><span class="sxs-lookup"><span data-stu-id="f80f2-119">Name</span></span>       | <span data-ttu-id="f80f2-120">类型</span><span class="sxs-lookup"><span data-stu-id="f80f2-120">Type</span></span> | <span data-ttu-id="f80f2-121">说明</span><span class="sxs-lookup"><span data-stu-id="f80f2-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f80f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f80f2-122">Authorization</span></span>  | <span data-ttu-id="f80f2-123">string</span><span class="sxs-lookup"><span data-stu-id="f80f2-123">string</span></span>  | <span data-ttu-id="f80f2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f80f2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f80f2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f80f2-126">Request body</span></span>
<span data-ttu-id="f80f2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f80f2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f80f2-128">响应</span><span class="sxs-lookup"><span data-stu-id="f80f2-128">Response</span></span>

<span data-ttu-id="f80f2-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f80f2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f80f2-131">示例</span><span class="sxs-lookup"><span data-stu-id="f80f2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f80f2-132">请求</span><span class="sxs-lookup"><span data-stu-id="f80f2-132">Request</span></span>
<span data-ttu-id="f80f2-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f80f2-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f80f2-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f80f2-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_orgcontact"
}-->
```http
DELETE https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="c"></a>[<span data-ttu-id="f80f2-135">C#</span><span class="sxs-lookup"><span data-stu-id="f80f2-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f80f2-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f80f2-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f80f2-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f80f2-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f80f2-138">响应</span><span class="sxs-lookup"><span data-stu-id="f80f2-138">Response</span></span>
<span data-ttu-id="f80f2-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f80f2-139">Here is an example of the response.</span></span> 
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
