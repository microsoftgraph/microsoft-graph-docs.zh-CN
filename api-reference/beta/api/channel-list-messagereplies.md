---
title: 列出频道邮件答复
description: 在团队的频道中列出邮件的所有答复。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3c3c681c820f4cc855105ec1605be920a98a1430
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456456"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="96689-103">列出频道邮件答复</span><span class="sxs-lookup"><span data-stu-id="96689-103">List channel message replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96689-104">在团队的[频道](../resources/channel.md)中列出[邮件](../resources/chatmessage.md)的所有答复。</span><span class="sxs-lookup"><span data-stu-id="96689-104">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

<span data-ttu-id="96689-105">此方法仅列出指定邮件的答复 (如果有)。</span><span class="sxs-lookup"><span data-stu-id="96689-105">This method lists only the replies of the specified message, if any.</span></span> <span data-ttu-id="96689-106">若要获取邮件本身, 只需调用[get 信道消息](channel-get-message.md)即可。</span><span class="sxs-lookup"><span data-stu-id="96689-106">To get the message itself, simply call [get channel message](channel-get-message.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="96689-107">权限</span><span class="sxs-lookup"><span data-stu-id="96689-107">Permissions</span></span>
<span data-ttu-id="96689-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96689-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96689-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="96689-110">Permission Type</span></span>|<span data-ttu-id="96689-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96689-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="96689-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96689-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96689-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96689-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="96689-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96689-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96689-115">不支持</span><span class="sxs-lookup"><span data-stu-id="96689-115">Not supported</span></span>|
|<span data-ttu-id="96689-116">Application</span><span class="sxs-lookup"><span data-stu-id="96689-116">Application</span></span>| <span data-ttu-id="96689-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="96689-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96689-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96689-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96689-119">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="96689-119">Optional query parameters</span></span>

<span data-ttu-id="96689-120">您可以使用[$top](/graph/query-parameters#top-parameter)查询参数来控制每个响应的项目数。</span><span class="sxs-lookup"><span data-stu-id="96689-120">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response.</span></span> <span data-ttu-id="96689-121">其他[OData 查询参数](/graph/query-parameters)目前不受支持。</span><span class="sxs-lookup"><span data-stu-id="96689-121">The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96689-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="96689-122">Request headers</span></span>
| <span data-ttu-id="96689-123">标头</span><span class="sxs-lookup"><span data-stu-id="96689-123">Header</span></span>       | <span data-ttu-id="96689-124">值</span><span class="sxs-lookup"><span data-stu-id="96689-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96689-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="96689-125">Authorization</span></span>  | <span data-ttu-id="96689-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96689-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="96689-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="96689-128">Request body</span></span>
<span data-ttu-id="96689-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96689-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96689-130">响应</span><span class="sxs-lookup"><span data-stu-id="96689-130">Response</span></span>
<span data-ttu-id="96689-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/channel.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="96689-131">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="96689-132">示例</span><span class="sxs-lookup"><span data-stu-id="96689-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96689-133">请求</span><span class="sxs-lookup"><span data-stu-id="96689-133">Request</span></span>
<span data-ttu-id="96689-134">在此示例中, 指定的邮件有两个答复。</span><span class="sxs-lookup"><span data-stu-id="96689-134">In this example, the specified message has two replies.</span></span> <span data-ttu-id="96689-135">每个答复都有一个或多个[chatMessageMention](../resources/chatmessagemention.md)对象。</span><span class="sxs-lookup"><span data-stu-id="96689-135">Each reply has one or more [chatMessageMention](../resources/chatmessagemention.md) objects.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message_replies"
}-->
```http
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies
```
##### <a name="response"></a><span data-ttu-id="96689-136">响应</span><span class="sxs-lookup"><span data-stu-id="96689-136">Response</span></span>
<span data-ttu-id="96689-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="96689-137">Here is an example of the response.</span></span> 

><span data-ttu-id="96689-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="96689-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/channel-list-messagereplies.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
