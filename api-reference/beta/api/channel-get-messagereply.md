---
title: 获取对频道消息的答复
description: 获取团队频道中对邮件的单个答复。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c6dff7204068f6c9ebb3397cc8e745229e399efa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42440344"
---
# <a name="get-a-reply-to-a-channel-message"></a><span data-ttu-id="a0506-103">获取对频道消息的答复</span><span class="sxs-lookup"><span data-stu-id="a0506-103">Get a reply to a channel message</span></span>

<span data-ttu-id="a0506-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a0506-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0506-105">获取团队[频道](../resources/channel.md)中对[邮件](../resources/chatmessage.md)的单个答复。</span><span class="sxs-lookup"><span data-stu-id="a0506-105">Get a single reply to a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0506-106">权限</span><span class="sxs-lookup"><span data-stu-id="a0506-106">Permissions</span></span>

<span data-ttu-id="a0506-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0506-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0506-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0506-109">Permission Type</span></span>|<span data-ttu-id="a0506-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0506-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="a0506-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0506-111">Delegated (work or school account)</span></span>| <span data-ttu-id="a0506-112">ChannelMessage、Group、group、Group。 All</span><span class="sxs-lookup"><span data-stu-id="a0506-112">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="a0506-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0506-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0506-114">不支持</span><span class="sxs-lookup"><span data-stu-id="a0506-114">Not supported</span></span>|
|<span data-ttu-id="a0506-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0506-115">Application</span></span>| <span data-ttu-id="a0506-116">ChannelMessage、Group、group、Group。 All</span><span class="sxs-lookup"><span data-stu-id="a0506-116">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="a0506-117">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="a0506-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="a0506-118">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="a0506-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="a0506-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0506-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a0506-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a0506-120">Optional query parameters</span></span>

<span data-ttu-id="a0506-121">目前不支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="a0506-121">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a0506-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0506-122">Request headers</span></span>

| <span data-ttu-id="a0506-123">标头</span><span class="sxs-lookup"><span data-stu-id="a0506-123">Header</span></span>       | <span data-ttu-id="a0506-124">值</span><span class="sxs-lookup"><span data-stu-id="a0506-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0506-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0506-125">Authorization</span></span>  | <span data-ttu-id="a0506-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0506-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0506-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0506-128">Request body</span></span>

<span data-ttu-id="a0506-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a0506-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0506-130">响应</span><span class="sxs-lookup"><span data-stu-id="a0506-130">Response</span></span>

<span data-ttu-id="a0506-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0506-131">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0506-132">示例</span><span class="sxs-lookup"><span data-stu-id="a0506-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a0506-133">请求</span><span class="sxs-lookup"><span data-stu-id="a0506-133">Request</span></span>

<span data-ttu-id="a0506-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0506-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a0506-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0506-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184", "1555377090002"],
  "name": "get_channel_message_reply"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies/1555377090002
```
# <a name="c"></a>[<span data-ttu-id="a0506-136">C#</span><span class="sxs-lookup"><span data-stu-id="a0506-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-reply-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a0506-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0506-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-reply-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a0506-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0506-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-reply-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a0506-139">响应</span><span class="sxs-lookup"><span data-stu-id="a0506-139">Response</span></span>
<span data-ttu-id="a0506-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a0506-140">Here is an example of the response.</span></span> 

><span data-ttu-id="a0506-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a0506-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
