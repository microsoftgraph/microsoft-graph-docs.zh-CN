---
title: 删除 eventMessage
description: 删除 eventMessage。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 80531f331ff2be2a4dc60386f0825ef3314a4a42
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461575"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="2821b-103">删除 eventMessage</span><span class="sxs-lookup"><span data-stu-id="2821b-103">Delete eventMessage</span></span>

<span data-ttu-id="2821b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2821b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2821b-105">删除 eventMessage。</span><span class="sxs-lookup"><span data-stu-id="2821b-105">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="2821b-106">权限</span><span class="sxs-lookup"><span data-stu-id="2821b-106">Permissions</span></span>
<span data-ttu-id="2821b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2821b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2821b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2821b-109">Permission type</span></span>      | <span data-ttu-id="2821b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2821b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2821b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2821b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2821b-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2821b-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2821b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2821b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2821b-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2821b-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="2821b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2821b-115">Application</span></span> | <span data-ttu-id="2821b-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2821b-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2821b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2821b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2821b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2821b-118">Request headers</span></span>
| <span data-ttu-id="2821b-119">名称</span><span class="sxs-lookup"><span data-stu-id="2821b-119">Name</span></span>       | <span data-ttu-id="2821b-120">类型</span><span class="sxs-lookup"><span data-stu-id="2821b-120">Type</span></span> | <span data-ttu-id="2821b-121">说明</span><span class="sxs-lookup"><span data-stu-id="2821b-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2821b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2821b-122">Authorization</span></span>  | <span data-ttu-id="2821b-123">string</span><span class="sxs-lookup"><span data-stu-id="2821b-123">string</span></span>  | <span data-ttu-id="2821b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2821b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2821b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2821b-126">Request body</span></span>
<span data-ttu-id="2821b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2821b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2821b-128">响应</span><span class="sxs-lookup"><span data-stu-id="2821b-128">Response</span></span>

<span data-ttu-id="2821b-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2821b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2821b-131">示例</span><span class="sxs-lookup"><span data-stu-id="2821b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2821b-132">请求</span><span class="sxs-lookup"><span data-stu-id="2821b-132">Request</span></span>
<span data-ttu-id="2821b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2821b-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2821b-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2821b-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="2821b-135">C#</span><span class="sxs-lookup"><span data-stu-id="2821b-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2821b-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2821b-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2821b-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2821b-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2821b-138">Java</span><span class="sxs-lookup"><span data-stu-id="2821b-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2821b-139">响应</span><span class="sxs-lookup"><span data-stu-id="2821b-139">Response</span></span>
<span data-ttu-id="2821b-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2821b-140">Here is an example of the response.</span></span> 
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
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
