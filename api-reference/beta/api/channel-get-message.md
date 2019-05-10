---
title: 获取通道消息
description: 检索团队通道中的单个消息（不包括其回复）。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 0a8d8d6ce3956e8af5f17cd42418d84b325e3577
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635494"
---
# <a name="get-channel-message"></a><span data-ttu-id="ec6d6-103">获取通道消息</span><span class="sxs-lookup"><span data-stu-id="ec6d6-103">Get channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec6d6-104">检索团队[通道](../resources/channel.md)中的单个[消息](../resources/chatmessage.md)（不包括其回复）。</span><span class="sxs-lookup"><span data-stu-id="ec6d6-104">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec6d6-105">权限</span><span class="sxs-lookup"><span data-stu-id="ec6d6-105">Permissions</span></span>
<span data-ttu-id="ec6d6-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec6d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec6d6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec6d6-108">Permission Type</span></span>|<span data-ttu-id="ec6d6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec6d6-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="ec6d6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec6d6-110">Delegated (work or school account)</span></span>|<span data-ttu-id="ec6d6-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec6d6-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="ec6d6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec6d6-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec6d6-113">不支持</span><span class="sxs-lookup"><span data-stu-id="ec6d6-113">Not supported</span></span>|
|<span data-ttu-id="ec6d6-114">Application</span><span class="sxs-lookup"><span data-stu-id="ec6d6-114">Application</span></span>| <span data-ttu-id="ec6d6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec6d6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec6d6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec6d6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec6d6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ec6d6-117">Optional query parameters</span></span>
<span data-ttu-id="ec6d6-118">目前不支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="ec6d6-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec6d6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec6d6-119">Request headers</span></span>
| <span data-ttu-id="ec6d6-120">标头</span><span class="sxs-lookup"><span data-stu-id="ec6d6-120">Header</span></span>       | <span data-ttu-id="ec6d6-121">值</span><span class="sxs-lookup"><span data-stu-id="ec6d6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ec6d6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec6d6-122">Authorization</span></span>  | <span data-ttu-id="ec6d6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec6d6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec6d6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec6d6-125">Request body</span></span>
<span data-ttu-id="ec6d6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec6d6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec6d6-127">响应</span><span class="sxs-lookup"><span data-stu-id="ec6d6-127">Response</span></span>

<span data-ttu-id="ec6d6-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec6d6-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec6d6-129">示例</span><span class="sxs-lookup"><span data-stu-id="ec6d6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec6d6-130">请求</span><span class="sxs-lookup"><span data-stu-id="ec6d6-130">Request</span></span>
<span data-ttu-id="ec6d6-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec6d6-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184
```
##### <a name="response"></a><span data-ttu-id="ec6d6-132">响应</span><span class="sxs-lookup"><span data-stu-id="ec6d6-132">Response</span></span>
<span data-ttu-id="ec6d6-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ec6d6-133">Here is an example of the response.</span></span> 

><span data-ttu-id="ec6d6-134">**注意：** 为了提高可读性，缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ec6d6-134">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="ec6d6-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ec6d6-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages/$entity",
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
    "attachments": [
        {
            "id": "5e32f195-168a-474f-a273-123123123",
            "contentType": "reference",
            "contentUrl": "https://test.sharepoint.com/sites/TestSite/Shared%20Documents/General/Test.txt",
            "content": null,
            "name": "Test.txt",
            "thumbnailUrl": null
        }
    ],
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
    "reactions": [
      {
        "reactionType": "like",
        "user": {
            "id": "5d8d505c-864f-4804-88c7-4583c966cde8",
            "displayName": "Megan Bowen",
            "userIdentityType": "aadUser"
        },
        "createdDateTime": "2019-04-16T00:58:53.184Z"
      }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ec6d6-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="ec6d6-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ec6d6-137">C#</span><span class="sxs-lookup"><span data-stu-id="ec6d6-137">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_channel_message-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec6d6-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="ec6d6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_channel_message-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-get-message.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/channel-get-message.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
