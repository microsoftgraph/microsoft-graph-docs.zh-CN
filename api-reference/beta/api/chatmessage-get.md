---
title: 在频道或聊天中获取 chatMessage
description: 在频道或聊天中检索单一消息（不包括其回复）。
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 82bd85c18d936136d24ce82ee1343d553fa6ae77
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971107"
---
# <a name="get-chatmessage-in-a-channel-or-chat"></a><span data-ttu-id="79b46-103">在频道或聊天中获取 chatMessage</span><span class="sxs-lookup"><span data-stu-id="79b46-103">Get chatMessage in a channel or chat</span></span>

<span data-ttu-id="79b46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79b46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79b46-105">在[频道](../resources/channel.md)或[聊天](../resources/chat.md)中检索单一[消息](../resources/chatmessage.md)或[消息回复](../resources/chatmessage.md)。</span><span class="sxs-lookup"><span data-stu-id="79b46-105">Retrieve a single [message](../resources/chatmessage.md) or a [message reply](../resources/chatmessage.md) in a [channel](../resources/channel.md) or a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="79b46-106">权限</span><span class="sxs-lookup"><span data-stu-id="79b46-106">Permissions</span></span>

<span data-ttu-id="79b46-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79b46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-channel"></a><span data-ttu-id="79b46-109">频道权限</span><span class="sxs-lookup"><span data-stu-id="79b46-109">Permissions for channel</span></span>

| <span data-ttu-id="79b46-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="79b46-110">Permission type</span></span>                        | <span data-ttu-id="79b46-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79b46-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="79b46-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79b46-112">Delegated (work or school account)</span></span>| <span data-ttu-id="79b46-113">ChannelMessage.Read.All、Group.Read.All、Group.Read.WriteAll</span><span class="sxs-lookup"><span data-stu-id="79b46-113">ChannelMessage.Read.All, Group.Read.All, Group.Read.WriteAll</span></span> |
|<span data-ttu-id="79b46-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79b46-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79b46-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="79b46-115">Not supported.</span></span>|
|<span data-ttu-id="79b46-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="79b46-116">Application</span></span>| <span data-ttu-id="79b46-117">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b46-117">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

### <a name="permissions-for-chat"></a><span data-ttu-id="79b46-118">聊天权限</span><span class="sxs-lookup"><span data-stu-id="79b46-118">Permissions for chat</span></span>

| <span data-ttu-id="79b46-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="79b46-119">Permission type</span></span>                        | <span data-ttu-id="79b46-120">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79b46-120">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="79b46-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79b46-121">Delegated (work or school account)</span></span>| <span data-ttu-id="79b46-122">Chat.Read、Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="79b46-122">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="79b46-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79b46-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79b46-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="79b46-124">Not supported.</span></span>|
|<span data-ttu-id="79b46-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="79b46-125">Application</span></span>| <span data-ttu-id="79b46-126">ChatMessage.Read.Chat\*、Chat.Read.All、Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b46-126">ChatMessage.Read.Chat\*, Chat.Read.All, Chat.ReadWrite.All</span></span>|

> <span data-ttu-id="79b46-127">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="79b46-127">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="79b46-128">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="79b46-128">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="79b46-129">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="79b46-129">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="79b46-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79b46-130">HTTP request</span></span>

