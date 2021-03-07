---
title: 获取通道消息
description: 检索团队通道中的单个消息（不包括其回复）。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7f8d0266688c0347e0b21e2bc793e13fbeaac82d
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515910"
---
# <a name="get-channel-message"></a><span data-ttu-id="64db5-103">获取通道消息</span><span class="sxs-lookup"><span data-stu-id="64db5-103">Get channel message</span></span>

<span data-ttu-id="64db5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64db5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="64db5-105">检索团队[通道](../resources/channel.md)中的单个[消息](../resources/chatmessage.md)（不包括其回复）。</span><span class="sxs-lookup"><span data-stu-id="64db5-105">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="64db5-106">权限</span><span class="sxs-lookup"><span data-stu-id="64db5-106">Permissions</span></span>
<span data-ttu-id="64db5-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="64db5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64db5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="64db5-109">Permission Type</span></span>|<span data-ttu-id="64db5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64db5-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="64db5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64db5-111">Delegated (work or school account)</span></span>| <span data-ttu-id="64db5-112">ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="64db5-112">ChannelMessage.Read.All</span></span> |
|<span data-ttu-id="64db5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64db5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64db5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="64db5-114">Not supported.</span></span>|
|<span data-ttu-id="64db5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="64db5-115">Application</span></span>| <span data-ttu-id="64db5-116">ChannelMessage.Read.Group\*、ChannelMessage.Read.All</span><span class="sxs-lookup"><span data-stu-id="64db5-116">ChannelMessage.Read.Group\*, ChannelMessage.Read.All</span></span> |

> <span data-ttu-id="64db5-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="64db5-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="64db5-118">在使用应用程序权限调用此 API 之前，你必须先请求访问权限。</span><span class="sxs-lookup"><span data-stu-id="64db5-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="64db5-119">有关详细信息，请参阅 [Microsoft Teams 中的受保护 API](/graph/teams-protected-apis)。</span><span class="sxs-lookup"><span data-stu-id="64db5-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="64db5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64db5-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="64db5-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="64db5-121">Optional query parameters</span></span>
<span data-ttu-id="64db5-122">目前不支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="64db5-122">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="64db5-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="64db5-123">Request headers</span></span>
| <span data-ttu-id="64db5-124">标头</span><span class="sxs-lookup"><span data-stu-id="64db5-124">Header</span></span>       | <span data-ttu-id="64db5-125">值</span><span class="sxs-lookup"><span data-stu-id="64db5-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="64db5-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="64db5-126">Authorization</span></span>  | <span data-ttu-id="64db5-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64db5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="64db5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="64db5-129">Request body</span></span>
<span data-ttu-id="64db5-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="64db5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64db5-131">响应</span><span class="sxs-lookup"><span data-stu-id="64db5-131">Response</span></span>

<span data-ttu-id="64db5-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64db5-132">If successful, this method returns a `200 OK` response code and a [chatmessage](../resources/chatmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64db5-133">示例</span><span class="sxs-lookup"><span data-stu-id="64db5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64db5-134">请求</span><span class="sxs-lookup"><span data-stu-id="64db5-134">Request</span></span>
<span data-ttu-id="64db5-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64db5-135">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="64db5-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="64db5-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["303d2c1c-f1c5-40ce-b68e-544343d7f42b", "19:fec4b0f2825d4c8c82abc09027a64184@thread.skype", "1555375673184"],
  "name": "get_channel_message"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/303d2c1c-f1c5-40ce-b68e-544343d7f42b/channels/19:fec4b0f2825d4c8c82abc09027a64184@thread.skype/messages/1555375673184
```
# <a name="c"></a>[<span data-ttu-id="64db5-137">C#</span><span class="sxs-lookup"><span data-stu-id="64db5-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-channel-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="64db5-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="64db5-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-channel-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="64db5-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="64db5-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-channel-message-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="64db5-140">Java</span><span class="sxs-lookup"><span data-stu-id="64db5-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-channel-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="64db5-141">响应</span><span class="sxs-lookup"><span data-stu-id="64db5-141">Response</span></span>
<span data-ttu-id="64db5-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="64db5-142">Here is an example of the response.</span></span> 

><span data-ttu-id="64db5-143">**注意：** 为了提高可读性，缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="64db5-143">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="64db5-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="64db5-144">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('303d2c1c-f1c5-40ce-b68e-544343d7f42b')/channels('19%3Afec4b0f2825d4c8c82abc09027a64184%40thread.skype')/messages/$entity",
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
  ]
}
-->


