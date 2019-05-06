---
title: 'conversationThread: reply'
description: '回复组对话中的线程并向其添加新帖子。 您可以指定父对话 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0500a51d582dcd728b7c0807d22ef4e58e4c5db7
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33591789"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="e3c55-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="e3c55-104">conversationThread: reply</span></span>

<span data-ttu-id="e3c55-p102">回复组对话中的线程并向其添加新帖子。可以在请求中指定父对话，也可以指定线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="e3c55-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3c55-107">权限</span><span class="sxs-lookup"><span data-stu-id="e3c55-107">Permissions</span></span>
<span data-ttu-id="e3c55-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3c55-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3c55-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3c55-110">Permission type</span></span>      | <span data-ttu-id="e3c55-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e3c55-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3c55-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3c55-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e3c55-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3c55-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e3c55-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3c55-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3c55-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3c55-115">Not supported.</span></span>    |
|<span data-ttu-id="e3c55-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3c55-116">Application</span></span> | <span data-ttu-id="e3c55-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3c55-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3c55-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3c55-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="e3c55-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3c55-119">Request headers</span></span>
| <span data-ttu-id="e3c55-120">标头</span><span class="sxs-lookup"><span data-stu-id="e3c55-120">Header</span></span>       | <span data-ttu-id="e3c55-121">值</span><span class="sxs-lookup"><span data-stu-id="e3c55-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e3c55-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3c55-122">Authorization</span></span>  | <span data-ttu-id="e3c55-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e3c55-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e3c55-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e3c55-125">Content-Type</span></span>  | <span data-ttu-id="e3c55-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e3c55-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e3c55-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3c55-128">Request body</span></span>
<span data-ttu-id="e3c55-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="e3c55-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e3c55-130">参数</span><span class="sxs-lookup"><span data-stu-id="e3c55-130">Parameter</span></span>    | <span data-ttu-id="e3c55-131">类型</span><span class="sxs-lookup"><span data-stu-id="e3c55-131">Type</span></span>   |<span data-ttu-id="e3c55-132">说明</span><span class="sxs-lookup"><span data-stu-id="e3c55-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3c55-133">帖子</span><span class="sxs-lookup"><span data-stu-id="e3c55-133">post</span></span>|[<span data-ttu-id="e3c55-134">帖子</span><span class="sxs-lookup"><span data-stu-id="e3c55-134">post</span></span>](../resources/post.md)|<span data-ttu-id="e3c55-135">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="e3c55-135">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="e3c55-136">响应</span><span class="sxs-lookup"><span data-stu-id="e3c55-136">Response</span></span>

<span data-ttu-id="e3c55-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e3c55-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3c55-139">示例</span><span class="sxs-lookup"><span data-stu-id="e3c55-139">Example</span></span>
<span data-ttu-id="e3c55-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="e3c55-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e3c55-141">请求</span><span class="sxs-lookup"><span data-stu-id="e3c55-141">Request</span></span>
<span data-ttu-id="e3c55-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e3c55-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    }
  }
}
```

##### <a name="response"></a><span data-ttu-id="e3c55-143">响应</span><span class="sxs-lookup"><span data-stu-id="e3c55-143">Response</span></span>
<span data-ttu-id="e3c55-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e3c55-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e3c55-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e3c55-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e3c55-146">语言</span><span class="sxs-lookup"><span data-stu-id="e3c55-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/conversationthread_reply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e3c55-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="e3c55-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/conversationthread_reply-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/conversationthread-reply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/conversationthread-reply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
