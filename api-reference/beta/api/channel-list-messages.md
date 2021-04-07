---
title: 列出频道消息
description: '检索团队频道中的消息列表（无回复）。 若要获取消息的回复，请调用“列出消息回复”或“获取消息回复”API。 '
localization_priority: Priority
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 74df4282a745fbabf11ccdee4fae7d64aeab5dbe
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610843"
---
# <a name="list-channel-messages"></a><span data-ttu-id="3d0f7-104">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="3d0f7-104">List channel messages</span></span>

<span data-ttu-id="3d0f7-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d0f7-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d0f7-106">检索[团队](../resources/team.md)[频道](../resources/channel.md)中的[消息](../resources/chatmessage.md)列表（无回复）。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-106">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> 

<span data-ttu-id="3d0f7-107">若要获取消息的回复，请调用[列出消息回复](chatmessage-list-replies.md)或[获取消息回复](chatmessage-get.md) API。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-107">To get the replies for a message, call the [list message replies](chatmessage-list-replies.md) or the [get message reply](chatmessage-get.md) API.</span></span> 

> <span data-ttu-id="3d0f7-108">**注意**：此 API 支持使用 [更改通知](../resources/webhooks.md)订阅更改（创建、更新和删除）。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-108">**Note**: This API supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="3d0f7-109">这使呼叫方可以实时订阅和获取更改。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-109">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="3d0f7-110">有关详细信息，请参阅[获取消息通知](/graph/teams-changenotifications-chatmessage)。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-110">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatmessage).</span></span>

## <a name="permissions"></a><span data-ttu-id="3d0f7-111">权限</span><span class="sxs-lookup"><span data-stu-id="3d0f7-111">Permissions</span></span>

<span data-ttu-id="3d0f7-p103">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d0f7-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d0f7-114">Permission Type</span></span>|<span data-ttu-id="3d0f7-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3d0f7-115">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="3d0f7-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d0f7-116">Delegated (work or school account)</span></span>| <span data-ttu-id="3d0f7-117">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d0f7-117">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="3d0f7-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d0f7-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d0f7-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-119">Not supported.</span></span>|
|<span data-ttu-id="3d0f7-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d0f7-120">Application</span></span>| <span data-ttu-id="3d0f7-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d0f7-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="3d0f7-122">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-122">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="3d0f7-123">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-123">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="3d0f7-124">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-124">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="3d0f7-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d0f7-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{team-id}/channels/{channel-id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d0f7-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3d0f7-126">Optional query parameters</span></span>

