---
title: 获取对频道消息的答复
description: 获取团队频道中对邮件的单个答复。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e8ffbc9d1135c1345d9fdeece42664d3eb16044d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35438501"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="2888e-103">获取对频道消息的答复</span><span class="sxs-lookup"><span data-stu-id="2888e-103">Get a reply to a channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2888e-104">获取团队[频道](../resources/channel.md)中对[邮件](../resources/chatmessage.md)的单个答复。</span><span class="sxs-lookup"><span data-stu-id="2888e-104">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="2888e-105">权限</span><span class="sxs-lookup"><span data-stu-id="2888e-105">Permissions</span></span>

<span data-ttu-id="2888e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2888e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2888e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2888e-108">Permission Type</span></span>|<span data-ttu-id="2888e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2888e-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="2888e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2888e-110">Delegated (work or school account)</span></span>|<span data-ttu-id="2888e-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2888e-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="2888e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2888e-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2888e-113">不支持</span><span class="sxs-lookup"><span data-stu-id="2888e-113">Not supported</span></span>|
|<span data-ttu-id="2888e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2888e-114">Application</span></span>| <span data-ttu-id="2888e-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2888e-115">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2888e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2888e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2888e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2888e-117">Optional query parameters</span></span>

<span data-ttu-id="2888e-118">目前不支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="2888e-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2888e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2888e-119">Request headers</span></span>

| <span data-ttu-id="2888e-120">标头</span><span class="sxs-lookup"><span data-stu-id="2888e-120">Header</span></span>       | <span data-ttu-id="2888e-121">值</span><span class="sxs-lookup"><span data-stu-id="2888e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2888e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2888e-122">Authorization</span></span>  | <span data-ttu-id="2888e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2888e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2888e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2888e-125">Request body</span></span>

<span data-ttu-id="2888e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2888e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2888e-127">响应</span><span class="sxs-lookup"><span data-stu-id="2888e-127">Response</span></span>

<span data-ttu-id="2888e-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2888e-128">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2888e-129">示例</span><span class="sxs-lookup"><span data-stu-id="2888e-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2888e-130">请求</span><span class="sxs-lookup"><span data-stu-id="2888e-130">Request</span></span>

<span data-ttu-id="2888e-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2888e-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2888e-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2888e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184", "1555377090002"],
  "name": "get_channel_message_reply"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies/1555377090002
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2888e-133">C#</span><span class="sxs-lookup"><span data-stu-id="2888e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2888e-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="2888e-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2888e-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="2888e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2888e-136">响应</span><span class="sxs-lookup"><span data-stu-id="2888e-136">Response</span></span>
<span data-ttu-id="2888e-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2888e-137">Here is an example of the response.</span></span> 

><span data-ttu-id="2888e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2888e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
