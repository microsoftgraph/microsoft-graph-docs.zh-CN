---
title: 'post: reply'
description: '在组对话中答复帖子，并向指定线程中添加新帖子。 可以指定 '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8acd39c63901dd90396ff2d44e7f206ece3bfe5a
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072405"
---
# <a name="post-reply"></a><span data-ttu-id="69d25-104">post: reply</span><span class="sxs-lookup"><span data-stu-id="69d25-104">post: reply</span></span>

<span data-ttu-id="69d25-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69d25-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69d25-106">回复帖子，并向组对话中的指定线程添加新帖子。</span><span class="sxs-lookup"><span data-stu-id="69d25-106">Reply to a post and add a new post to the specified thread in a group conversation.</span></span> 

<span data-ttu-id="69d25-107">可以在请求中同时指定父对话和线程，或者仅指定父线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="69d25-107">You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span>

## <a name="permissions"></a><span data-ttu-id="69d25-108">权限</span><span class="sxs-lookup"><span data-stu-id="69d25-108">Permissions</span></span>
<span data-ttu-id="69d25-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="69d25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69d25-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="69d25-111">Permission type</span></span>      | <span data-ttu-id="69d25-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="69d25-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69d25-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69d25-113">Delegated (work or school account)</span></span> | <span data-ttu-id="69d25-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69d25-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="69d25-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69d25-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69d25-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="69d25-116">Not supported.</span></span>    |
|<span data-ttu-id="69d25-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="69d25-117">Application</span></span> | <span data-ttu-id="69d25-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69d25-118">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="69d25-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69d25-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply

```
## <a name="request-headers"></a><span data-ttu-id="69d25-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="69d25-120">Request headers</span></span>
| <span data-ttu-id="69d25-121">标头</span><span class="sxs-lookup"><span data-stu-id="69d25-121">Header</span></span>       | <span data-ttu-id="69d25-122">值</span><span class="sxs-lookup"><span data-stu-id="69d25-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="69d25-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="69d25-123">Authorization</span></span>  | <span data-ttu-id="69d25-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="69d25-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="69d25-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="69d25-126">Request body</span></span>
<span data-ttu-id="69d25-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="69d25-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="69d25-128">参数</span><span class="sxs-lookup"><span data-stu-id="69d25-128">Parameter</span></span>    | <span data-ttu-id="69d25-129">类型</span><span class="sxs-lookup"><span data-stu-id="69d25-129">Type</span></span>   |<span data-ttu-id="69d25-130">说明</span><span class="sxs-lookup"><span data-stu-id="69d25-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69d25-131">帖子</span><span class="sxs-lookup"><span data-stu-id="69d25-131">post</span></span>|[<span data-ttu-id="69d25-132">帖子</span><span class="sxs-lookup"><span data-stu-id="69d25-132">post</span></span>](../resources/post.md)|<span data-ttu-id="69d25-133">正在回复的新帖子。</span><span class="sxs-lookup"><span data-stu-id="69d25-133">The new post that is being replied with.</span></span>|

## <a name="response"></a><span data-ttu-id="69d25-134">响应</span><span class="sxs-lookup"><span data-stu-id="69d25-134">Response</span></span>

<span data-ttu-id="69d25-p104">如果成功，此方法返回 `202 Accepted` 响应代码。它不返回响应正文。</span><span class="sxs-lookup"><span data-stu-id="69d25-p104">If successful, this method returns `202 Accepted` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="69d25-137">示例</span><span class="sxs-lookup"><span data-stu-id="69d25-137">Example</span></span>
<span data-ttu-id="69d25-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="69d25-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="69d25-139">请求</span><span class="sxs-lookup"><span data-stu-id="69d25-139">Request</span></span>
<span data-ttu-id="69d25-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69d25-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="69d25-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="69d25-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/reply
Content-type: application/json
Content-length: 1131

{
  "post": {
    "body": {
      "contentType": "",
      "content": "content-value"
    },
    "receivedDateTime": "2016-10-19T10:37:00Z",
    "hasAttachments": true,
    "from": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "sender": {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    },
    "conversationThreadId": "conversationThreadId-value",
    "newParticipants": [
      {
        "emailAddress": {
          "name": "name-value",
          "address": "address-value"
        }
      }
    ],
    "conversationId": "conversationId-value",
    "createdDateTime": "2016-10-19T10:37:00Z",
    "lastModifiedDateTime": "2016-10-19T10:37:00Z",
    "changeKey": "changeKey-value",
    "categories": [
      "categories-value"
    ],
    "id": "id-value",
    "inReplyTo": {
    },
    "attachments": [
      {
        "@odata.type": "#microsoft.graph.fileAttachment",
        "lastModifiedDateTime": "2016-10-19T10:37:00Z",
        "name": "name-value",
        "contentType": "contentType-value",
        "size": 99,
        "isInline": true,
        "id": "id-value"
      }
    ]
  }
}
```
# <a name="c"></a>[<span data-ttu-id="69d25-142">C#</span><span class="sxs-lookup"><span data-stu-id="69d25-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="69d25-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="69d25-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="69d25-144">Java</span><span class="sxs-lookup"><span data-stu-id="69d25-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="69d25-145">响应</span><span class="sxs-lookup"><span data-stu-id="69d25-145">Response</span></span>
##### <a name="response"></a><span data-ttu-id="69d25-146">响应</span><span class="sxs-lookup"><span data-stu-id="69d25-146">Response</span></span>
<span data-ttu-id="69d25-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="69d25-147">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


