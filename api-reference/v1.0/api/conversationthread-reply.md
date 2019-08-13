---
title: 'conversationThread: reply'
description: '回复组对话中的线程并向其添加新帖子。 您可以指定父对话 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 20ac51d1321341e397e58ce40e70dd45548115a0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327582"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="572f4-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="572f4-104">conversationThread: reply</span></span>

<span data-ttu-id="572f4-p102">回复组对话中的线程并向其添加新帖子。可以在请求中指定父对话，也可以指定线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="572f4-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="572f4-107">权限</span><span class="sxs-lookup"><span data-stu-id="572f4-107">Permissions</span></span>
<span data-ttu-id="572f4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="572f4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="572f4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="572f4-110">Permission type</span></span>      | <span data-ttu-id="572f4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="572f4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="572f4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="572f4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="572f4-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="572f4-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="572f4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="572f4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="572f4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="572f4-115">Not supported.</span></span>    |
|<span data-ttu-id="572f4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="572f4-116">Application</span></span> | <span data-ttu-id="572f4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="572f4-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="572f4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="572f4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="572f4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="572f4-119">Request headers</span></span>
| <span data-ttu-id="572f4-120">标头</span><span class="sxs-lookup"><span data-stu-id="572f4-120">Header</span></span>       | <span data-ttu-id="572f4-121">值</span><span class="sxs-lookup"><span data-stu-id="572f4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="572f4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="572f4-122">Authorization</span></span>  | <span data-ttu-id="572f4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="572f4-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="572f4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="572f4-125">Content-Type</span></span>  | <span data-ttu-id="572f4-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="572f4-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="572f4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="572f4-128">Request body</span></span>
<span data-ttu-id="572f4-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="572f4-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="572f4-130">参数</span><span class="sxs-lookup"><span data-stu-id="572f4-130">Parameter</span></span>    | <span data-ttu-id="572f4-131">类型</span><span class="sxs-lookup"><span data-stu-id="572f4-131">Type</span></span>   |<span data-ttu-id="572f4-132">说明</span><span class="sxs-lookup"><span data-stu-id="572f4-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="572f4-133">帖子</span><span class="sxs-lookup"><span data-stu-id="572f4-133">post</span></span>|[<span data-ttu-id="572f4-134">帖子</span><span class="sxs-lookup"><span data-stu-id="572f4-134">post</span></span>](../resources/post.md)|<span data-ttu-id="572f4-135">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="572f4-135">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="572f4-136">响应</span><span class="sxs-lookup"><span data-stu-id="572f4-136">Response</span></span>

<span data-ttu-id="572f4-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="572f4-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="572f4-139">示例</span><span class="sxs-lookup"><span data-stu-id="572f4-139">Example</span></span>
<span data-ttu-id="572f4-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="572f4-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="572f4-141">请求</span><span class="sxs-lookup"><span data-stu-id="572f4-141">Request</span></span>
<span data-ttu-id="572f4-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="572f4-142">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="572f4-143">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="572f4-143">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="572f4-144">C#</span><span class="sxs-lookup"><span data-stu-id="572f4-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/conversationthread-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="572f4-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="572f4-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/conversationthread-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="572f4-146">Java</span><span class="sxs-lookup"><span data-stu-id="572f4-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/conversationthread-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="572f4-147">响应</span><span class="sxs-lookup"><span data-stu-id="572f4-147">Response</span></span>
<span data-ttu-id="572f4-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="572f4-148">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationThread: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
