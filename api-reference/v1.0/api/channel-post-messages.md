---
title: 在频道中发送 chatMessage
description: 在指定的频道中创建新的 chatMessage。
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 444729528c0ff97feed650f240e6d4e8e70dd921
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208456"
---
# <a name="send-chatmessage-in-channel"></a><span data-ttu-id="c0b5e-103">在频道中发送 chatMessage</span><span class="sxs-lookup"><span data-stu-id="c0b5e-103">Send chatMessage in channel</span></span>

<span data-ttu-id="c0b5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0b5e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c0b5e-105">在指定的频道[中发送新的 chatMessage](../resources/chatmessage.md) [。](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="c0b5e-105">Send a new [chatMessage](../resources/chatmessage.md) in the specified [channel](../resources/channel.md).</span></span>

> <span data-ttu-id="c0b5e-106">**注意**：使用安全工具 [作为](/legal/microsoft-apis/terms-of-use)Microsoft Teams违反日志文件。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-106">**Note**: It is a violation of the [terms of use](/legal/microsoft-apis/terms-of-use) to use Microsoft Teams as a log file.</span></span> <span data-ttu-id="c0b5e-107">仅发送用户将阅读的邮件。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-107">Only send messages that people will read.</span></span>

## <a name="permissions"></a><span data-ttu-id="c0b5e-108">权限</span><span class="sxs-lookup"><span data-stu-id="c0b5e-108">Permissions</span></span>

<span data-ttu-id="c0b5e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c0b5e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c0b5e-111">Permission type</span></span>                        | <span data-ttu-id="c0b5e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c0b5e-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c0b5e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c0b5e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c0b5e-114">ChannelMessage.Send</span><span class="sxs-lookup"><span data-stu-id="c0b5e-114">ChannelMessage.Send</span></span> |
| <span data-ttu-id="c0b5e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c0b5e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0b5e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-116">Not supported.</span></span> |
| <span data-ttu-id="c0b5e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c0b5e-117">Application</span></span>                            | <span data-ttu-id="c0b5e-118">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="c0b5e-118">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="c0b5e-119">**注意**：仅迁移 *支持应用程序*[权限](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-119">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="c0b5e-120">将来，Microsoft 可能要求你或你的客户根据导入的数据量支付其他费用。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->

## <a name="http-request"></a><span data-ttu-id="c0b5e-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c0b5e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/channels/{channel-id}/messages
```

## <a name="request-headers"></a><span data-ttu-id="c0b5e-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c0b5e-122">Request headers</span></span>

| <span data-ttu-id="c0b5e-123">名称</span><span class="sxs-lookup"><span data-stu-id="c0b5e-123">Name</span></span>          | <span data-ttu-id="c0b5e-124">说明</span><span class="sxs-lookup"><span data-stu-id="c0b5e-124">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c0b5e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0b5e-125">Authorization</span></span> | <span data-ttu-id="c0b5e-126">Bearer {code}。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-126">Bearer {code}.</span></span> <span data-ttu-id="c0b5e-127">必需。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-127">Required.</span></span> |
| <span data-ttu-id="c0b5e-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="c0b5e-128">Content-type</span></span> | <span data-ttu-id="c0b5e-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c0b5e-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c0b5e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c0b5e-131">Request body</span></span>

<span data-ttu-id="c0b5e-132">在请求正文中，提供 [chatMessage](../resources/chatmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-132">In the request body, supply a JSON representation of a [chatMessage](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="c0b5e-133">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-133">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="c0b5e-134">响应</span><span class="sxs-lookup"><span data-stu-id="c0b5e-134">Response</span></span>

<span data-ttu-id="c0b5e-135">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [chatMessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-135">If successful, this method returns a `201 Created` response code and a new [chatMessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c0b5e-136">示例</span><span class="sxs-lookup"><span data-stu-id="c0b5e-136">Examples</span></span>

### <a name="example-1-create-a-message-in-a-specified-channel"></a><span data-ttu-id="c0b5e-137">示例 1：在指定的频道创建消息</span><span class="sxs-lookup"><span data-stu-id="c0b5e-137">Example 1: Create a message in a specified channel</span></span>

<span data-ttu-id="c0b5e-138">有关示例的更全面的列表，请参阅在频道或[聊天中创建 chatMessage。](chatmessage-post.md)</span><span class="sxs-lookup"><span data-stu-id="c0b5e-138">For a more comprehensive list of examples, see [Create chatMessage in a channel or a chat](chatmessage-post.md).</span></span>

### <a name="request"></a><span data-ttu-id="c0b5e-139">请求</span><span class="sxs-lookup"><span data-stu-id="c0b5e-139">Request</span></span>
<span data-ttu-id="c0b5e-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-140">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="c0b5e-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0b5e-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_channelmessage_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="c0b5e-142">C#</span><span class="sxs-lookup"><span data-stu-id="c0b5e-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-channelmessage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0b5e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0b5e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-channelmessage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0b5e-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0b5e-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-channelmessage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0b5e-145">Java</span><span class="sxs-lookup"><span data-stu-id="c0b5e-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-channelmessage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0b5e-146">响应</span><span class="sxs-lookup"><span data-stu-id="c0b5e-146">Response</span></span>

<span data-ttu-id="c0b5e-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-147">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages/$entity",
    "id": "1616990032035",
    "replyToId": null,
    "etag": "1616990032035",
    "messageType": "message",
    "createdDateTime": "2021-03-29T03:53:52.035Z",
    "lastModifiedDateTime": "2021-03-29T03:53:52.035Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616990032035?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990032035&parentMessageId=1616990032035",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
            "displayName": "Robin Kline",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "text",
        "content": "Hello World"
    },
    "channelIdentity": {
        "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
        "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-import-messages"></a><span data-ttu-id="c0b5e-148">示例 2：导入邮件</span><span class="sxs-lookup"><span data-stu-id="c0b5e-148">Example 2: Import messages</span></span>

> <span data-ttu-id="c0b5e-149">**注意**：此方案 `Teamwork.Migrate.All` 需要权限范围。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-149">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="c0b5e-150">请求</span><span class="sxs-lookup"><span data-stu-id="c0b5e-150">Request</span></span>

<span data-ttu-id="c0b5e-151">以下示例显示如何使用 请求正文中的 和 键导入 `createDateTime` `from` 实时邮件。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-151">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>


# <a name="http"></a>[<span data-ttu-id="c0b5e-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0b5e-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_channelmessage_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
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
   }
}
```
# <a name="c"></a>[<span data-ttu-id="c0b5e-153">C#</span><span class="sxs-lookup"><span data-stu-id="c0b5e-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-channelmessage-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0b5e-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0b5e-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-channelmessage-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0b5e-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0b5e-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-channelmessage-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0b5e-156">Java</span><span class="sxs-lookup"><span data-stu-id="c0b5e-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-channelmessage-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c0b5e-157">响应</span><span class="sxs-lookup"><span data-stu-id="c0b5e-157">Response</span></span>

<span data-ttu-id="c0b5e-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-158">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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
         "displayName":"John Doe",
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

### <a name="example-3-import-messages-with-inline-images"></a><span data-ttu-id="c0b5e-159">示例 3：导入包含内嵌图像的邮件</span><span class="sxs-lookup"><span data-stu-id="c0b5e-159">Example 3: Import messages with inline images</span></span>

> [!NOTE]
> <span data-ttu-id="c0b5e-160">目前，内联图像是导入邮件 API 架构支持的唯一媒体类型。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-160">Currently, inline images are the only media type supported by the import message API schema.</span></span>

> <span data-ttu-id="c0b5e-161">**注意**：此方案 `Teamwork.Migrate.All` 需要权限范围。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-161">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="c0b5e-162">请求</span><span class="sxs-lookup"><span data-stu-id="c0b5e-162">Request</span></span>

<span data-ttu-id="c0b5e-163">以下示例演示如何使用 请求正文中的 和 键导入包含内嵌图像的 `createDateTime` `from` 返回时间邮件。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-163">The following example shows how to import back-in-time messages containing inline images using the `createDateTime` and `from` keys in the request body.</span></span>


# <a name="http"></a>[<span data-ttu-id="c0b5e-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="c0b5e-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_channelmessage_3"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"id-value",
         "displayName":"John Doe",
         "userIdentityType":"aadUser"
      }
   },
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
# <a name="c"></a>[<span data-ttu-id="c0b5e-165">C#</span><span class="sxs-lookup"><span data-stu-id="c0b5e-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-channelmessage-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c0b5e-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c0b5e-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-channelmessage-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c0b5e-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c0b5e-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-channelmessage-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c0b5e-168">Java</span><span class="sxs-lookup"><span data-stu-id="c0b5e-168">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-channelmessage-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c0b5e-169">响应</span><span class="sxs-lookup"><span data-stu-id="c0b5e-169">Response</span></span>

<span data-ttu-id="c0b5e-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c0b5e-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages/$entity",
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

## <a name="see-also"></a><span data-ttu-id="c0b5e-171">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c0b5e-171">See also</span></span>

* [<span data-ttu-id="c0b5e-172">使用 Microsoft Graph 将第三方平台消息导入 Teams</span><span class="sxs-lookup"><span data-stu-id="c0b5e-172">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="c0b5e-173">创建频道</span><span class="sxs-lookup"><span data-stu-id="c0b5e-173">Create channel</span></span>](channel-post.md)

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
