---
title: 列出频道邮件答复
description: 在团队的频道中列出邮件的所有答复。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f9dbee6a85b6f0b569f14c8970b9f42a8760e59b
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000523"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="5e7a5-103">列出频道邮件答复</span><span class="sxs-lookup"><span data-stu-id="5e7a5-103">List channel message replies</span></span>

<span data-ttu-id="5e7a5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e7a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e7a5-105">在团队的[频道](../resources/channel.md)中列出[邮件](../resources/chatmessage.md)的所有答复。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-105">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

<span data-ttu-id="5e7a5-106">此方法仅列出指定邮件的答复（如果有）。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-106">This method lists only the replies of the specified message, if any.</span></span> <span data-ttu-id="5e7a5-107">若要获取邮件本身，只需调用 [get 信道消息](channel-get-message.md)即可。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-107">To get the message itself, simply call [get channel message](channel-get-message.md).</span></span>

> <span data-ttu-id="5e7a5-108">**注意** ：此 API 支持订阅使用 [更改通知](../resources/webhooks.md) (创建、更新和删除) 更改。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-108">**Note** : This API supports subscribing to changes (create, update, and delete) using [change notifications](../resources/webhooks.md).</span></span> <span data-ttu-id="5e7a5-109">这允许呼叫者实时订阅和获取更改。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-109">This allows callers to subscribe and get changes in real time.</span></span> <span data-ttu-id="5e7a5-110">有关详细信息，请参阅 [获取邮件通知](/graph/teams-changenotifications-chatmessage)。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-110">For details, see [Get notifications for messages](/graph/teams-changenotifications-chatmessage).</span></span>

## <a name="permissions"></a><span data-ttu-id="5e7a5-111">权限</span><span class="sxs-lookup"><span data-stu-id="5e7a5-111">Permissions</span></span>
<span data-ttu-id="5e7a5-p103">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e7a5-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e7a5-114">Permission Type</span></span>|<span data-ttu-id="5e7a5-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e7a5-115">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="5e7a5-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e7a5-116">Delegated (work or school account)</span></span>| <span data-ttu-id="5e7a5-117">ChannelMessage.Read.All、Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e7a5-117">ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |
|<span data-ttu-id="5e7a5-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e7a5-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e7a5-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-119">Not supported.</span></span>|
|<span data-ttu-id="5e7a5-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e7a5-120">Application</span></span>| <span data-ttu-id="5e7a5-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e7a5-121">ChannelMessage.Read.Group\*, ChannelMessage.Read.All, Group.Read.All, Group.ReadWrite.All</span></span> |

> <span data-ttu-id="5e7a5-122">**注意** ：标有 \* 的权限使用 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-122">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="5e7a5-p104">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。有关详细信息，请参阅 [Microsoft Teams 中受保护的 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-p104">Before calling this API with application permissions, you must request access. For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="5e7a5-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e7a5-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5e7a5-126">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5e7a5-126">Optional query parameters</span></span>

<span data-ttu-id="5e7a5-p105">可以使用 [$ top](/graph/query-parameters#top-parameter) 查询参数来控制每个响应的项目​​数。当前不支持其他 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-p105">You can use the [$top](/graph/query-parameters#top-parameter) query parameter to control the number of items per response. The other [OData query parameters](/graph/query-parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e7a5-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e7a5-129">Request headers</span></span>
| <span data-ttu-id="5e7a5-130">标头</span><span class="sxs-lookup"><span data-stu-id="5e7a5-130">Header</span></span>       | <span data-ttu-id="5e7a5-131">值</span><span class="sxs-lookup"><span data-stu-id="5e7a5-131">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5e7a5-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e7a5-132">Authorization</span></span>  | <span data-ttu-id="5e7a5-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e7a5-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e7a5-135">Request body</span></span>
<span data-ttu-id="5e7a5-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5e7a5-137">响应</span><span class="sxs-lookup"><span data-stu-id="5e7a5-137">Response</span></span>
<span data-ttu-id="5e7a5-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-138">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e7a5-139">示例</span><span class="sxs-lookup"><span data-stu-id="5e7a5-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e7a5-140">请求</span><span class="sxs-lookup"><span data-stu-id="5e7a5-140">Request</span></span>
<span data-ttu-id="5e7a5-141">在此示例中，指定的邮件有两个答复。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-141">In this example, the specified message has two replies.</span></span> <span data-ttu-id="5e7a5-142">每个答复都有一个或多个 [chatMessageMention](../resources/chatmessagemention.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-142">Each reply has one or more [chatMessageMention](../resources/chatmessagemention.md) objects.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e7a5-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e7a5-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message_replies"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184/replies
```
# <a name="c"></a>[<span data-ttu-id="5e7a5-144">C#</span><span class="sxs-lookup"><span data-stu-id="5e7a5-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-replies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e7a5-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e7a5-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-replies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e7a5-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e7a5-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-replies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e7a5-147">Java</span><span class="sxs-lookup"><span data-stu-id="5e7a5-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-message-replies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="5e7a5-148">响应</span><span class="sxs-lookup"><span data-stu-id="5e7a5-148">Response</span></span>
<span data-ttu-id="5e7a5-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-149">Here is an example of the response.</span></span> 

><span data-ttu-id="5e7a5-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5e7a5-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
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
            "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
            "lastEditedDateTime": null,
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

