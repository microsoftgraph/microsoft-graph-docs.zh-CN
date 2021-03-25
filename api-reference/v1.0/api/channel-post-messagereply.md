---
title: 在频道中回复消息
description: 在渠道中回复现有消息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e56d43e84dc7ba2cc47fd30ac47e9cb2fdcc8ea
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202252"
---
# <a name="reply-to-a-message-in-a-channel"></a><span data-ttu-id="8ee1c-103">在频道中回复消息</span><span class="sxs-lookup"><span data-stu-id="8ee1c-103">Reply to a message in a channel</span></span>

<span data-ttu-id="8ee1c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ee1c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8ee1c-105">在指定的频道中创建新的 [chatMessage](../resources/chatmessage.md) [回复](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-105">Create a new reply to a [chatMessage](../resources/chatmessage.md) in a specified [channel](../resources/channel.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="8ee1c-106">权限</span><span class="sxs-lookup"><span data-stu-id="8ee1c-106">Permissions</span></span>

<span data-ttu-id="8ee1c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8ee1c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ee1c-109">Permission type</span></span>                        | <span data-ttu-id="8ee1c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8ee1c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8ee1c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ee1c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8ee1c-112">ChannelMessage.Send、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ee1c-112">ChannelMessage.Send, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="8ee1c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ee1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ee1c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-114">Not supported.</span></span> |
| <span data-ttu-id="8ee1c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ee1c-115">Application</span></span>                            | <span data-ttu-id="8ee1c-116">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="8ee1c-116">Teamwork.Migrate.All</span></span> |

> <span data-ttu-id="8ee1c-117">**注意**：仅迁移 *支持应用程序*[权限](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-117">**Note**: Application permissions are *only* supported for [migration](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<span data-ttu-id="8ee1c-118">将来，Microsoft 可能要求你或你的客户根据导入的数据量支付其他费用。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-118">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported.</span></span>

## <a name="http-request"></a><span data-ttu-id="8ee1c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ee1c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies
```

## <a name="request-headers"></a><span data-ttu-id="8ee1c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ee1c-120">Request headers</span></span>

| <span data-ttu-id="8ee1c-121">名称</span><span class="sxs-lookup"><span data-stu-id="8ee1c-121">Name</span></span>       | <span data-ttu-id="8ee1c-122">类型</span><span class="sxs-lookup"><span data-stu-id="8ee1c-122">Type</span></span> | <span data-ttu-id="8ee1c-123">说明</span><span class="sxs-lookup"><span data-stu-id="8ee1c-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="8ee1c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ee1c-124">Authorization</span></span>  | <span data-ttu-id="8ee1c-125">string</span><span class="sxs-lookup"><span data-stu-id="8ee1c-125">string</span></span>  | <span data-ttu-id="8ee1c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ee1c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ee1c-128">Request body</span></span>

<span data-ttu-id="8ee1c-129">在请求正文中，提供 message 对象的 JSON [表示](../resources/chatmessage.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-129">In the request body, supply a JSON representation of a [message](../resources/chatmessage.md) object.</span></span> <span data-ttu-id="8ee1c-130">只有 body 属性是必需的，其他属性是可选的。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-130">Only the body property is mandatory, other properties are optional.</span></span>

## <a name="response"></a><span data-ttu-id="8ee1c-131">响应</span><span class="sxs-lookup"><span data-stu-id="8ee1c-131">Response</span></span>

<span data-ttu-id="8ee1c-132">如果成功，此方法返回 `201 Created` 包含已创建 [消息的响应](../resources/chatmessage.md) 代码。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-132">If successful, this method returns `201 Created` response code with the [message](../resources/chatmessage.md) that was created.</span></span>

## <a name="examples"></a><span data-ttu-id="8ee1c-133">示例</span><span class="sxs-lookup"><span data-stu-id="8ee1c-133">Examples</span></span>

### <a name="example-1-create-a-new-reply-to-a-chatmessage"></a><span data-ttu-id="8ee1c-134">示例 1：创建对 chatMessage 的新回复</span><span class="sxs-lookup"><span data-stu-id="8ee1c-134">Example 1: Create a new reply to a chatMessage</span></span>

#### <a name="request"></a><span data-ttu-id="8ee1c-135">请求</span><span class="sxs-lookup"><span data-stu-id="8ee1c-135">Request</span></span>
<span data-ttu-id="8ee1c-136">请求示例如下所示。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-136">The following is an example of a request.</span></span>

<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

#### <a name="response"></a><span data-ttu-id="8ee1c-137">响应</span><span class="sxs-lookup"><span data-stu-id="8ee1c-137">Response</span></span>

<span data-ttu-id="8ee1c-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-138">The following is an example of the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages('1590776551682')/replies/$entity",
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

### <a name="example-2-import-messages"></a><span data-ttu-id="8ee1c-139">示例 2：导入邮件</span><span class="sxs-lookup"><span data-stu-id="8ee1c-139">Example 2: Import messages</span></span>

> <span data-ttu-id="8ee1c-140">**注意**：此方案 `Teamwork.Migrate.All` 需要权限范围。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-140">**Note**: The permission scope `Teamwork.Migrate.All` is required for this scenario.</span></span>

#### <a name="request"></a><span data-ttu-id="8ee1c-141">请求</span><span class="sxs-lookup"><span data-stu-id="8ee1c-141">Request</span></span>

<span data-ttu-id="8ee1c-142">以下示例显示如何使用 请求正文中的 和 键导入 `createDateTime` `from` 实时邮件。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-142">The following example show how to import back-in-time messages using the `createDateTime` and `from` keys in the request body.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies

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

#### <a name="response"></a><span data-ttu-id="8ee1c-143">响应</span><span class="sxs-lookup"><span data-stu-id="8ee1c-143">Response</span></span>

<span data-ttu-id="8ee1c-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8ee1c-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages('1590776551682')/replies/$entity",
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
