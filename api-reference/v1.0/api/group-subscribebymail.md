---
title: 组：subscribeByMail
description: 调用此方法将允许当前用户接收有关该组中新帖子、活动和文件的电子邮件通知。仅支持 Office 365 组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 20321b9f3a7d6558e8229fc33b327b4a8b48068d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373390"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="184a9-104">组：subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="184a9-104">group: subscribeByMail</span></span>
<span data-ttu-id="184a9-p102">调用此方法将允许当前用户接收有关该组中新帖子、活动和文件的电子邮件通知。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="184a9-p102">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="184a9-107">权限</span><span class="sxs-lookup"><span data-stu-id="184a9-107">Permissions</span></span>
<span data-ttu-id="184a9-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="184a9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="184a9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="184a9-110">Permission type</span></span>      | <span data-ttu-id="184a9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="184a9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="184a9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="184a9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="184a9-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="184a9-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="184a9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="184a9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="184a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="184a9-115">Not supported.</span></span>    |
|<span data-ttu-id="184a9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="184a9-116">Application</span></span> | <span data-ttu-id="184a9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="184a9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="184a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="184a9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="184a9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="184a9-119">Request headers</span></span>
| <span data-ttu-id="184a9-120">标头</span><span class="sxs-lookup"><span data-stu-id="184a9-120">Header</span></span>       | <span data-ttu-id="184a9-121">值</span><span class="sxs-lookup"><span data-stu-id="184a9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="184a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="184a9-122">Authorization</span></span>  | <span data-ttu-id="184a9-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="184a9-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="184a9-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="184a9-125">Prefer</span></span> | <span data-ttu-id="184a9-126">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="184a9-126">return=minimal.</span></span> <span data-ttu-id="184a9-127">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="184a9-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="184a9-128">可选。</span><span class="sxs-lookup"><span data-stu-id="184a9-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="184a9-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="184a9-129">Request body</span></span>
<span data-ttu-id="184a9-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="184a9-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="184a9-131">响应</span><span class="sxs-lookup"><span data-stu-id="184a9-131">Response</span></span>
<span data-ttu-id="184a9-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="184a9-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="184a9-134">示例</span><span class="sxs-lookup"><span data-stu-id="184a9-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="184a9-135">请求</span><span class="sxs-lookup"><span data-stu-id="184a9-135">Request</span></span>
<span data-ttu-id="184a9-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="184a9-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="184a9-137">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="184a9-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="184a9-138">C#</span><span class="sxs-lookup"><span data-stu-id="184a9-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="184a9-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="184a9-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="184a9-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="184a9-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="184a9-141">Java</span><span class="sxs-lookup"><span data-stu-id="184a9-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-subscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="184a9-142">响应</span><span class="sxs-lookup"><span data-stu-id="184a9-142">Response</span></span>
<span data-ttu-id="184a9-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="184a9-143">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
