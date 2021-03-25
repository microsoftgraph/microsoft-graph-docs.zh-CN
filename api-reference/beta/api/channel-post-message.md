---
title: 在频道中创建 chatMessage
description: 在指定的频道中创建新的 chatMessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 97b0b0d2db2ad813440d034f0cb3ae47149f24bb
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200945"
---
# <a name="create-chatmessage-in-channel"></a><span data-ttu-id="c13ed-103">在频道中创建 chatMessage</span><span class="sxs-lookup"><span data-stu-id="c13ed-103">Create chatMessage in channel</span></span>

<span data-ttu-id="c13ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c13ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c13ed-105">在指定的[频道中创建新的 chatMessage。](../resources/chatmessage.md) [](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="c13ed-105">Create a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="c13ed-106">**注意**：使用 Microsoft Teams [](/legal/microsoft-apis/terms-of-use)作为 microsoft Teams 日志文件。</span><span class="sxs-lookup"><span data-stu-id="c13ed-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="c13ed-107">仅发送用户将阅读的邮件。</span><span class="sxs-lookup"><span data-stu-id="c13ed-107">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="c13ed-108">权限</span><span class="sxs-lookup"><span data-stu-id="c13ed-108">Permissions</span></span>

<span data-ttu-id="c13ed-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c13ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c13ed-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c13ed-111">Permission type</span></span>                        | <span data-ttu-id="c13ed-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c13ed-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c13ed-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c13ed-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c13ed-114">ChannelMessage.Send、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c13ed-114">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="c13ed-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c13ed-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c13ed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c13ed-116">Not supported.</span></span> |
| <span data-ttu-id="c13ed-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c13ed-117">Application</span></span>                            | <span data-ttu-id="c13ed-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="c13ed-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="c13ed-119">**注意**：仅迁移 *支持应用程序*[权限](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)。</span><span class="sxs-lookup"><span data-stu-id="c13ed-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="c13ed-120">将来，Microsoft 可能要求你或你的客户根据导入的数据量支付其他费用。</span><span class="sxs-lookup"><span data-stu-id="c13ed-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->

## <a name="http-request"></a><span data-ttu-id="c13ed-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c13ed-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/channels/{channel-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="c13ed-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c13ed-122">Request headers</span></span>

| <span data-ttu-id="c13ed-123">名称</span><span class="sxs-lookup"><span data-stu-id="c13ed-123">Name</span></span>          | <span data-ttu-id="c13ed-124">说明</span><span class="sxs-lookup"><span data-stu-id="c13ed-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c13ed-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c13ed-125">Authorization</span></span> | <span data-ttu-id="c13ed-126">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="c13ed-126">Bearer {code}.</span></span> <span data-ttu-id="c13ed-127">必需。</span><span class="sxs-lookup"><span data-stu-id="c13ed-127">Required.</span></span> |
| <span data-ttu-id="c13ed-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="c13ed-128">Content-type</span></span> | <span data-ttu-id="c13ed-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c13ed-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c13ed-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c13ed-131">Request body</span></span>

<span data-ttu-id="c13ed-132">在请求正文中，提供 [chatMessage](../resources/chatmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c13ed-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="c13ed-133">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="c13ed-133">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="c13ed-134">响应</span><span class="sxs-lookup"><span data-stu-id="c13ed-134">Response</span></span>

<span data-ttu-id="c13ed-135">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [chatMessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c13ed-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c13ed-136">示例</span><span class="sxs-lookup"><span data-stu-id="c13ed-136">Examples</span></span>

### <a name="example-1-create-a-message-in-a-specified-channel"></a><span data-ttu-id="c13ed-137">示例 1：在指定的频道创建消息</span><span class="sxs-lookup"><span data-stu-id="c13ed-137">Example 1: Create a message in a specified channel</span></span>

<span data-ttu-id="c13ed-138">有关示例的更全面的列表，请参阅在频道或[聊天中创建 chatMessage。](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="c13ed-138">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="c13ed-139">请求</span><span class="sxs-lookup"><span data-stu-id="c13ed-139">Request</span></span>
<span data-ttu-id="c13ed-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c13ed-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c13ed-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c13ed-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel_1"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```

# <a name="c"></a>[<span data-ttu-id="c13ed-142">C#</span><span class="sxs-lookup"><span data-stu-id="c13ed-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c13ed-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c13ed-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c13ed-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c13ed-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c13ed-145">Java</span><span class="sxs-lookup"><span data-stu-id="c13ed-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c13ed-146">响应</span><span class="sxs-lookup"><span data-stu-id="c13ed-146">Response</span></span>

<span data-ttu-id="c13ed-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c13ed-147">The following is an example of the response.</span></span>

> <span data-ttu-id="c13ed-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c13ed-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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

### <a name="example-2-import-messages"></a><span data-ttu-id="c13ed-150">示例 2：导入邮件</span><span class="sxs-lookup"><span data-stu-id="c13ed-150">Example 2: Import messages</span></span>

> <span data-ttu-id="c13ed-151">**注意**：此方案 `Teamwork.Migrate.All` 需要权限范围。</span><span class="sxs-lookup"><span data-stu-id="c13ed-151">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="c13ed-152">请求</span><span class="sxs-lookup"><span data-stu-id="c13ed-152">Request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c13ed-153">以下示例显示如何使用 请求正文中的 和 键导入 `createDateTime` `from` 实时邮件。</span><span class="sxs-lookup"><span data-stu-id="c13ed-153">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages

{
   "messageType":"message",
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "deleted":false,
   "from":{
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
}
```

### <a name="response"></a><span data-ttu-id="c13ed-154">响应</span><span class="sxs-lookup"><span data-stu-id="c13ed-154">Response</span></span>

<span data-ttu-id="c13ed-155">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c13ed-155">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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

### <a name="example-3-import-messages-with-inline-images"></a><span data-ttu-id="c13ed-156">示例 3：导入包含内嵌图像的邮件</span><span class="sxs-lookup"><span data-stu-id="c13ed-156">Example 3: Import messages with inline images</span></span>

> [!NOTE]
> <span data-ttu-id="c13ed-157">目前，内联图像是导入邮件 API 架构支持的唯一媒体类型。</span><span class="sxs-lookup"><span data-stu-id="c13ed-157">Currently, inline images are the only media type supported by the import message API schema.</span></span>

> <span data-ttu-id="c13ed-158">**注意**：此方案 `Teamwork.Migrate.All` 需要权限范围。</span><span class="sxs-lookup"><span data-stu-id="c13ed-158">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="c13ed-159">请求</span><span class="sxs-lookup"><span data-stu-id="c13ed-159">Request</span></span>
<!-- { "blockType": "ignored" } -->
<span data-ttu-id="c13ed-160">以下示例演示如何使用 请求正文中的 和 键导入包含内嵌图像的 `createDateTime` `from` 返回时间邮件。</span><span class="sxs-lookup"><span data-stu-id="c13ed-160">The following example shows how to import back-in-time messages containing inline images using the `createDateTime` and `from` keys in the request body.</span></span>

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages

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

#### <a name="response"></a><span data-ttu-id="c13ed-161">响应</span><span class="sxs-lookup"><span data-stu-id="c13ed-161">Response</span></span>

<span data-ttu-id="c13ed-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c13ed-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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

## <a name="see-also"></a><span data-ttu-id="c13ed-163">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c13ed-163">See also</span></span>

* [<span data-ttu-id="c13ed-164">使用 Microsoft Graph 将第三方平台消息导入 Teams</span><span class="sxs-lookup"><span data-stu-id="c13ed-164">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="c13ed-165">创建频道</span><span class="sxs-lookup"><span data-stu-id="c13ed-165">Create channel</span></span>](channel-post.md)

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
