---
title: 'conversationThread: reply'
description: '答复在组对话中的线程并向其添加新文章。 您可以指定父对话 '
author: dkershaw10
ms.openlocfilehash: 196a28c5b8a5ae2bfa98a2cbfd4aa0d120cbceef
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/22/2018
ms.locfileid: "27413181"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="6cb77-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="6cb77-104">conversationThread: reply</span></span>

> <span data-ttu-id="6cb77-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6cb77-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cb77-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6cb77-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6cb77-p103">回复组对话中的线程并向其添加新帖子。可以在请求中指定父对话，也可以指定线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="6cb77-p103">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="6cb77-109">权限</span><span class="sxs-lookup"><span data-stu-id="6cb77-109">Permissions</span></span>
<span data-ttu-id="6cb77-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6cb77-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cb77-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6cb77-112">Permission type</span></span>      | <span data-ttu-id="6cb77-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6cb77-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cb77-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6cb77-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6cb77-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cb77-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6cb77-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6cb77-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cb77-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cb77-117">Not supported.</span></span>    |
|<span data-ttu-id="6cb77-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6cb77-118">Application</span></span> | <span data-ttu-id="6cb77-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6cb77-119">Not supported.</span></span>    |

## <a name="http-request"></a><span data-ttu-id="6cb77-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6cb77-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="6cb77-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="6cb77-121">Request headers</span></span>
| <span data-ttu-id="6cb77-122">标头</span><span class="sxs-lookup"><span data-stu-id="6cb77-122">Header</span></span>       | <span data-ttu-id="6cb77-123">值</span><span class="sxs-lookup"><span data-stu-id="6cb77-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6cb77-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cb77-124">Authorization</span></span>  | <span data-ttu-id="6cb77-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6cb77-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6cb77-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6cb77-127">Content-Type</span></span>  | <span data-ttu-id="6cb77-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6cb77-p106">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6cb77-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="6cb77-130">Request body</span></span>
<span data-ttu-id="6cb77-131">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="6cb77-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6cb77-132">参数</span><span class="sxs-lookup"><span data-stu-id="6cb77-132">Parameter</span></span>    | <span data-ttu-id="6cb77-133">类型</span><span class="sxs-lookup"><span data-stu-id="6cb77-133">Type</span></span>   |<span data-ttu-id="6cb77-134">说明</span><span class="sxs-lookup"><span data-stu-id="6cb77-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cb77-135">帖子</span><span class="sxs-lookup"><span data-stu-id="6cb77-135">post</span></span>|[<span data-ttu-id="6cb77-136">帖子</span><span class="sxs-lookup"><span data-stu-id="6cb77-136">post</span></span>](../resources/post.md)|<span data-ttu-id="6cb77-137">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="6cb77-137">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="6cb77-138">响应</span><span class="sxs-lookup"><span data-stu-id="6cb77-138">Response</span></span>

<span data-ttu-id="6cb77-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6cb77-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cb77-141">示例</span><span class="sxs-lookup"><span data-stu-id="6cb77-141">Example</span></span>
<span data-ttu-id="6cb77-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="6cb77-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6cb77-143">请求</span><span class="sxs-lookup"><span data-stu-id="6cb77-143">Request</span></span>
<span data-ttu-id="6cb77-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6cb77-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "conversationthread_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/reply
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

##### <a name="response"></a><span data-ttu-id="6cb77-145">响应</span><span class="sxs-lookup"><span data-stu-id="6cb77-145">Response</span></span>
<span data-ttu-id="6cb77-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6cb77-146">Here is an example of the response.</span></span>
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
  "tocPath": ""
}-->
