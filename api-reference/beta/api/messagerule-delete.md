---
title: 删除 messageRule
description: 删除指定的 messageRule 对象。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b6b3751ca02eb2e0c704ef839d1bfa24e9ac4260
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447919"
---
# <a name="delete-messagerule"></a><span data-ttu-id="d3d2c-103">删除 messageRule</span><span class="sxs-lookup"><span data-stu-id="d3d2c-103">Delete messageRule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3d2c-104">删除指定的 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3d2c-105">权限</span><span class="sxs-lookup"><span data-stu-id="d3d2c-105">Permissions</span></span>
<span data-ttu-id="d3d2c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3d2c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3d2c-108">Permission type</span></span>      | <span data-ttu-id="d3d2c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d3d2c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3d2c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3d2c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d3d2c-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3d2c-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="d3d2c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3d2c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3d2c-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3d2c-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="d3d2c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3d2c-114">Application</span></span> | <span data-ttu-id="d3d2c-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3d2c-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3d2c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3d2c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d3d2c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3d2c-117">Request headers</span></span>
| <span data-ttu-id="d3d2c-118">名称</span><span class="sxs-lookup"><span data-stu-id="d3d2c-118">Name</span></span>       | <span data-ttu-id="d3d2c-119">说明</span><span class="sxs-lookup"><span data-stu-id="d3d2c-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d3d2c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3d2c-120">Authorization</span></span>  | <span data-ttu-id="d3d2c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d3d2c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3d2c-123">Request body</span></span>
<span data-ttu-id="d3d2c-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d3d2c-125">响应</span><span class="sxs-lookup"><span data-stu-id="d3d2c-125">Response</span></span>
<span data-ttu-id="d3d2c-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3d2c-128">示例</span><span class="sxs-lookup"><span data-stu-id="d3d2c-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3d2c-129">请求</span><span class="sxs-lookup"><span data-stu-id="d3d2c-129">Request</span></span>
<span data-ttu-id="d3d2c-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d3d2c-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d3d2c-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d3d2c-132">C#</span><span class="sxs-lookup"><span data-stu-id="d3d2c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3d2c-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3d2c-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d3d2c-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="d3d2c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d3d2c-135">响应</span><span class="sxs-lookup"><span data-stu-id="d3d2c-135">Response</span></span>
<span data-ttu-id="d3d2c-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d3d2c-136">Here is an example of the response.</span></span> 
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