<span data-ttu-id="79b46-131">**获取频道中的消息**</span><span class="sxs-lookup"><span data-stu-id="79b46-131">**Get message in a channel**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}
GET /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies/{reply-id}
```

<span data-ttu-id="79b46-132">**获取聊天中的消息**</span><span class="sxs-lookup"><span data-stu-id="79b46-132">**Get message in a chat**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/messages/{message-id}
GET /users/{user-id | user-principal-name}/chats/{chat-id}/messages/{message-id}
GET /me/chats/{chat-id}/messages/{message-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="79b46-133">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="79b46-133">Optional query parameters</span></span>
<span data-ttu-id="79b46-134">此运营商不支持通过 [OData 查询参数](/graph/query-parameters) 来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="79b46-134">This method does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="79b46-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="79b46-135">Request headers</span></span>
| <span data-ttu-id="79b46-136">标头</span><span class="sxs-lookup"><span data-stu-id="79b46-136">Header</span></span>       | <span data-ttu-id="79b46-137">值</span><span class="sxs-lookup"><span data-stu-id="79b46-137">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="79b46-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="79b46-138">Authorization</span></span>  | <span data-ttu-id="79b46-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79b46-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="79b46-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="79b46-141">Request body</span></span>
<span data-ttu-id="79b46-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="79b46-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79b46-143">响应</span><span class="sxs-lookup"><span data-stu-id="79b46-143">Response</span></span>

<span data-ttu-id="79b46-144">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="79b46-144">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79b46-145">示例</span><span class="sxs-lookup"><span data-stu-id="79b46-145">Examples</span></span>

### <a name="example-1-get-a-message-in-a-chat"></a><span data-ttu-id="79b46-146">示例 1：获取聊天中的消息。</span><span class="sxs-lookup"><span data-stu-id="79b46-146">Example 1: Get a message in a chat</span></span>
#### <a name="request"></a><span data-ttu-id="79b46-147">请求</span><span class="sxs-lookup"><span data-stu-id="79b46-147">Request</span></span>
<span data-ttu-id="79b46-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="79b46-148">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79b46-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="79b46-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagechannel_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces/messages/1612289992105
```
# <a name="c"></a>[<span data-ttu-id="79b46-150">C#</span><span class="sxs-lookup"><span data-stu-id="79b46-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagechannel-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79b46-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79b46-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagechannel-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79b46-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79b46-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagechannel-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79b46-153">Java</span><span class="sxs-lookup"><span data-stu-id="79b46-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagechannel-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79b46-154">响应</span><span class="sxs-lookup"><span data-stu-id="79b46-154">Response</span></span>
<span data-ttu-id="79b46-155">以下示例显示了相应的响应。`chatId`</span><span class="sxs-lookup"><span data-stu-id="79b46-155">The following example shows the response.`chatId`</span></span> <span data-ttu-id="79b46-156">标识包含此消息的[聊天](../resources/chat.md)。</span><span class="sxs-lookup"><span data-stu-id="79b46-156">identifies the [chat](../resources/chat.md) that contains this message.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3A8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5%40unq.gbl.spaces')/messages/$entity",
    "id": "1612289992105",
    "replyToId": null,
    "etag": "1612289992105",
    "messageType": "message",
    "createdDateTime": "2021-02-02T18:19:52.105Z",
    "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
    "importance": "normal",
    "locale": "en-us",
    "webUrl": null,
    "channelIdentity": null,
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
        "content": "test"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-get-a-message-in-a-channel"></a><span data-ttu-id="79b46-157">示例 2：获取频道中的消息。</span><span class="sxs-lookup"><span data-stu-id="79b46-157">Example 2: Get a message in a channel</span></span>
