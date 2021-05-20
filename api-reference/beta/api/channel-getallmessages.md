---
title: 频道：getAllMessages
description: 检索团队中跨频道的所有消息。
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3174401b2d25bf2c7c00f0cffca2c048af7deca6
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546117"
---
# <a name="channel-getallmessages"></a><span data-ttu-id="962a1-103">频道：getAllMessages</span><span class="sxs-lookup"><span data-stu-id="962a1-103">channel: getAllMessages</span></span>

<span data-ttu-id="962a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="962a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="962a1-105">检索[团队](../resources/team.md)中所有[频道](../resources/channel.md)之间的[消息](../resources/chatmessage.md)，包括文本、音频和视频对话。</span><span class="sxs-lookup"><span data-stu-id="962a1-105">Retrieve [messages](../resources/chatmessage.md) across all [channels](../resources/channel.md) in a [team](../resources/team.md), including text, audio, and video conversations.</span></span> 

<span data-ttu-id="962a1-106">若要了解有关使用 Microsoft Teams 导出 API 来导出内容，请参阅[使用 Microsoft Teams 导出 API 导出内容](/microsoftteams/export-teams-content)。</span><span class="sxs-lookup"><span data-stu-id="962a1-106">To learn more about using the Microsoft Teams export APIs to export content, see [Export content with the Microsoft Teams export APIs](/microsoftteams/export-teams-content).</span></span>

## <a name="permissions"></a><span data-ttu-id="962a1-107">权限</span><span class="sxs-lookup"><span data-stu-id="962a1-107">Permissions</span></span>

<span data-ttu-id="962a1-p101">要调用此 API，需要以下权限。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="962a1-p101">The following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="962a1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="962a1-110">Permission type</span></span>      | <span data-ttu-id="962a1-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="962a1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="962a1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="962a1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="962a1-113">不支持</span><span class="sxs-lookup"><span data-stu-id="962a1-113">Not supported</span></span> |
|<span data-ttu-id="962a1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="962a1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="962a1-115">不支持</span><span class="sxs-lookup"><span data-stu-id="962a1-115">Not supported</span></span> |
|<span data-ttu-id="962a1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="962a1-116">Application</span></span> | <span data-ttu-id="962a1-117">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="962a1-117">ChannelMessage.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="962a1-118">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="962a1-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="962a1-119">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="962a1-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="962a1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="962a1-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/getAllMessages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="962a1-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="962a1-121">Optional query parameters</span></span>

<span data-ttu-id="962a1-122">可以使用 [$top](/graph/query-parameters#top-parameter) 查询参数控制每个响应中的项目数。</span><span class="sxs-lookup"><span data-stu-id="962a1-122">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span>
<span data-ttu-id="962a1-123">此外，**lastModifiedDateTime** 上的 **dateTime** 范围查询还支持 [$filter](/graph/query-parameters#filter-parameter)。</span><span class="sxs-lookup"><span data-stu-id="962a1-123">Additionally, [$filter](/graph/query-parameters#filter-parameter) is supported with **dateTime** range query on **lastModifiedDateTime**.</span></span> <span data-ttu-id="962a1-124">目前不支持其他 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="962a1-124">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-body"></a><span data-ttu-id="962a1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="962a1-125">Request body</span></span>

<span data-ttu-id="962a1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="962a1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="962a1-127">响应</span><span class="sxs-lookup"><span data-stu-id="962a1-127">Response</span></span>

<span data-ttu-id="962a1-128">若成功，此方法将返回 `200 OK`响应代码，同时也会返回通道中的所有消息。</span><span class="sxs-lookup"><span data-stu-id="962a1-128">If successful, this method returns a `200 OK` response code and also returns all the messages in the channel.</span></span>

## <a name="example"></a><span data-ttu-id="962a1-129">示例</span><span class="sxs-lookup"><span data-stu-id="962a1-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="962a1-130">请求</span><span class="sxs-lookup"><span data-stu-id="962a1-130">Request</span></span>

<span data-ttu-id="962a1-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="962a1-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="962a1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="962a1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_allchannelmessages_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/getAllMessages
```
# <a name="c"></a>[<span data-ttu-id="962a1-133">C#</span><span class="sxs-lookup"><span data-stu-id="962a1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-allchannelmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="962a1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="962a1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-allchannelmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="962a1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="962a1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-allchannelmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="962a1-136">Java</span><span class="sxs-lookup"><span data-stu-id="962a1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-allchannelmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="962a1-137">响应</span><span class="sxs-lookup"><span data-stu-id="962a1-137">Response</span></span>

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
