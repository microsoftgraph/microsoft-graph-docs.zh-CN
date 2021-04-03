---
title: 列出频道消息回复
description: 列出团队频道中邮件的所有回复。
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: aaa40106f3b1364bc1b5ad13ac0a8ecfbc894513
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582889"
---
# <a name="list-replies"></a><span data-ttu-id="90733-103">列出答复</span><span class="sxs-lookup"><span data-stu-id="90733-103">List replies</span></span>

<span data-ttu-id="90733-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90733-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90733-105">列出团队[频道中消息](../resources/chatmessage.md)[的所有](../resources/channel.md)回复。</span><span class="sxs-lookup"><span data-stu-id="90733-105">List all the replies to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

<span data-ttu-id="90733-106">此方法仅列出指定邮件的答复（如果有）。</span><span class="sxs-lookup"><span data-stu-id="90733-106">This method lists only the replies of the specified message, if any.</span></span> <span data-ttu-id="90733-107">若要获取消息本身，只需调用 [获取频道消息](chatmessage-get.md)。</span><span class="sxs-lookup"><span data-stu-id="90733-107">To get the message itself, simply call [get channel message](chatmessage-get.md).</span></span>

> <span data-ttu-id="90733-108">**注意**：此 API 支持使用 [更改通知](../resources/webhooks.md)订阅更改（创建、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="90733-108">**Note**: This API supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="90733-109">这使呼叫方可以实时订阅和获取更改。</span><span class="sxs-lookup"><span data-stu-id="90733-109">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="90733-110">有关详细信息，请参阅[获取消息通知](/graph/teams-changenotifications-chatmessage)。</span><span class="sxs-lookup"><span data-stu-id="90733-110">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatmessage).</span></span>

## <a name="permissions"></a><span data-ttu-id="90733-111">权限</span><span class="sxs-lookup"><span data-stu-id="90733-111">Permissions</span></span>
<span data-ttu-id="90733-p103">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90733-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90733-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="90733-114">Permission Type</span></span>|<span data-ttu-id="90733-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90733-115">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="90733-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90733-116">Delegated (work or school account)</span></span>| <span data-ttu-id="90733-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="90733-117">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="90733-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90733-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90733-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="90733-119">Not supported.</span></span>|
|<span data-ttu-id="90733-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="90733-120">Application</span></span>| <span data-ttu-id="90733-121">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="90733-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="90733-122">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="90733-122">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="90733-123">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="90733-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="90733-124">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="90733-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="90733-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90733-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90733-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="90733-126">Optional query parameters</span></span>

<span data-ttu-id="90733-127">可以使用 [$top](/graph/query-parameters#top-parameter) 查询参数控制每个响应中的项目数。</span><span class="sxs-lookup"><span data-stu-id="90733-127">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="90733-128">允许的最大 `$top` 值为 50。</span><span class="sxs-lookup"><span data-stu-id="90733-128">Maximum allowed `$top` value is 50.</span></span>
<span data-ttu-id="90733-129">目前不支持其他 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="90733-129">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90733-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="90733-130">Request headers</span></span>
| <span data-ttu-id="90733-131">标头</span><span class="sxs-lookup"><span data-stu-id="90733-131">Header</span></span>       | <span data-ttu-id="90733-132">值</span><span class="sxs-lookup"><span data-stu-id="90733-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="90733-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="90733-133">Authorization</span></span>  | <span data-ttu-id="90733-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90733-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="90733-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="90733-136">Request body</span></span>
<span data-ttu-id="90733-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90733-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90733-138">响应</span><span class="sxs-lookup"><span data-stu-id="90733-138">Response</span></span>
<span data-ttu-id="90733-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="90733-139">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90733-140">示例</span><span class="sxs-lookup"><span data-stu-id="90733-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="90733-141">请求</span><span class="sxs-lookup"><span data-stu-id="90733-141">Request</span></span>
<span data-ttu-id="90733-142">本示例中，指定的邮件有三个回复。</span><span class="sxs-lookup"><span data-stu-id="90733-142">In this example, the specified message has three replies.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_listmessagereplies_1"
}-->
```http
GET https://graph.microsoft.com/v1.0/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616989510408/replies
```

### <a name="response"></a><span data-ttu-id="90733-143">响应</span><span class="sxs-lookup"><span data-stu-id="90733-143">Response</span></span>
<span data-ttu-id="90733-144">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="90733-144">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1616989510408')/replies",
    "@odata.count": 3,
    "value": [
        {
            "id": "1616989753153",
            "replyToId": "1616989510408",
            "etag": "1616989753153",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:49:13.153Z",
            "lastModifiedDateTime": "2021-03-29T03:49:13.153Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989753153?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989753153&parentMessageId=1616989510408",
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
                "content": "Reply3"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1616989750004",
            "replyToId": "1616989510408",
            "etag": "1616989750004",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:49:10.004Z",
            "lastModifiedDateTime": "2021-03-29T03:49:10.004Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989750004?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989750004&parentMessageId=1616989510408",
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
                "content": "Reply2"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "id": "1616989747416",
            "replyToId": "1616989510408",
            "etag": "1616989747416",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:49:07.416Z",
            "lastModifiedDateTime": "2021-03-29T03:49:07.416Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616989747416?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616989747416&parentMessageId=1616989510408",
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
                "content": "Reply1"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->