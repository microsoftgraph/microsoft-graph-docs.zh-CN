---
title: 删除 messageRule
description: 删除指定的 messageRule 对象。
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3d4405473188108e304dc18b280d70ebb18806db
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43354902"
---
# <a name="delete-messagerule"></a><span data-ttu-id="96eba-103">删除 messageRule</span><span class="sxs-lookup"><span data-stu-id="96eba-103">Delete messageRule</span></span>

<span data-ttu-id="96eba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96eba-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="96eba-105">删除指定的 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96eba-105">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96eba-106">权限</span><span class="sxs-lookup"><span data-stu-id="96eba-106">Permissions</span></span>
<span data-ttu-id="96eba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96eba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96eba-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="96eba-109">Permission type</span></span>      | <span data-ttu-id="96eba-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96eba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96eba-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96eba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="96eba-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96eba-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="96eba-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96eba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96eba-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96eba-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="96eba-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="96eba-115">Application</span></span> | <span data-ttu-id="96eba-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96eba-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="96eba-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96eba-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="96eba-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="96eba-118">Request headers</span></span>
| <span data-ttu-id="96eba-119">名称</span><span class="sxs-lookup"><span data-stu-id="96eba-119">Name</span></span>       | <span data-ttu-id="96eba-120">说明</span><span class="sxs-lookup"><span data-stu-id="96eba-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="96eba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="96eba-121">Authorization</span></span>  | <span data-ttu-id="96eba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96eba-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="96eba-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="96eba-124">Request body</span></span>
<span data-ttu-id="96eba-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96eba-125">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="96eba-126">响应</span><span class="sxs-lookup"><span data-stu-id="96eba-126">Response</span></span>
<span data-ttu-id="96eba-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="96eba-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96eba-129">示例</span><span class="sxs-lookup"><span data-stu-id="96eba-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96eba-130">请求</span><span class="sxs-lookup"><span data-stu-id="96eba-130">Request</span></span>
<span data-ttu-id="96eba-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96eba-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="96eba-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="96eba-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
# <a name="c"></a>[<span data-ttu-id="96eba-133">C#</span><span class="sxs-lookup"><span data-stu-id="96eba-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="96eba-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="96eba-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="96eba-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="96eba-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="96eba-136">Java</span><span class="sxs-lookup"><span data-stu-id="96eba-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="96eba-137">响应</span><span class="sxs-lookup"><span data-stu-id="96eba-137">Response</span></span>
<span data-ttu-id="96eba-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="96eba-138">Here is an example of the response.</span></span> 
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
