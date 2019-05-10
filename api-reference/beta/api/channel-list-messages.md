---
title: 列出频道消息
description: '检索团队频道中的消息列表（无回复）。 若要获取消息的回复，请调用“列出消息回复”或“获取消息回复”API。 '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: f482222d1eb6c672d97109a9cc7d6f6d9c838a5e
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635594"
---
# <a name="list-channel-messages"></a><span data-ttu-id="81bf5-104">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="81bf5-104">List channel messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81bf5-105">检索[团队](../resources/team.md)[频道](../resources/channel.md)中的[消息](../resources/chatmessage.md)列表（无回复）。</span><span class="sxs-lookup"><span data-stu-id="81bf5-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> 

<span data-ttu-id="81bf5-106">若要获取消息的回复，请调用[列出消息回复](channel-get-messagereply.md)或[获取消息回复](channel-list-messagereplies.md) API。</span><span class="sxs-lookup"><span data-stu-id="81bf5-106">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span> 

## <a name="permissions"></a><span data-ttu-id="81bf5-107">权限</span><span class="sxs-lookup"><span data-stu-id="81bf5-107">Permissions</span></span>

<span data-ttu-id="81bf5-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81bf5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81bf5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="81bf5-110">Permission Type</span></span>|<span data-ttu-id="81bf5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81bf5-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="81bf5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81bf5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81bf5-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81bf5-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="81bf5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81bf5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81bf5-115">不支持</span><span class="sxs-lookup"><span data-stu-id="81bf5-115">Not supported</span></span>|
|<span data-ttu-id="81bf5-116">Application</span><span class="sxs-lookup"><span data-stu-id="81bf5-116">Application</span></span>| <span data-ttu-id="81bf5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="81bf5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81bf5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81bf5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81bf5-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="81bf5-119">Optional query parameters</span></span>

<span data-ttu-id="81bf5-120">可以使用 [$top](/graph/query-parameters#top-parameter) 查询参数控制每个响应中的项目数。</span><span class="sxs-lookup"><span data-stu-id="81bf5-120">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="81bf5-121">目前不支持其他 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="81bf5-121">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81bf5-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="81bf5-122">Request headers</span></span>

| <span data-ttu-id="81bf5-123">标头</span><span class="sxs-lookup"><span data-stu-id="81bf5-123">Header</span></span>       | <span data-ttu-id="81bf5-124">值</span><span class="sxs-lookup"><span data-stu-id="81bf5-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="81bf5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="81bf5-125">Authorization</span></span>  | <span data-ttu-id="81bf5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81bf5-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="81bf5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="81bf5-128">Request body</span></span>

<span data-ttu-id="81bf5-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="81bf5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81bf5-130">响应</span><span class="sxs-lookup"><span data-stu-id="81bf5-130">Response</span></span>

<span data-ttu-id="81bf5-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="81bf5-131">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81bf5-132">示例</span><span class="sxs-lookup"><span data-stu-id="81bf5-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="81bf5-133">请求</span><span class="sxs-lookup"><span data-stu-id="81bf5-133">Request</span></span>

<span data-ttu-id="81bf5-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="81bf5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype"],
  "name": "get_channel_messages"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages
```
##### <a name="response"></a><span data-ttu-id="81bf5-135">响应</span><span class="sxs-lookup"><span data-stu-id="81bf5-135">Response</span></span>
<span data-ttu-id="81bf5-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="81bf5-136">Here is an example of the response.</span></span> 

><span data-ttu-id="81bf5-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="81bf5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages",
    "@odata.count": 3,
    "value": [
        {
            "id": "1555375673184",
            "replyToId": null,
            "etag": "1555375673184",
            "messageType": "message",
            "createdDateTime": "2019-04-16T00:47:53.184Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f",
                    "displayName": "Adele Vance",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div><div>Nice to join this team. <at id=\"0\">Megan Bowen</at>, have we got the March report ready please?</div>\n</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Megan Bowen",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
                            "displayName": "Megan Bowen",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": []
        },
        {
            "id": "1548100551644",
            "replyToId": null,
            "etag": "1548100551893",
            "messageType": "message",
            "createdDateTime": "2019-01-21T19:55:51.644Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "importance": "normal",
            "locale": "en-us",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "c651e5be-7631-42ad-99c6-12c59def11fb",
                    "displayName": "Miriam Graham",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div>I've added an Excel tab to the channel containing the P&amp;L Summary. \r\n<div style=\"display:inline\"><at id=\"0\">Isaiah Langer</at></div> and team, please review the Sale Summary tab in particular, and make any necessary updates.</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Isaiah Langer",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "b525e831-bd00-45e5-860c-a4329ef5f5d8",
                            "displayName": "Isaiah Langer",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": [
                {
                    "reactionType": "like",
                    "createdDateTime": "2019-01-21T19:55:51.893Z",
                    "user": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "e1ecb745-c10f-40af-a9d4-cab946c80ac7",
                            "displayName": null,
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ]
        },
        {
            "id": "1548100547534",
            "replyToId": null,
            "etag": "1548100547534",
            "messageType": "message",
            "createdDateTime": "2019-01-21T19:55:47.534Z",
            "lastModifiedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "importance": "high",
            "locale": "en-us",
            "policyViolation": null,
            "from": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f",
                    "displayName": "Adele Vance",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "html",
                "content": "<div>Just a reminder to everyone to please update your monthly reports by this Friday!</div>"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="81bf5-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="81bf5-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="81bf5-140">C#</span><span class="sxs-lookup"><span data-stu-id="81bf5-140">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel_messages-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="81bf5-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="81bf5-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel_messages-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-list-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