#### <a name="request"></a><span data-ttu-id="79b46-158">请求</span><span class="sxs-lookup"><span data-stu-id="79b46-158">Request</span></span>
<span data-ttu-id="79b46-159">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="79b46-159">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79b46-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="79b46-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagechannel_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349
```
# <a name="c"></a>[<span data-ttu-id="79b46-161">C#</span><span class="sxs-lookup"><span data-stu-id="79b46-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagechannel-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79b46-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79b46-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagechannel-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79b46-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79b46-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagechannel-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79b46-164">Java</span><span class="sxs-lookup"><span data-stu-id="79b46-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagechannel-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79b46-165">响应</span><span class="sxs-lookup"><span data-stu-id="79b46-165">Response</span></span>
<span data-ttu-id="79b46-166">以下示例显示了相应的响应。`channelIdentity`</span><span class="sxs-lookup"><span data-stu-id="79b46-166">The following example shows the response.`channelIdentity`</span></span> <span data-ttu-id="79b46-167">标识包含此消息的[团队](../resources/team.md)和[频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="79b46-167">identifies the [team](../resources/team.md) and [channel](../resources/channel.md) that contains this message.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages/$entity",
    "id": "1614618259349",
    "replyToId": null,
    "etag": "1614618259349",
    "messageType": "message",
    "createdDateTime": "2021-03-01T17:04:19.349Z",
    "lastModifiedDateTime": "2021-03-01T17:04:19.349Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1614618259349?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1614618259349&parentMessageId=1614618259349",
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
        "contentType": "html",
        "content": "<div><div><div><span><img height=\"250\" src=\"https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1614618259349/hostedContents/aWQ9eF8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNSx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kOS1jZTI3NDkxOTIzMTJjYWI5NDczMWQwYTgzNTFjN2VhNS92aWV3cy9pbWdv/$value\" width=\"424.6575342465753\" style=\"vertical-align:bottom; width:424px; height:250px\"></span></div></div></div>"
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

### <a name="example-3-get-reply-to-a-message-in-a-channel"></a><span data-ttu-id="79b46-168">示例 3：获取对频道中的消息回复</span><span class="sxs-lookup"><span data-stu-id="79b46-168">Example 3: Get reply to a message in a channel</span></span>
#### <a name="request"></a><span data-ttu-id="79b46-169">请求</span><span class="sxs-lookup"><span data-stu-id="79b46-169">Request</span></span>
<span data-ttu-id="79b46-170">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="79b46-170">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="79b46-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="79b46-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_chatmessagechannel_3"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1612509044972/replies/1613671348387
```
# <a name="c"></a>[<span data-ttu-id="79b46-172">C#</span><span class="sxs-lookup"><span data-stu-id="79b46-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-chatmessagechannel-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="79b46-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="79b46-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-chatmessagechannel-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="79b46-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="79b46-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-chatmessagechannel-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="79b46-175">Java</span><span class="sxs-lookup"><span data-stu-id="79b46-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-chatmessagechannel-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="79b46-176">响应</span><span class="sxs-lookup"><span data-stu-id="79b46-176">Response</span></span>
<span data-ttu-id="79b46-177">以下示例显示了相应的响应。`replyToId`</span><span class="sxs-lookup"><span data-stu-id="79b46-177">The following example shows the response.`replyToId`</span></span> <span data-ttu-id="79b46-178">包含根消息的 `id`。</span><span class="sxs-lookup"><span data-stu-id="79b46-178">contains the `id` of the root message.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages('1612509044972')/replies/$entity",
    "id": "1613671348387",
    "replyToId": "1612509044972",
    "etag": "1613671348387",
    "messageType": "message",
    "createdDateTime": "2021-02-18T18:02:28.387Z",
    "lastModifiedDateTime": "2021-02-18T18:02:28.387Z",
    "lastEditedDateTime": null,
    "deletedDateTime": null,
    "subject": null,
    "summary": null,
    "chatId": null,
    "importance": "normal",
    "locale": "en-us",
    "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1613671348387?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1613671348387&parentMessageId=1612509044972",
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
        "contentType": "html",
        "content": "<div><div>Test</div></div>"
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

## <a name="see-also"></a><span data-ttu-id="79b46-179">另请参阅</span><span class="sxs-lookup"><span data-stu-id="79b46-179">See also</span></span>

- [<span data-ttu-id="79b46-180">列出频道中的消息</span><span class="sxs-lookup"><span data-stu-id="79b46-180">List messages in a channel</span></span>](channel-list-messages.md)
- [<span data-ttu-id="79b46-181">列出聊天中的消息</span><span class="sxs-lookup"><span data-stu-id="79b46-181">List messages in a chat</span></span>](chat-list-messages.md)
- [<span data-ttu-id="79b46-182">在频道或聊天中发送消息</span><span class="sxs-lookup"><span data-stu-id="79b46-182">Send message in a channel or a chat</span></span>](chatmessage-post.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Retrieve a single message (without its replies) in a channel or a chat.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
