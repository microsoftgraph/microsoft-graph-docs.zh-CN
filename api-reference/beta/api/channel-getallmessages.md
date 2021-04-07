---
title: 频道：getAllMessages
description: 检索团队中跨频道的所有消息。
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9d8f4ed1db42b7d5f35d12f8f612bc544ef6e4c2
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610975"
---
# <a name="channel-getallmessages"></a><span data-ttu-id="20115-103">频道：getAllMessages</span><span class="sxs-lookup"><span data-stu-id="20115-103">channel: getAllMessages</span></span>

<span data-ttu-id="20115-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20115-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20115-105">检索[团队](../resources/team.md)中所有[频道](../resources/channel.md)之间的[消息](../resources/chatmessage.md)，包括文本、音频和视频对话。</span><span class="sxs-lookup"><span data-stu-id="20115-105">Retrieve [messages](../resources/chatmessage.md) across all [channels](../resources/channel.md) in a [team](../resources/team.md) including text, audio, and video conversations.</span></span>

## <a name="permissions"></a><span data-ttu-id="20115-106">权限</span><span class="sxs-lookup"><span data-stu-id="20115-106">Permissions</span></span>

<span data-ttu-id="20115-107">调用此 API 需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="20115-107">The following permissions are required to call this API.</span></span> <span data-ttu-id="20115-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20115-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20115-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="20115-109">Permission type</span></span>      | <span data-ttu-id="20115-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20115-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20115-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20115-111">Delegated (work or school account)</span></span> | <span data-ttu-id="20115-112">不支持</span><span class="sxs-lookup"><span data-stu-id="20115-112">Not supported</span></span> |
|<span data-ttu-id="20115-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20115-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20115-114">不支持</span><span class="sxs-lookup"><span data-stu-id="20115-114">Not supported</span></span> |
|<span data-ttu-id="20115-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="20115-115">Application</span></span> | <span data-ttu-id="20115-116">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="20115-116">ChannelMessage.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="20115-117">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="20115-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="20115-118">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="20115-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="20115-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20115-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/getAllMessages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="20115-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="20115-120">Optional query parameters</span></span>

<span data-ttu-id="20115-121">可以使用 [$top](/graph/query-parameters#top-parameter) 查询参数控制每个响应中的项目数。</span><span class="sxs-lookup"><span data-stu-id="20115-121">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span>
<span data-ttu-id="20115-122">目前不支持其他 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="20115-122">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-body"></a><span data-ttu-id="20115-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="20115-123">Request body</span></span>

<span data-ttu-id="20115-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="20115-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="20115-125">响应</span><span class="sxs-lookup"><span data-stu-id="20115-125">Response</span></span>

<span data-ttu-id="20115-126">若成功，此方法将返回 `200 OK`响应代码，同时也会返回通道中的所有消息。</span><span class="sxs-lookup"><span data-stu-id="20115-126">If successful, this method returns a `200 OK` response code and also returns all the messages in the channel.</span></span>

## <a name="example"></a><span data-ttu-id="20115-127">示例</span><span class="sxs-lookup"><span data-stu-id="20115-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="20115-128">请求</span><span class="sxs-lookup"><span data-stu-id="20115-128">Request</span></span>

<span data-ttu-id="20115-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="20115-129">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="20115-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="20115-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allchannelmessages_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages
```
# <a name="c"></a>[<span data-ttu-id="20115-131">C#</span><span class="sxs-lookup"><span data-stu-id="20115-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allchannelmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="20115-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="20115-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allchannelmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="20115-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="20115-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allchannelmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="20115-134">Java</span><span class="sxs-lookup"><span data-stu-id="20115-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-allchannelmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="20115-135">响应</span><span class="sxs-lookup"><span data-stu-id="20115-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true,
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(chatMessage)",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages?$skip=2",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1616990417393",
            "replyToId": null,
            "etag": "1616990417393",
            "messageType": "message",
            "createdDateTime": "2021-03-29T04:00:17.393Z",
            "lastModifiedDateTime": "2021-03-29T04:00:17.393Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3Ad5d2708d408c41d98424c1c354c19db3%40thread.tacv2/1616990417393?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990417393&parentMessageId=1616990417393",
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
                "content": "Test message"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:d5d2708d408c41d98424c1c354c19db3@thread.tacv2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1616990171266",
            "replyToId": "1616990032035",
            "etag": "1616990171266",
            "messageType": "message",
            "createdDateTime": "2021-03-29T03:56:11.266Z",
            "lastModifiedDateTime": "2021-03-29T03:56:11.266Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616990171266?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616990171266&parentMessageId=1616990032035",
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
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "channels: getallmessages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
