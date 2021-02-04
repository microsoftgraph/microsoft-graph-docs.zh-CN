---
title: 在频道中回复消息
description: 回复频道中的现有邮件。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: db0164be77260c60c2d89c726b048b4af8dc741d
ms.sourcegitcommit: d02c438bcd58e8f64bfcd5fba0b40e436b46570e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/04/2021
ms.locfileid: "50101900"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="304da-103">在频道中回复消息</span><span class="sxs-lookup"><span data-stu-id="304da-103">Reply to a message in a channel</span></span>

<span data-ttu-id="304da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="304da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="304da-105">在指定的频道中创建新的 [chatMessage](../resources/chatmessage.md) [回复](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="304da-105">Create a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="304da-106">**注意**：使用 Microsoft Teams [](/legal/microsoft-apis/terms-of-use)作为 microsoft Teams 日志文件。</span><span class="sxs-lookup"><span data-stu-id="304da-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="304da-107">仅发送用户将阅读的邮件。</span><span class="sxs-lookup"><span data-stu-id="304da-107">Only send messages that people will read.</span></span>
<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD001 -->

## <a name="permissions"></a><span data-ttu-id="304da-108">权限</span><span class="sxs-lookup"><span data-stu-id="304da-108">Permissions</span></span>
<span data-ttu-id="304da-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="304da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="304da-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="304da-111">Permission type</span></span>                        | <span data-ttu-id="304da-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="304da-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="304da-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="304da-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="304da-114">ChannelMessage.Send、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="304da-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="304da-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="304da-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="304da-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="304da-116">Not supported.</span></span> |
| <span data-ttu-id="304da-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="304da-117">Application</span></span>                            | <span data-ttu-id="304da-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="304da-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="304da-119">**注意**：应用程序权限仅 *受* 迁移 [支持](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)。</span><span class="sxs-lookup"><span data-stu-id="304da-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>

## <a name="http-request"></a><span data-ttu-id="304da-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="304da-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="304da-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="304da-121">Request headers</span></span>
| <span data-ttu-id="304da-122">名称</span><span class="sxs-lookup"><span data-stu-id="304da-122">Name</span></span>       | <span data-ttu-id="304da-123">类型</span><span class="sxs-lookup"><span data-stu-id="304da-123">Type</span></span> | <span data-ttu-id="304da-124">说明</span><span class="sxs-lookup"><span data-stu-id="304da-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="304da-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="304da-125">Authorization</span></span>  | <span data-ttu-id="304da-126">string</span><span class="sxs-lookup"><span data-stu-id="304da-126">string</span></span>  | <span data-ttu-id="304da-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="304da-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="304da-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="304da-129">Request body</span></span>
<span data-ttu-id="304da-130">在请求正文中，提供邮件对象的 JSON [表示形式](../resources/chatmessage.md) 。</span><span class="sxs-lookup"><span data-stu-id="304da-130">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="304da-131">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="304da-131">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="304da-132">响应</span><span class="sxs-lookup"><span data-stu-id="304da-132">Response</span></span>

<span data-ttu-id="304da-133">如果成功，此方法返回 `201 Created` 包含已创建 [消息的响应](../resources/chatmessage.md) 代码。</span><span class="sxs-lookup"><span data-stu-id="304da-133">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="example-1-create-a-new-reply-to-a-chatmessage"></a><span data-ttu-id="304da-134">示例 1：创建 chatMessage 的新回复</span><span class="sxs-lookup"><span data-stu-id="304da-134">Example 1: Create a new reply to a chatMessage</span></span>

<span data-ttu-id="304da-135">有关示例的更全面的列表，请参阅在频道[或聊天中创建 chatMessage。](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="304da-135">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="304da-136">请求</span><span class="sxs-lookup"><span data-stu-id="304da-136">Request</span></span>
<span data-ttu-id="304da-137">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="304da-137">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="304da-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="304da-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

# <a name="c"></a>[<span data-ttu-id="304da-139">C#</span><span class="sxs-lookup"><span data-stu-id="304da-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="304da-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="304da-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="304da-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="304da-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="304da-142">Java</span><span class="sxs-lookup"><span data-stu-id="304da-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="304da-143">响应</span><span class="sxs-lookup"><span data-stu-id="304da-143">Response</span></span>

<span data-ttu-id="304da-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="304da-144">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages('id-value')/replies/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
    "lastEditedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "id-value",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-import-messages"></a><span data-ttu-id="304da-145">示例 2：导入邮件</span><span class="sxs-lookup"><span data-stu-id="304da-145">Example 2: Import messages</span></span>

> <span data-ttu-id="304da-146">**注意**：此方案 `Teamwork.Migrate.All` 需要权限范围。</span><span class="sxs-lookup"><span data-stu-id="304da-146">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="304da-147">请求</span><span class="sxs-lookup"><span data-stu-id="304da-147">Request</span></span>

<span data-ttu-id="304da-148">以下示例显示如何使用请求正文中的 and 键导入返回 `createDateTime` `from` 时间邮件。</span><span class="sxs-lookup"><span data-stu-id="304da-148">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/messages/{messageId}/replies

{
   "replyToId":null,
   "messageType":"message",
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "lastModifiedDateTime":null,
   "deleted":false,
   "subject":null,
   "summary":null,
   "importance":"normal",
   "locale":"en-us",
   "policyViolation":null,
   "from":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"id-value",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}
```

---
#### <a name="response"></a><span data-ttu-id="304da-149">响应</span><span class="sxs-lookup"><span data-stu-id="304da-149">Response</span></span>

<span data-ttu-id="304da-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="304da-150">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams/{teamId}/channels/{channelId}/messages/$entity",
   "id":"id-value",
   "replyToId":null,
   "etag":"id-value",
   "messageType":"message",
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "lastModifiedDateTime":null,
   "deleted":false,
   "subject":null,
   "summary":null,
   "importance":"normal",
   "locale":"en-us",
   "policyViolation":null,
   "from":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"id-value",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a reply message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
