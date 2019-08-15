---
title: 列出频道邮件答复
description: 在团队的频道中列出邮件的所有答复。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 087420938b08362057fc07f86c94e024ad18fd4e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36418759"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="c1462-103">列出频道邮件答复</span><span class="sxs-lookup"><span data-stu-id="c1462-103">List channel message replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1462-104">在团队的[频道](../resources/channel.md)中列出[邮件](../resources/chatmessage.md)的所有答复。</span><span class="sxs-lookup"><span data-stu-id="c1462-104">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

<span data-ttu-id="c1462-105">此方法仅列出指定邮件的答复 (如果有)。</span><span class="sxs-lookup"><span data-stu-id="c1462-105">This method lists only the replies of the specified message, if any.</span></span> <span data-ttu-id="c1462-106">若要获取邮件本身, 只需调用[get 信道消息](channel-get-message.md)即可。</span><span class="sxs-lookup"><span data-stu-id="c1462-106">To get the message itself, simply call [get channel message](channel-get-message.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c1462-107">权限</span><span class="sxs-lookup"><span data-stu-id="c1462-107">Permissions</span></span>
<span data-ttu-id="c1462-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1462-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1462-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1462-110">Permission Type</span></span>|<span data-ttu-id="c1462-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1462-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c1462-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1462-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c1462-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1462-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="c1462-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1462-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1462-115">不支持</span><span class="sxs-lookup"><span data-stu-id="c1462-115">Not supported</span></span>|
|<span data-ttu-id="c1462-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1462-116">Application</span></span>| <span data-ttu-id="c1462-117">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1462-117">Group.Read.All,Group.ReadWrite.All</span></span>|

> [!NOTE]
> <span data-ttu-id="c1462-118">在使用应用程序权限调用此 API 之前, 您必须请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="c1462-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="c1462-119">有关详细信息, 请参阅[Microsoft 团队中的受保护 api](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="c1462-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="c1462-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1462-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c1462-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1462-121">Optional query parameters</span></span>

<span data-ttu-id="c1462-122">可以使用 [$top](/graph/query-parameters#top-parameter) 查询参数控制每个响应中的项目数。</span><span class="sxs-lookup"><span data-stu-id="c1462-122">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="c1462-123">目前不支持其他 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c1462-123">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1462-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1462-124">Request headers</span></span>
| <span data-ttu-id="c1462-125">标头</span><span class="sxs-lookup"><span data-stu-id="c1462-125">Header</span></span>       | <span data-ttu-id="c1462-126">值</span><span class="sxs-lookup"><span data-stu-id="c1462-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c1462-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1462-127">Authorization</span></span>  | <span data-ttu-id="c1462-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1462-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c1462-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1462-130">Request body</span></span>
<span data-ttu-id="c1462-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1462-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1462-132">响应</span><span class="sxs-lookup"><span data-stu-id="c1462-132">Response</span></span>
<span data-ttu-id="c1462-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/channel.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c1462-133">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1462-134">示例</span><span class="sxs-lookup"><span data-stu-id="c1462-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1462-135">请求</span><span class="sxs-lookup"><span data-stu-id="c1462-135">Request</span></span>
<span data-ttu-id="c1462-136">在此示例中, 指定的邮件有两个答复。</span><span class="sxs-lookup"><span data-stu-id="c1462-136">In this example, the specified message has two replies.</span></span> <span data-ttu-id="c1462-137">每个答复都有一个或多个[chatMessageMention](../resources/chatmessagemention.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c1462-137">Each reply has one or more [chatMessageMention](../resources/chatmessagemention.md) objects.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1462-138">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c1462-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message_replies"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1462-139">C#</span><span class="sxs-lookup"><span data-stu-id="c1462-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1462-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1462-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1462-141">目标-C</span><span class="sxs-lookup"><span data-stu-id="c1462-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c1462-142">响应</span><span class="sxs-lookup"><span data-stu-id="c1462-142">Response</span></span>
<span data-ttu-id="c1462-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c1462-143">Here is an example of the response.</span></span> 

><span data-ttu-id="c1462-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c1462-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages('1555375673184')/replies",
    "@odata.count": 2,
    "value": [
        {
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
        },
        {
            "id": "1555375848360",
            "replyToId": "1555375673184",
            "etag": "1555375848360",
            "messageType": "message",
            "createdDateTime": "2019-04-16T00:50:48.36Z",
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
                "content": "<div><div>And, <at id=\"0\">Alex Wilber</at>, can we see the February report as well?</div>\n</div>"
            },
            "attachments": [],
            "mentions": [
                {
                    "id": 0,
                    "mentionText": "Alex Wilber",
                    "mentioned": {
                        "application": null,
                        "device": null,
                        "conversation": null,
                        "user": {
                            "id": "be178404-260a-4f80-b7e5-d52c1e6fdc71",
                            "displayName": "Alex Wilber",
                            "userIdentityType": "aadUser"
                        }
                    }
                }
            ],
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
  "description": "List channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
