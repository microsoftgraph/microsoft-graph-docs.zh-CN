---
title: 'conversationThread: reply'
description: '回复组对话中的线程并向其添加新帖子。 您可以指定父对话 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7d08673808fb67f7c6feb640a5dc3c81057e6f92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518166"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="567c7-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="567c7-104">conversationThread: reply</span></span>

<span data-ttu-id="567c7-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="567c7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="567c7-p102">回复组对话中的线程并向其添加新帖子。可以在请求中指定父对话，也可以指定线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="567c7-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="567c7-108">权限</span><span class="sxs-lookup"><span data-stu-id="567c7-108">Permissions</span></span>
<span data-ttu-id="567c7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="567c7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="567c7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="567c7-111">Permission type</span></span>      | <span data-ttu-id="567c7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="567c7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="567c7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="567c7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="567c7-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="567c7-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="567c7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="567c7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="567c7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="567c7-116">Not supported.</span></span>    |
|<span data-ttu-id="567c7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="567c7-117">Application</span></span> | <span data-ttu-id="567c7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="567c7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="567c7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="567c7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="567c7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="567c7-120">Request headers</span></span>
| <span data-ttu-id="567c7-121">标头</span><span class="sxs-lookup"><span data-stu-id="567c7-121">Header</span></span>       | <span data-ttu-id="567c7-122">值</span><span class="sxs-lookup"><span data-stu-id="567c7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="567c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="567c7-123">Authorization</span></span>  | <span data-ttu-id="567c7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="567c7-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="567c7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="567c7-126">Content-Type</span></span>  | <span data-ttu-id="567c7-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="567c7-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="567c7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="567c7-129">Request body</span></span>
<span data-ttu-id="567c7-130">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="567c7-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="567c7-131">参数</span><span class="sxs-lookup"><span data-stu-id="567c7-131">Parameter</span></span>    | <span data-ttu-id="567c7-132">类型</span><span class="sxs-lookup"><span data-stu-id="567c7-132">Type</span></span>   |<span data-ttu-id="567c7-133">说明</span><span class="sxs-lookup"><span data-stu-id="567c7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="567c7-134">帖子</span><span class="sxs-lookup"><span data-stu-id="567c7-134">post</span></span>|[<span data-ttu-id="567c7-135">帖子</span><span class="sxs-lookup"><span data-stu-id="567c7-135">post</span></span>](../resources/post.md)|<span data-ttu-id="567c7-136">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="567c7-136">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="567c7-137">响应</span><span class="sxs-lookup"><span data-stu-id="567c7-137">Response</span></span>

<span data-ttu-id="567c7-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="567c7-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="567c7-140">示例</span><span class="sxs-lookup"><span data-stu-id="567c7-140">Example</span></span>
<span data-ttu-id="567c7-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="567c7-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="567c7-142">请求</span><span class="sxs-lookup"><span data-stu-id="567c7-142">Request</span></span>
<span data-ttu-id="567c7-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="567c7-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="567c7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="567c7-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="567c7-145">C#</span><span class="sxs-lookup"><span data-stu-id="567c7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/conversationthread-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="567c7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="567c7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/conversationthread-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="567c7-147">Java</span><span class="sxs-lookup"><span data-stu-id="567c7-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/conversationthread-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="567c7-148">响应</span><span class="sxs-lookup"><span data-stu-id="567c7-148">Response</span></span>
<span data-ttu-id="567c7-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="567c7-149">Here is an example of the response.</span></span>
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
