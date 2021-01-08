---
title: 频道： getAllMessages
description: 检索团队中跨渠道的所有消息。
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4ad45990655059db63d90c79225c676e4cf06ec0
ms.sourcegitcommit: a0a5690ad9c109149e0b8c8baba164648ff5c226
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2021
ms.locfileid: "49784766"
---
# <a name="channels-getallmessages"></a><span data-ttu-id="2c115-103">频道： getAllMessages</span><span class="sxs-lookup"><span data-stu-id="2c115-103">channels: getAllMessages</span></span>

<span data-ttu-id="2c115-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c115-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c115-105">检索[团队](../resources/team.md)中所有[渠道](../resources/channel.md)之间的所有[消息](../resources/chatmessage.md)，包括文本、音频和视频对话。</span><span class="sxs-lookup"><span data-stu-id="2c115-105">Retrieve all [messages](../resources/chatmessage.md) across all [channels](../resources/channel.md) in a [team](../resources/team.md) including text, audio, and video conversations.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c115-106">权限</span><span class="sxs-lookup"><span data-stu-id="2c115-106">Permissions</span></span>

<span data-ttu-id="2c115-107">调用此 API 需要以下权限。</span><span class="sxs-lookup"><span data-stu-id="2c115-107">The following permissions are required to call this API.</span></span> <span data-ttu-id="2c115-108">若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c115-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c115-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c115-109">Permission type</span></span>      | <span data-ttu-id="2c115-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c115-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c115-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c115-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2c115-112">不支持</span><span class="sxs-lookup"><span data-stu-id="2c115-112">Not supported</span></span> |
|<span data-ttu-id="2c115-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c115-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c115-114">不支持</span><span class="sxs-lookup"><span data-stu-id="2c115-114">Not supported</span></span> |
|<span data-ttu-id="2c115-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c115-115">Application</span></span> | <span data-ttu-id="2c115-116">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="2c115-116">ChannelMessage.Read.All</span></span> |

> [!NOTE]
> <span data-ttu-id="2c115-117">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="2c115-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="2c115-118">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="2c115-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="2c115-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c115-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/getAllMessages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2c115-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2c115-120">Optional query parameters</span></span>

<span data-ttu-id="2c115-121">此操作当前不支持使用 [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2c115-121">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="2c115-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c115-122">Request body</span></span>

<span data-ttu-id="2c115-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c115-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c115-124">响应</span><span class="sxs-lookup"><span data-stu-id="2c115-124">Response</span></span>

<span data-ttu-id="2c115-125">若成功，此方法将返回 `200 OK`响应代码，同时也会返回通道中的所有消息。</span><span class="sxs-lookup"><span data-stu-id="2c115-125">If successful, this method returns a `200 OK` response code and also returns all the messages in the channel.</span></span>

## <a name="example"></a><span data-ttu-id="2c115-126">示例</span><span class="sxs-lookup"><span data-stu-id="2c115-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="2c115-127">请求</span><span class="sxs-lookup"><span data-stu-id="2c115-127">Request</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/0e05a7e4-a48d-4615-b0b7-c7494da9ce68/channels/getAllMessages
```

### <a name="response"></a><span data-ttu-id="2c115-128">响应</span><span class="sxs-lookup"><span data-stu-id="2c115-128">Response</span></span>

><span data-ttu-id="2c115-129">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2c115-129">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metdata#Collection(chatMessage)",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/beta/teams/a5212c6a-a8b1-49cd-bd40-7f83f0a42861/channels/getAllMessages?$top=2&$skip=2",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/beta/teams/ab5332ba-6dd9-46d3-ade5-5c61a2f148b2/channels/19%3A72409da00b014de5ba2d2bef4a44db09%40thread.tacv2/messages/1580173996201",
            "id": "1580173996201",
            "replyToId": null,
            "etag": "1580173996201",
            "messageType": "message",
            "createdDateTime": "2020-01-28T01:13:16.201Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A72409da00b014de5ba2d2bef4a44db09%40thread.tacv2/1580173996201?groupId=ab5332ba-6dd9-46d3-ade5-5c61a2f148b2&tenantId=e0d829d2-c239-4b28-9d08-c096da71be7a&createdTime=1580173996201&parentMessageId=1580173996201",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "a5212c6a-a8b1-49cd-bd40-7f83f0a42861",
                    "displayName": "spoons test",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Test"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.id": "https://graph.microsoft.com/beta/teams/ab5332ba-6dd9-46d3-ade5-5c61a2f148b2/channels/19%3A72409da00b014de5ba2d2bef4a44db09%40thread.tacv2/messages/1580768557513",
            "id": "1580768557513",
            "replyToId": null,
            "etag": "1580768557513",
            "messageType": "message",
            "createdDateTime": "2020-02-03T22:22:37.513Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "a5212c6a-a8b1-49cd-bd40-7f83f0a42861",
                    "displayName": "spoons test",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "hi user1,user3"
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
