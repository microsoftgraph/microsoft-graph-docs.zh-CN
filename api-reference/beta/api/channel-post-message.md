---
title: 在频道中创建 chatMessage
description: 在指定的频道中创建新的了 chatmessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f7bdb9322b59e78b5b5fe363cccd0713314f3a70
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959148"
---
# <a name="create-chatmessage-in-channel"></a><span data-ttu-id="73d16-103">在信道中创建了 chatmessage</span><span class="sxs-lookup"><span data-stu-id="73d16-103">Create chatMessage in channel</span></span>

<span data-ttu-id="73d16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73d16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73d16-105">在指定的[频道](../resources/channel.md)中创建新的[了 chatmessage](../resources/chatmessage.md) 。</span><span class="sxs-lookup"><span data-stu-id="73d16-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="73d16-106">**注意** ：我们建议您不要使用此 API 进行数据迁移。</span><span class="sxs-lookup"><span data-stu-id="73d16-106">**Note** : We don't recommend that you use this API for data migration.</span></span> <span data-ttu-id="73d16-107">它不具有典型迁移所需的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="73d16-107">It does not have the throughput necessary for a typical migration.</span></span>

> <span data-ttu-id="73d16-108">**注意** ：违反使用 Microsoft 团队作为日志文件的 [使用条款](/legal/microsoft-apis/terms-of-use) 。</span><span class="sxs-lookup"><span data-stu-id="73d16-108">**Note** : It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="73d16-109">仅发送人员将阅读的邮件。</span><span class="sxs-lookup"><span data-stu-id="73d16-109">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="73d16-110">权限</span><span class="sxs-lookup"><span data-stu-id="73d16-110">Permissions</span></span>

<span data-ttu-id="73d16-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73d16-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73d16-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="73d16-113">Permission type</span></span>                        | <span data-ttu-id="73d16-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73d16-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="73d16-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73d16-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="73d16-116">ChannelMessage、Group、Group 写。 All</span><span class="sxs-lookup"><span data-stu-id="73d16-116">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="73d16-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73d16-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73d16-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="73d16-118">Not supported.</span></span> |
| <span data-ttu-id="73d16-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="73d16-119">Application</span></span>                            | <span data-ttu-id="73d16-120">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="73d16-120">Teamwork.Migrate.All</span></span> |

<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->

## <a name="http-request"></a><span data-ttu-id="73d16-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73d16-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="73d16-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="73d16-122">Request headers</span></span>

| <span data-ttu-id="73d16-123">名称</span><span class="sxs-lookup"><span data-stu-id="73d16-123">Name</span></span>          | <span data-ttu-id="73d16-124">说明</span><span class="sxs-lookup"><span data-stu-id="73d16-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="73d16-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="73d16-125">Authorization</span></span> | <span data-ttu-id="73d16-126">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="73d16-126">Bearer {code}.</span></span> <span data-ttu-id="73d16-127">必需。</span><span class="sxs-lookup"><span data-stu-id="73d16-127">Required.</span></span> |
| <span data-ttu-id="73d16-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="73d16-128">Content-type</span></span> | <span data-ttu-id="73d16-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="73d16-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73d16-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="73d16-131">Request body</span></span>