<span data-ttu-id="3d0f7-127">可以使用 [$top](/graph/query-parameters#top-parameter) 查询参数控制每个响应中的项目数。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-127">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="3d0f7-128">`$top` 的最大允许值为 50。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-128">Maximum allowed value for `$top` is 50.</span></span>
<span data-ttu-id="3d0f7-129">目前不支持其他 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-129">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

> <span data-ttu-id="3d0f7-130">**请注意：**[GET /teams/{team-id}/channels/{channel-id}/messages/delta](chatmessage-delta.md) 支持按日期进行筛选，此时得到的数据与使用 GET /teams/{team-id}/channels/{channel-id}/messages。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-130">**Note:** [GET /teams/{team-id}/channels/{channel-id}/messages/delta](chatmessage-delta.md) supports filtering by date, which provides similar data to    GET /teams/{team-id}/channels/{channel-id}/messages .</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d0f7-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d0f7-131">Request headers</span></span>

| <span data-ttu-id="3d0f7-132">标头</span><span class="sxs-lookup"><span data-stu-id="3d0f7-132">Header</span></span>       | <span data-ttu-id="3d0f7-133">值</span><span class="sxs-lookup"><span data-stu-id="3d0f7-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3d0f7-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d0f7-134">Authorization</span></span>  | <span data-ttu-id="3d0f7-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3d0f7-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d0f7-137">Request body</span></span>

<span data-ttu-id="3d0f7-138">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d0f7-139">响应</span><span class="sxs-lookup"><span data-stu-id="3d0f7-139">Response</span></span>

<span data-ttu-id="3d0f7-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatMessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-140">If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d0f7-141">示例</span><span class="sxs-lookup"><span data-stu-id="3d0f7-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d0f7-142">请求</span><span class="sxs-lookup"><span data-stu-id="3d0f7-142">Request</span></span>

<span data-ttu-id="3d0f7-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-143">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3d0f7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d0f7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_listchannelmessages_1"
}-->
```
GET https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages
```
# <a name="c"></a>[<span data-ttu-id="3d0f7-145">C#</span><span class="sxs-lookup"><span data-stu-id="3d0f7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-listchannelmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d0f7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d0f7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-listchannelmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d0f7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d0f7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-listchannelmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d0f7-148">Java</span><span class="sxs-lookup"><span data-stu-id="3d0f7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-listchannelmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3d0f7-149">响应</span><span class="sxs-lookup"><span data-stu-id="3d0f7-149">Response</span></span>
<span data-ttu-id="3d0f7-150">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-150">The following is an example of the request.</span></span> <span data-ttu-id="3d0f7-151">响应中的 `nextLink` 可用于获取下一页消息。</span><span class="sxs-lookup"><span data-stu-id="3d0f7-151">`nextLink` in the response can be used to get the next page of messages.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2')/messages",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages?$skiptoken=%5b%7B%22token%22%3a%22%2bRID%3a~vpsQAJ9uAC047gwAAACcBQ%3d%3d%23RT%3a1%23TRC%3a20%23RTD%3aAyAER1ygxSHVHGAn2S99BTI6OzViOjZnOGU5ZWM1ZDVmOGdiZjk2OGNkZmNmMTczNGY3QXVpc2ZiZS91YmR3MzwyNzIyNDY2OTU0NTg6AA%3d%3d%23ISV%3a2%23IEO%3a65551%23QCF%3a3%23FPC%3aAggEAAAAcBYAABUFAADQKgAABAAAAHAWAAACALu4GwAAAHAWAAACAPSTMwAAAHAWAACaAFWa84BXgQKAEIAMgBaAE4AUgAuAAoAIwAIgACAAAiAACAABACCAAAEVgBSAI4AYgA%2bAGQAEEAAQAAEABACAAAIEEBBAACAYgB%2bAH4AbgBqACoAHwAICCBAEEIAAAgEQAACAIoAZgB2ADoAMgAKAPoAZgB2AJoAXgBIAgiAAQUqLF4AJgALACARAgBCACoAfgB6AIwABgYCQAAFXAAAAcBYAAAYA%2f50ZgGeEXwAAAHAWAAAEAPaBS4V7AAAAcBYAAAIA1aSJAAAAcBYAAAIAtLmbAAAAcBYAAAIAqKXdAAAAcBYAAAQAppUugOMAAABwFgAABADQoAWA6wAAAHAWAAAEABGl94M5AAAA0CoAAAYA6pF7iYOBaQIAANAqAAAcAEUPAMAAMAACAQCBAHQAADDAgCAAQgByAQAzUJDRBAAA0CoAAAQAETwKAA4FAADQKgAAAgBekRUFAADQKgAAHAB2pQCABYAMgJeAH4ATgAGAvIIIgASABIAFgCWA%22%2c%22range%22%3a%7B%22min%22%3a%2205C1D79B33ADE4%22%2c%22max%22%3a%2205C1D7A52F89EC%22%7D%7D%5d",
    "value": [
        {
            "id": "1616965872395",
            "replyToId": null,
            "etag": "1616965872395",
            "messageType": "message",
            "createdDateTime": "2021-03-28T21:11:12.395Z",
            "lastModifiedDateTime": "2021-03-28T21:11:12.395Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616965872395?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616965872395&parentMessageId=1616965872395",
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
                "content": "Hello World <at id=\"0\">Jane Smith</at>"
            },
            "channelIdentity": {
                "teamId": "fbe2bf47-16c8-47cf-b4a5-4b9b187c508b",
                "channelId": "19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Jane Smith",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "ef1c916a-3135-4417-ba27-8eb7bd084193",
                            "displayName": "Jane Smith",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
            "reactions": []
        },
        {
            "id": "1616963377068",
            "replyToId": null,
            "etag": "1616963377068",
            "messageType": "message",
            "createdDateTime": "2021-03-28T20:29:37.068Z",
            "lastModifiedDateTime": "2021-03-28T20:29:37.068Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": "",
            "summary": null,
            "chatId": null,
            "importance": "normal",
            "locale": "en-us",
            "webUrl": "https://teams.microsoft.com/l/message/19%3A4a95f7d8db4c4e7fae857bcebe0623e6%40thread.tacv2/1616963377068?groupId=fbe2bf47-16c8-47cf-b4a5-4b9b187c508b&tenantId=2432b57b-0abd-43db-aa7b-16eadd115d34&createdTime=1616963377068&parentMessageId=1616963377068",
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
                "content": "<div><div><div><span><img height=\"145\" src=\"https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents/aWQ9eF8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kMS02YmI3Nzk3ZGU2MmRjODdjODA4YmQ1ZmI0OWM4NjI2ZC92aWV3cy9pbWdv/$value\" width=\"131\" style=\"vertical-align:bottom; width:131px; height:145px\"></span><div>&nbsp;</div></div><div><div><span><img height=\"65\" src=\"https://graph.microsoft.com/beta/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages/1616963377068/hostedContents/aWQ9eF8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNCx0eXBlPTEsdXJsPWh0dHBzOi8vdXMtYXBpLmFzbS5za3lwZS5jb20vdjEvb2JqZWN0cy8wLXd1cy1kNi0xMzY3OTE4MzVlODIxOGZlMmUwZWEwYTA1ODAxNjRiNC92aWV3cy9pbWdv/$value\" width=\"79\" style=\"vertical-align:bottom; width:79px; height:65px\"></span></div></div></div></div>"
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
  "description": "List channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

