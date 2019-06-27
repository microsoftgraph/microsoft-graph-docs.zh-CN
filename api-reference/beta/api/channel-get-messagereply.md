---
title: 获取对频道消息的答复
description: 获取团队频道中对邮件的单个答复。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4d0ec855b2b91ce9ee912725140e7222c32ff630
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262109"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="4f704-103">获取对频道消息的答复</span><span class="sxs-lookup"><span data-stu-id="4f704-103">Get a reply to a channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f704-104">获取团队[频道](../resources/channel.md)中对[邮件](../resources/chatmessage.md)的单个答复。</span><span class="sxs-lookup"><span data-stu-id="4f704-104">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f704-105">权限</span><span class="sxs-lookup"><span data-stu-id="4f704-105">Permissions</span></span>

<span data-ttu-id="4f704-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f704-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f704-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f704-108">Permission Type</span></span>|<span data-ttu-id="4f704-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f704-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="4f704-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f704-110">Delegated (work or school account)</span></span>|<span data-ttu-id="4f704-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f704-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="4f704-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f704-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f704-113">不支持</span><span class="sxs-lookup"><span data-stu-id="4f704-113">Not supported</span></span>|
|<span data-ttu-id="4f704-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f704-114">Application</span></span>| <span data-ttu-id="4f704-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f704-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f704-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f704-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f704-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4f704-117">Optional query parameters</span></span>

<span data-ttu-id="4f704-118">目前不支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="4f704-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f704-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f704-119">Request headers</span></span>

| <span data-ttu-id="4f704-120">标头</span><span class="sxs-lookup"><span data-stu-id="4f704-120">Header</span></span>       | <span data-ttu-id="4f704-121">值</span><span class="sxs-lookup"><span data-stu-id="4f704-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4f704-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f704-122">Authorization</span></span>  | <span data-ttu-id="4f704-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f704-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4f704-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f704-125">Request body</span></span>

<span data-ttu-id="4f704-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4f704-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f704-127">响应</span><span class="sxs-lookup"><span data-stu-id="4f704-127">Response</span></span>

<span data-ttu-id="4f704-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f704-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f704-129">示例</span><span class="sxs-lookup"><span data-stu-id="4f704-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4f704-130">请求</span><span class="sxs-lookup"><span data-stu-id="4f704-130">Request</span></span>

<span data-ttu-id="4f704-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f704-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184", "1555377090002"],
  "name": "get_channel_message_reply"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies/1555377090002
```
##### <a name="response"></a><span data-ttu-id="4f704-132">响应</span><span class="sxs-lookup"><span data-stu-id="4f704-132">Response</span></span>
<span data-ttu-id="4f704-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4f704-133">Here is an example of the response.</span></span> 

><span data-ttu-id="4f704-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4f704-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages('1555375673184')/replies/$entity",
    "id": "1555377090002",
    "replyToId": "1555375673184",
    "etag": "1555377090002",
    "messageType": "message",
    "createdDateTime": "2019-04-16T01:11:30.002Z",
    "lastModifiedDateTime": null,
    "deletedDateTime": null,
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
            "id": "bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f",
            "displayName": "Adele Vance",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
    },
    "attachments": [],
    "mentions": [
        {
            "id": 0,
            "mentionText": "Megan",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
                    "displayName": "Megan",
                    "userIdentityType": "aadUser"
                }
            }
        },
        {
            "id": 1,
            "mentionText": "Alex",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "user": {
                    "id": "be178404-260a-4f80-b7e5-d52c1e6fdc71",
                    "displayName": "Alex",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
    "reactions": []
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4f704-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="4f704-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4f704-137">C#</span><span class="sxs-lookup"><span data-stu-id="4f704-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel_message_reply-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4f704-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="4f704-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel_message_reply-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4f704-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="4f704-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_channel_message_reply-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a reply to a channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get-messagereply.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/channel-get-messagereply.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-get-messagereply.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