<span data-ttu-id="73d16-132">在请求正文中，提供 [了 chatmessage](../resources/chatmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73d16-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="73d16-133">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="73d16-133">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="73d16-134">响应</span><span class="sxs-lookup"><span data-stu-id="73d16-134">Response</span></span>

<span data-ttu-id="73d16-135">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [了 chatmessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73d16-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73d16-136">示例</span><span class="sxs-lookup"><span data-stu-id="73d16-136">Examples</span></span>

### <a name="example-1-create-a-message-in-a-specified-channel"></a><span data-ttu-id="73d16-137">示例1：在指定的频道中创建邮件</span><span class="sxs-lookup"><span data-stu-id="73d16-137">Example 1: Create a message in a specified channel</span></span>

<span data-ttu-id="73d16-138">有关示例的更完整列表，请参阅 [Create 了 chatmessage in a 信道 or chat](chatmessage-post.md)。</span><span class="sxs-lookup"><span data-stu-id="73d16-138">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="73d16-139">请求</span><span class="sxs-lookup"><span data-stu-id="73d16-139">Request</span></span>
<span data-ttu-id="73d16-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73d16-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="73d16-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="73d16-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```

# <a name="c"></a>[<span data-ttu-id="73d16-142">C#</span><span class="sxs-lookup"><span data-stu-id="73d16-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="73d16-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73d16-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="73d16-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="73d16-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="73d16-145">Java</span><span class="sxs-lookup"><span data-stu-id="73d16-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="73d16-146">响应</span><span class="sxs-lookup"><span data-stu-id="73d16-146">Response</span></span>

<span data-ttu-id="73d16-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73d16-147">The following is an example of the response.</span></span>

> <span data-ttu-id="73d16-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="73d16-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
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

### <a name="example-2-import-messages-text-only"></a><span data-ttu-id="73d16-150">示例2： (纯文本) 中导入邮件</span><span class="sxs-lookup"><span data-stu-id="73d16-150">Example 2: Import messages (text only)</span></span>

> <span data-ttu-id="73d16-151">**注意** ： `Teamwork.Migrate.All` 此方案需要权限范围。</span><span class="sxs-lookup"><span data-stu-id="73d16-151">**Note** : The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="73d16-152">请求</span><span class="sxs-lookup"><span data-stu-id="73d16-152">Request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="73d16-153">下面的示例展示了如何使用 `createDateTime` 请求正文中的和键导入时消息 `from` 。</span><span class="sxs-lookup"><span data-stu-id="73d16-153">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/messages

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

### <a name="response"></a><span data-ttu-id="73d16-154">响应</span><span class="sxs-lookup"><span data-stu-id="73d16-154">Response</span></span>

<span data-ttu-id="73d16-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73d16-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('teamId')/channels('channelId')/messages/$entity",
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

### <a name="example-3-import-messages-with-inline-images"></a><span data-ttu-id="73d16-156">示例3：使用内嵌图像导入邮件</span><span class="sxs-lookup"><span data-stu-id="73d16-156">Example 3: Import messages with inline images</span></span>

> [!NOTE]
> <span data-ttu-id="73d16-157">目前，内嵌图像是导入邮件 API 架构所支持的唯一媒体类型。</span><span class="sxs-lookup"><span data-stu-id="73d16-157">Currently, inline images are the only media type supported by the import message API schema.</span></span>

> <span data-ttu-id="73d16-158">**注意** ： `Teamwork.Migrate.All` 此方案需要权限范围。</span><span class="sxs-lookup"><span data-stu-id="73d16-158">**Note** : The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="73d16-159">请求</span><span class="sxs-lookup"><span data-stu-id="73d16-159">Request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="73d16-160">下面的示例演示如何使用 `createDateTime` 请求正文中的和键导入包含内嵌图像的 "正在运行的邮件" `from` 。</span><span class="sxs-lookup"><span data-stu-id="73d16-160">The following example shows how to import back-in-time messages containing inline images using the `createDateTime` and `from` keys in the request body.</span></span>

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/messages

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"id-value",
         "displayName":"John Doe",
         "userIdentityType":"aadUser"
      }
   },
{
   "body":{
      "contentType":"html",
      "content":"<div><div>\n<div><span><img height=\"250\" src=\"../hostedContents/1/$value\" width=\"176.2295081967213\" style=\"vertical-align:bottom; width:176px; height:250px\"></span>\n\n</div>\n\n\n</div>\n</div>"
   },
   "hostedContents":[
      {
         "@microsoft.graph.temporaryId":"1",
         "contentBytes":"iVBORw0KGgoAAAANSUhEUgAAANcAAAExCAYAAADvFzeeAAAXjklEQVR4Ae2d/XNU1RnH+9e0FFrA0RCIyaS8hRA0HV5KbS1gHRgVpjMClY4GHJ3yYm1HCmXaWttaaZUZtIIFKYi8lFAkvOQ9u5vN225IARVBbX9/Os9NbrLZbMjmhCfJPX5+2Lmb3T25y3O+n/M599x7w9f+++UXwoMakIF7n4GvUdR7X1RqSk01A8CFuZm5GGUAuIwKi72wF3ABF+YyygBwGRUWc2Eu4AIuzGWUAeAyKizmwlzABVyYyygDwGVUWMyFuYALuDCXUQaAy6iwmAtzARdwfWXMdeuzT+TGxz3Sfb1LunrapL07IW3pePDQ5/qavqef0c+OdYAELuAac4jGGkLL9rdvfyo9N9ODQAqBGmmrwGlb/R0u3xG4gMspOC5hG882CoRaaCSA8n1ff9doIQMu4PIOrus3u+8ZVNnw6e/Od5AALuDKOyz5hmqiPnfnzi1J9bSbgRWCpvvQfY307wQu4BoxJCOFaDK8rwsQmQsUIQhWW93XSIsewAVckYdLQ24F0Ui/926AARdwRRounZ6Np7GyYdN9DzdFBC7gijRc43GMlQ1U9s/6HXJNjYELuHI<<-----Removed----->>>>",
         "contentType":"image/png"
      }
   ]
}
```

#### <a name="response"></a><span data-ttu-id="73d16-161">响应</span><span class="sxs-lookup"><span data-stu-id="73d16-161">Response</span></span>

<span data-ttu-id="73d16-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73d16-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('teamId')/channels('channelId')/messages/$entity",
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
      "content":"<div><div>\n<div><span><img height=\"250\" src=\"https://graph.microsoft.com/teams/teamId/channels/channelId/messages/id-value/hostedContents/hostedContentId/$value\" width=\"176.2295081967213\" style=\"vertical-align:bottom; width:176px; height:250px\"></span>\n\n</div>\n\n\n</div>\n</div>"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}

```

## <a name="see-also"></a><span data-ttu-id="73d16-163">另请参阅</span><span class="sxs-lookup"><span data-stu-id="73d16-163">See also</span></span>

* [<span data-ttu-id="73d16-164">使用 Microsoft Graph 将第三方平台消息导入 Teams</span><span class="sxs-lookup"><span data-stu-id="73d16-164">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="73d16-165">创建频道</span><span class="sxs-lookup"><span data-stu-id="73d16-165">Create channel</span></span>](channel-post.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Send message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
