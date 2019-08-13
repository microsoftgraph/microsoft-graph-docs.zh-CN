---
title: 删除 messageRule
description: 删除指定的 messageRule 对象。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 177b66649bae0ed78ffde2b689e20aee21dcf68b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342787"
---
# <a name="delete-messagerule"></a><span data-ttu-id="3853a-103">删除 messageRule</span><span class="sxs-lookup"><span data-stu-id="3853a-103">Delete messageRule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3853a-104">删除指定的 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3853a-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3853a-105">权限</span><span class="sxs-lookup"><span data-stu-id="3853a-105">Permissions</span></span>
<span data-ttu-id="3853a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3853a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3853a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3853a-108">Permission type</span></span>      | <span data-ttu-id="3853a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3853a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3853a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3853a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3853a-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3853a-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="3853a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3853a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3853a-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3853a-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="3853a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3853a-114">Application</span></span> | <span data-ttu-id="3853a-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3853a-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3853a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3853a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="3853a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3853a-117">Request headers</span></span>
| <span data-ttu-id="3853a-118">名称</span><span class="sxs-lookup"><span data-stu-id="3853a-118">Name</span></span>       | <span data-ttu-id="3853a-119">说明</span><span class="sxs-lookup"><span data-stu-id="3853a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3853a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3853a-120">Authorization</span></span>  | <span data-ttu-id="3853a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3853a-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="3853a-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3853a-123">Request body</span></span>
<span data-ttu-id="3853a-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3853a-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="3853a-125">响应</span><span class="sxs-lookup"><span data-stu-id="3853a-125">Response</span></span>
<span data-ttu-id="3853a-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3853a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3853a-128">示例</span><span class="sxs-lookup"><span data-stu-id="3853a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3853a-129">请求</span><span class="sxs-lookup"><span data-stu-id="3853a-129">Request</span></span>
<span data-ttu-id="3853a-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3853a-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3853a-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3853a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3853a-132">C#</span><span class="sxs-lookup"><span data-stu-id="3853a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3853a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3853a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3853a-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="3853a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3853a-135">Java</span><span class="sxs-lookup"><span data-stu-id="3853a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3853a-136">响应</span><span class="sxs-lookup"><span data-stu-id="3853a-136">Response</span></span>
<span data-ttu-id="3853a-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3853a-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
