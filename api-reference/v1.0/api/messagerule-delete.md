---
title: 删除 messageRule
description: 删除指定的 messageRule 对象。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: cef718dc2f9ef23cc006ba61a3cde71c38d2b1c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019045"
---
# <a name="delete-messagerule"></a><span data-ttu-id="cdfc1-103">删除 messageRule</span><span class="sxs-lookup"><span data-stu-id="cdfc1-103">Delete messageRule</span></span>

<span data-ttu-id="cdfc1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdfc1-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="cdfc1-105">删除指定的 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cdfc1-105">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdfc1-106">权限</span><span class="sxs-lookup"><span data-stu-id="cdfc1-106">Permissions</span></span>
<span data-ttu-id="cdfc1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cdfc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdfc1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdfc1-109">Permission type</span></span>      | <span data-ttu-id="cdfc1-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdfc1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdfc1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdfc1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cdfc1-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdfc1-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="cdfc1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdfc1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdfc1-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdfc1-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="cdfc1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdfc1-115">Application</span></span> | <span data-ttu-id="cdfc1-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cdfc1-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdfc1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdfc1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cdfc1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdfc1-118">Request headers</span></span>
| <span data-ttu-id="cdfc1-119">名称</span><span class="sxs-lookup"><span data-stu-id="cdfc1-119">Name</span></span>       | <span data-ttu-id="cdfc1-120">说明</span><span class="sxs-lookup"><span data-stu-id="cdfc1-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cdfc1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdfc1-121">Authorization</span></span>  | <span data-ttu-id="cdfc1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cdfc1-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="cdfc1-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdfc1-124">Request body</span></span>
<span data-ttu-id="cdfc1-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cdfc1-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="cdfc1-126">响应</span><span class="sxs-lookup"><span data-stu-id="cdfc1-126">Response</span></span>
<span data-ttu-id="cdfc1-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="cdfc1-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdfc1-129">示例</span><span class="sxs-lookup"><span data-stu-id="cdfc1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cdfc1-130">请求</span><span class="sxs-lookup"><span data-stu-id="cdfc1-130">Request</span></span>
<span data-ttu-id="cdfc1-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cdfc1-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cdfc1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdfc1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
# <a name="c"></a>[<span data-ttu-id="cdfc1-133">C#</span><span class="sxs-lookup"><span data-stu-id="cdfc1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdfc1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdfc1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdfc1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdfc1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdfc1-136">Java</span><span class="sxs-lookup"><span data-stu-id="cdfc1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="cdfc1-137">响应</span><span class="sxs-lookup"><span data-stu-id="cdfc1-137">Response</span></span>
<span data-ttu-id="cdfc1-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="cdfc1-138">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

