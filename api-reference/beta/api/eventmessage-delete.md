---
title: 删除 eventMessage
description: 删除 eventMessage。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f9a5a55f56e2e4cab47efb95fe33cae07d6b6938
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419844"
---
# <a name="delete-eventmessage"></a><span data-ttu-id="e654a-103">删除 eventMessage</span><span class="sxs-lookup"><span data-stu-id="e654a-103">Delete eventMessage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e654a-104">删除 eventMessage。</span><span class="sxs-lookup"><span data-stu-id="e654a-104">Delete eventMessage.</span></span>
## <a name="permissions"></a><span data-ttu-id="e654a-105">权限</span><span class="sxs-lookup"><span data-stu-id="e654a-105">Permissions</span></span>
<span data-ttu-id="e654a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e654a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e654a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e654a-108">Permission type</span></span>      | <span data-ttu-id="e654a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e654a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e654a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e654a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e654a-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e654a-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e654a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e654a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e654a-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e654a-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="e654a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e654a-114">Application</span></span> | <span data-ttu-id="e654a-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e654a-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e654a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e654a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/messages/{id}
DELETE /users/{id | userPrincipalName}/messages/{id}

DELETE /me/mailFolders/{id}/messages/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e654a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e654a-117">Request headers</span></span>
| <span data-ttu-id="e654a-118">名称</span><span class="sxs-lookup"><span data-stu-id="e654a-118">Name</span></span>       | <span data-ttu-id="e654a-119">类型</span><span class="sxs-lookup"><span data-stu-id="e654a-119">Type</span></span> | <span data-ttu-id="e654a-120">说明</span><span class="sxs-lookup"><span data-stu-id="e654a-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e654a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e654a-121">Authorization</span></span>  | <span data-ttu-id="e654a-122">string</span><span class="sxs-lookup"><span data-stu-id="e654a-122">string</span></span>  | <span data-ttu-id="e654a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e654a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e654a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e654a-125">Request body</span></span>
<span data-ttu-id="e654a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e654a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e654a-127">响应</span><span class="sxs-lookup"><span data-stu-id="e654a-127">Response</span></span>

<span data-ttu-id="e654a-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e654a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e654a-130">示例</span><span class="sxs-lookup"><span data-stu-id="e654a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e654a-131">请求</span><span class="sxs-lookup"><span data-stu-id="e654a-131">Request</span></span>
<span data-ttu-id="e654a-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e654a-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e654a-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e654a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_eventmessage"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/messages/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e654a-134">C#</span><span class="sxs-lookup"><span data-stu-id="e654a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-eventmessage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e654a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e654a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-eventmessage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e654a-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="e654a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-eventmessage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e654a-137">响应</span><span class="sxs-lookup"><span data-stu-id="e654a-137">Response</span></span>
<span data-ttu-id="e654a-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e654a-138">Here is an example of the response.</span></span> 
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
  "description": "Delete eventMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
