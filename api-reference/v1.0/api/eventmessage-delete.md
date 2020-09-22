---
title: 删除 eventMessage
description: 删除 eventMessage。
author: harini84
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 833c2af37ae92cccea5abf0c2eefc3efbaa75c16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038737"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="f746e-103">删除 eventMessage</span><span class="sxs-lookup"><span data-stu-id="f746e-103">Delete eventMessage</span></span>

<span data-ttu-id="f746e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f746e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f746e-105">删除 eventMessage。</span><span class="sxs-lookup"><span data-stu-id="f746e-105">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="f746e-106">权限</span><span class="sxs-lookup"><span data-stu-id="f746e-106">Permissions</span></span>
<span data-ttu-id="f746e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f746e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f746e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f746e-109">Permission type</span></span>      | <span data-ttu-id="f746e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f746e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f746e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f746e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f746e-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f746e-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f746e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f746e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f746e-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f746e-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="f746e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f746e-115">Application</span></span> | <span data-ttu-id="f746e-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f746e-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f746e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f746e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f746e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f746e-118">Request headers</span></span>
| <span data-ttu-id="f746e-119">名称</span><span class="sxs-lookup"><span data-stu-id="f746e-119">Name</span></span>       | <span data-ttu-id="f746e-120">类型</span><span class="sxs-lookup"><span data-stu-id="f746e-120">Type</span></span> | <span data-ttu-id="f746e-121">说明</span><span class="sxs-lookup"><span data-stu-id="f746e-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f746e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f746e-122">Authorization</span></span>  | <span data-ttu-id="f746e-123">string</span><span class="sxs-lookup"><span data-stu-id="f746e-123">string</span></span>  | <span data-ttu-id="f746e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f746e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f746e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f746e-126">Request body</span></span>
<span data-ttu-id="f746e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f746e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f746e-128">响应</span><span class="sxs-lookup"><span data-stu-id="f746e-128">Response</span></span>

<span data-ttu-id="f746e-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f746e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f746e-131">示例</span><span class="sxs-lookup"><span data-stu-id="f746e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f746e-132">请求</span><span class="sxs-lookup"><span data-stu-id="f746e-132">Request</span></span>
<span data-ttu-id="f746e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f746e-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f746e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f746e-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/messages/{id}
```
# <a name="c"></a>[<span data-ttu-id="f746e-135">C#</span><span class="sxs-lookup"><span data-stu-id="f746e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f746e-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f746e-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f746e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f746e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f746e-138">Java</span><span class="sxs-lookup"><span data-stu-id="f746e-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-eventmessage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f746e-139">响应</span><span class="sxs-lookup"><span data-stu-id="f746e-139">Response</span></span>
<span data-ttu-id="f746e-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f746e-140">Here is an example of the response.</span></span> 
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

