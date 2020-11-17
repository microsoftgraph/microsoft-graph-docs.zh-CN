---
title: 列出频道消息
description: '检索团队渠道中的消息列表（无回复）。要获取消息的回复，请调用列表消息回复或获取消息回复 API。 '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 94cc4967d12f9ea2ae6190d4d1691d40283c43df
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000516"
---
# <a name="list-channel-messages"></a><span data-ttu-id="65289-104">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="65289-104">List channel messages</span></span>

<span data-ttu-id="65289-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65289-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65289-106">检索[团队](../resources/team.md)[频道](../resources/channel.md)中的[消息](../resources/chatmessage.md)列表（无回复）。</span><span class="sxs-lookup"><span data-stu-id="65289-106">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> 

<span data-ttu-id="65289-107">若要获取消息的回复，请调用[列出消息回复](channel-list-messagereplies.md)或[获取消息回复](channel-get-messagereply.md) API。</span><span class="sxs-lookup"><span data-stu-id="65289-107">To get the replies for a message, call the [list message replies](channel-list-messagereplies.md) or the [get message reply](channel-get-messagereply.md) API.</span></span> 

> <span data-ttu-id="65289-108">**注意**：此 API 支持使用[更改通知](../resources/webhooks.md)订阅更改（创建、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="65289-108">**Note**: This API supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="65289-109">这使呼叫方可以实时订阅和获取更改。</span><span class="sxs-lookup"><span data-stu-id="65289-109">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="65289-110">有关详细信息，请参阅[获取消息通知](/graph/teams-changenotifications-chatmessage)。</span><span class="sxs-lookup"><span data-stu-id="65289-110">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatmessage).</span></span>

## <a name="permissions"></a><span data-ttu-id="65289-111">权限</span><span class="sxs-lookup"><span data-stu-id="65289-111">Permissions</span></span>

<span data-ttu-id="65289-p103">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65289-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65289-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="65289-114">Permission Type</span></span>|<span data-ttu-id="65289-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65289-115">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="65289-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65289-116">Delegated (work or school account)</span></span>| <span data-ttu-id="65289-117">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65289-117">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="65289-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65289-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65289-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="65289-119">Not supported.</span></span>|
|<span data-ttu-id="65289-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="65289-120">Application</span></span>| <span data-ttu-id="65289-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65289-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="65289-122">**注意**：标有 \* 的权限使用 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="65289-122">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="65289-p104">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。有关详细信息，请参阅 [Microsoft Teams 中受保护的 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="65289-p104">Before calling this API with application permissions, you must request access. For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="65289-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65289-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="65289-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="65289-126">Optional query parameters</span></span>

<span data-ttu-id="65289-p105">可以使用 [$ top](/graph/query-parameters#top-parameter) 查询参数来控制每个响应的项目​​数。当前不支持其他 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="65289-p105">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response. The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

> <span data-ttu-id="65289-129">**注意：**[GET /teams/{id}/channels/{id}/messages/delta](chatmessage-delta.md) 支持按日期进行筛选，此时得到的数据与使用 GET /teams/{id}/channels/{id}/messages 时类似。</span><span class="sxs-lookup"><span data-stu-id="65289-129">**Note:** [GET /teams/{id}/channels/{id}/messages/delta](chatmessage-delta.md) supports filtering by date, which provides similar data to GET /teams/{id}/channels/{id}/messages.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65289-130">请求标头</span><span class="sxs-lookup"><span data-stu-id="65289-130">Request headers</span></span>

| <span data-ttu-id="65289-131">标头</span><span class="sxs-lookup"><span data-stu-id="65289-131">Header</span></span>       | <span data-ttu-id="65289-132">值</span><span class="sxs-lookup"><span data-stu-id="65289-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="65289-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="65289-133">Authorization</span></span>  | <span data-ttu-id="65289-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65289-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="65289-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="65289-136">Request body</span></span>

<span data-ttu-id="65289-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="65289-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65289-138">响应</span><span class="sxs-lookup"><span data-stu-id="65289-138">Response</span></span>

<span data-ttu-id="65289-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="65289-139">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65289-140">示例</span><span class="sxs-lookup"><span data-stu-id="65289-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="65289-141">请求</span><span class="sxs-lookup"><span data-stu-id="65289-141">Request</span></span>

<span data-ttu-id="65289-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65289-142">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65289-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="65289-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype"],
  "name": "get_channel_messages"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages
```
# <a name="c"></a>[<span data-ttu-id="65289-144">C#</span><span class="sxs-lookup"><span data-stu-id="65289-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-messages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65289-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65289-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-messages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65289-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65289-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-messages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="65289-147">Java</span><span class="sxs-lookup"><span data-stu-id="65289-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-messages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="65289-148">响应</span><span class="sxs-lookup"><span data-stu-id="65289-148">Response</span></span>
<span data-ttu-id="65289-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="65289-149">Here is an example of the response.</span></span> 

><span data-ttu-id="65289-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="65289-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
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
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
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
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
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
  ]
}
-->

