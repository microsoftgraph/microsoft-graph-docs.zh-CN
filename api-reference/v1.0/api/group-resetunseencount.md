---
title: 组：resetUnseenCount
description: 重置当前用户自上次访问后未查看的所有帖子的 unseenCount。仅支持 Office 365 组。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 790fc7f1e1e457789ed677c4fb544da3f597cb19
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885359"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="4db98-104">组：resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="4db98-104">group: resetUnseenCount</span></span>
<span data-ttu-id="4db98-p102">重置当前用户自上次访问后未查看的所有帖子的 unseenCount。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="4db98-p102">Reset the unseenCount of all the posts that the current user has not seen since their last visit. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="4db98-107">权限</span><span class="sxs-lookup"><span data-stu-id="4db98-107">Permissions</span></span>
<span data-ttu-id="4db98-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4db98-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4db98-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4db98-110">Permission type</span></span>      | <span data-ttu-id="4db98-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4db98-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4db98-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4db98-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4db98-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4db98-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4db98-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4db98-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4db98-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4db98-115">Not supported.</span></span>    |
|<span data-ttu-id="4db98-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4db98-116">Application</span></span> | <span data-ttu-id="4db98-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4db98-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4db98-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4db98-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="4db98-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4db98-119">Request headers</span></span>
| <span data-ttu-id="4db98-120">标头</span><span class="sxs-lookup"><span data-stu-id="4db98-120">Header</span></span>       | <span data-ttu-id="4db98-121">值</span><span class="sxs-lookup"><span data-stu-id="4db98-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4db98-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4db98-122">Authorization</span></span>  | <span data-ttu-id="4db98-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4db98-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4db98-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="4db98-125">Prefer</span></span> | <span data-ttu-id="4db98-126">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="4db98-126">return=minimal.</span></span> <span data-ttu-id="4db98-127">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="4db98-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="4db98-128">可选。</span><span class="sxs-lookup"><span data-stu-id="4db98-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="4db98-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4db98-129">Request body</span></span>
<span data-ttu-id="4db98-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4db98-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4db98-131">响应</span><span class="sxs-lookup"><span data-stu-id="4db98-131">Response</span></span>
<span data-ttu-id="4db98-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4db98-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4db98-134">示例</span><span class="sxs-lookup"><span data-stu-id="4db98-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4db98-135">请求</span><span class="sxs-lookup"><span data-stu-id="4db98-135">Request</span></span>
<span data-ttu-id="4db98-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4db98-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4db98-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4db98-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4db98-138">C#</span><span class="sxs-lookup"><span data-stu-id="4db98-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-resetunseencount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4db98-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="4db98-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-resetunseencount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4db98-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="4db98-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-resetunseencount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4db98-141">Java</span><span class="sxs-lookup"><span data-stu-id="4db98-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-resetunseencount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4db98-142">响应</span><span class="sxs-lookup"><span data-stu-id="4db98-142">Response</span></span>
<span data-ttu-id="4db98-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4db98-143">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
