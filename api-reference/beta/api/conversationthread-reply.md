---
title: 'conversationThread: reply'
description: '回复组对话中的线程并向其添加新帖子。 您可以指定父对话 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 54609d291180fba6bc771ac2932ff3ef25d5d82f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455343"
---
# <a name="conversationthread-reply"></a><span data-ttu-id="eaa82-104">conversationThread: reply</span><span class="sxs-lookup"><span data-stu-id="eaa82-104">conversationThread: reply</span></span>

<span data-ttu-id="eaa82-p102">回复组对话中的线程并向其添加新帖子。可以在请求中指定父对话，也可以指定线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="eaa82-p102">Reply to a thread in a group conversation and add a new post to it. You can specify the parent conversation in the request, or, you can specify just the thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="eaa82-107">权限</span><span class="sxs-lookup"><span data-stu-id="eaa82-107">Permissions</span></span>
<span data-ttu-id="eaa82-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eaa82-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaa82-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eaa82-110">Permission type</span></span>      | <span data-ttu-id="eaa82-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eaa82-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaa82-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eaa82-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eaa82-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaa82-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="eaa82-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eaa82-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaa82-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eaa82-115">Not supported.</span></span>    |
|<span data-ttu-id="eaa82-116">Application</span><span class="sxs-lookup"><span data-stu-id="eaa82-116">Application</span></span> | <span data-ttu-id="eaa82-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="eaa82-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaa82-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eaa82-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="eaa82-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eaa82-119">Request headers</span></span>
| <span data-ttu-id="eaa82-120">标头</span><span class="sxs-lookup"><span data-stu-id="eaa82-120">Header</span></span>       | <span data-ttu-id="eaa82-121">值</span><span class="sxs-lookup"><span data-stu-id="eaa82-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eaa82-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaa82-122">Authorization</span></span>  | <span data-ttu-id="eaa82-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eaa82-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eaa82-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eaa82-125">Content-Type</span></span>  | <span data-ttu-id="eaa82-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="eaa82-p105">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eaa82-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="eaa82-128">Request body</span></span>
<span data-ttu-id="eaa82-129">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="eaa82-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="eaa82-130">参数</span><span class="sxs-lookup"><span data-stu-id="eaa82-130">Parameter</span></span>    | <span data-ttu-id="eaa82-131">类型</span><span class="sxs-lookup"><span data-stu-id="eaa82-131">Type</span></span>   |<span data-ttu-id="eaa82-132">描述</span><span class="sxs-lookup"><span data-stu-id="eaa82-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eaa82-133">帖子</span><span class="sxs-lookup"><span data-stu-id="eaa82-133">post</span></span>|[<span data-ttu-id="eaa82-134">帖子</span><span class="sxs-lookup"><span data-stu-id="eaa82-134">post</span></span>](../resources/post.md)|<span data-ttu-id="eaa82-135">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="eaa82-135">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="eaa82-136">响应</span><span class="sxs-lookup"><span data-stu-id="eaa82-136">Response</span></span>

<span data-ttu-id="eaa82-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="eaa82-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaa82-139">示例</span><span class="sxs-lookup"><span data-stu-id="eaa82-139">Example</span></span>
<span data-ttu-id="eaa82-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="eaa82-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="eaa82-141">请求</span><span class="sxs-lookup"><span data-stu-id="eaa82-141">Request</span></span>
<span data-ttu-id="eaa82-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eaa82-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="eaa82-143">响应</span><span class="sxs-lookup"><span data-stu-id="eaa82-143">Response</span></span>
<span data-ttu-id="eaa82-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="eaa82-144">Here is an example of the response.</span></span>
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
