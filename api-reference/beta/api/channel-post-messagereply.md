---
title: 在频道中回复消息
description: 回复频道中的现有消息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b7c9e4b706e848218d55ab1898a03096f2d5aba9
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201097"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="acf99-103">在频道中回复消息</span><span class="sxs-lookup"><span data-stu-id="acf99-103">Reply to a message in a channel</span></span>

<span data-ttu-id="acf99-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acf99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acf99-105">在指定的频道中创建新的 [chatMessage](../resources/chatmessage.md) [回复](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="acf99-105">Create a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="acf99-106">**注意**：使用 Microsoft Teams [](/legal/microsoft-apis/terms-of-use)作为 microsoft Teams 日志文件。</span><span class="sxs-lookup"><span data-stu-id="acf99-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="acf99-107">仅发送用户将阅读的邮件。</span><span class="sxs-lookup"><span data-stu-id="acf99-107">Only send messages that people will read.</span></span>
<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD001 -->

## <a name="permissions"></a><span data-ttu-id="acf99-108">权限</span><span class="sxs-lookup"><span data-stu-id="acf99-108">Permissions</span></span>
<span data-ttu-id="acf99-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="acf99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="acf99-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="acf99-111">Permission type</span></span>                        | <span data-ttu-id="acf99-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="acf99-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="acf99-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="acf99-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="acf99-114">ChannelMessage.Send、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acf99-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="acf99-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="acf99-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acf99-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="acf99-116">Not supported.</span></span> |
| <span data-ttu-id="acf99-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="acf99-117">Application</span></span>                            | <span data-ttu-id="acf99-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="acf99-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="acf99-119">**注意**：仅迁移 *支持应用程序*[权限](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)。</span><span class="sxs-lookup"><span data-stu-id="acf99-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="acf99-120">将来，Microsoft 可能要求你或你的客户根据导入的数据量支付其他费用。</span><span class="sxs-lookup"><span data-stu-id="acf99-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="acf99-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="acf99-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="acf99-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="acf99-122">Request headers</span></span>
| <span data-ttu-id="acf99-123">名称</span><span class="sxs-lookup"><span data-stu-id="acf99-123">Name</span></span>       | <span data-ttu-id="acf99-124">类型</span><span class="sxs-lookup"><span data-stu-id="acf99-124">Type</span></span> | <span data-ttu-id="acf99-125">说明</span><span class="sxs-lookup"><span data-stu-id="acf99-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="acf99-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="acf99-126">Authorization</span></span>  | <span data-ttu-id="acf99-127">string</span><span class="sxs-lookup"><span data-stu-id="acf99-127">string</span></span>  | <span data-ttu-id="acf99-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="acf99-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="acf99-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="acf99-130">Request body</span></span>
<span data-ttu-id="acf99-131">在请求正文中，提供 message 对象的 JSON [表示](../resources/chatmessage.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="acf99-131">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="acf99-132">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="acf99-132">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="acf99-133">响应</span><span class="sxs-lookup"><span data-stu-id="acf99-133">Response</span></span>

<span data-ttu-id="acf99-134">如果成功，此方法返回 `201 Created` 包含已创建 [消息的响应](../resources/chatmessage.md) 代码。</span><span class="sxs-lookup"><span data-stu-id="acf99-134">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="acf99-135">示例</span><span class="sxs-lookup"><span data-stu-id="acf99-135">Examples</span></span>

### <a name="example-1-create-a-new-reply-to-a-chatmessage"></a><span data-ttu-id="acf99-136">示例 1：创建对 chatMessage 的新回复</span><span class="sxs-lookup"><span data-stu-id="acf99-136">Example 1: Create a new reply to a chatMessage</span></span>

<span data-ttu-id="acf99-137">有关示例的更全面的列表，请参阅在频道或[聊天中创建 chatMessage。](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="acf99-137">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

#### <a name="request"></a><span data-ttu-id="acf99-138">请求</span><span class="sxs-lookup"><span data-stu-id="acf99-138">Request</span></span>
<span data-ttu-id="acf99-139">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="acf99-139">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="acf99-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="acf99-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

# <a name="c"></a>[<span data-ttu-id="acf99-141">C#</span><span class="sxs-lookup"><span data-stu-id="acf99-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-reply-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acf99-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acf99-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-reply-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acf99-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acf99-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-reply-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="acf99-144">Java</span><span class="sxs-lookup"><span data-stu-id="acf99-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-reply-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="acf99-145">响应</span><span class="sxs-lookup"><span data-stu-id="acf99-145">Response</span></span>

<span data-ttu-id="acf99-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="acf99-146">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages('1590776551682')/replies/$entity",
    "id": "1591039710682",
    "replyToId": "1590776551682",
    "etag": "1591039710682",
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
            "id": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
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

### <a name="example-2-import-messages"></a><span data-ttu-id="acf99-147">示例 2：导入邮件</span><span class="sxs-lookup"><span data-stu-id="acf99-147">Example 2: Import messages</span></span>

> <span data-ttu-id="acf99-148">**注意**：此方案 `Teamwork.Migrate.All` 需要权限范围。</span><span class="sxs-lookup"><span data-stu-id="acf99-148">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="acf99-149">请求</span><span class="sxs-lookup"><span data-stu-id="acf99-149">Request</span></span>

<span data-ttu-id="acf99-150">以下示例显示如何使用 请求正文中的 和 键导入 `createDateTime` `from` 实时邮件。</span><span class="sxs-lookup"><span data-stu-id="acf99-150">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
         "displayName":"Joh Doe"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   }
}
```

---
#### <a name="response"></a><span data-ttu-id="acf99-151">响应</span><span class="sxs-lookup"><span data-stu-id="acf99-151">Response</span></span>

<span data-ttu-id="acf99-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="acf99-152">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages('1590776551682')/replies/$entity",
   "id":"1591039710682",
   "replyToId":"1590776551682",
   "etag":"1591039710682",
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
         "id":"8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
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
