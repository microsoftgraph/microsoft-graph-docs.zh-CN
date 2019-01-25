---
title: 列表通道邮件答复
description: 列表中的工作组的通道的邮件的所有的回复。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4ac3b068e93e370ce981d478c87e573f248695c6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512295"
---
# <a name="list-channel-message-replies"></a><span data-ttu-id="1bab9-103">列表通道邮件答复</span><span class="sxs-lookup"><span data-stu-id="1bab9-103">List channel message replies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bab9-104">列出所有[频道](../resources/channel.md)的工作组中的[邮件](../resources/chatmessage.md)的回复。</span><span class="sxs-lookup"><span data-stu-id="1bab9-104">List all the replies of a [message](../resources/chatmessage.md) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="1bab9-105">权限</span><span class="sxs-lookup"><span data-stu-id="1bab9-105">Permissions</span></span>
<span data-ttu-id="1bab9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1bab9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bab9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bab9-108">Permission Type</span></span>|<span data-ttu-id="1bab9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1bab9-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="1bab9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bab9-110">Delegated (work or school account)</span></span>|<span data-ttu-id="1bab9-111">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bab9-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="1bab9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bab9-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bab9-113">不支持</span><span class="sxs-lookup"><span data-stu-id="1bab9-113">Not supported</span></span>|
|<span data-ttu-id="1bab9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bab9-114">Application</span></span>| <span data-ttu-id="1bab9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bab9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1bab9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bab9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}/replies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1bab9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1bab9-117">Optional query parameters</span></span>
<span data-ttu-id="1bab9-118">目前不支持的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="1bab9-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1bab9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bab9-119">Request headers</span></span>
| <span data-ttu-id="1bab9-120">标头</span><span class="sxs-lookup"><span data-stu-id="1bab9-120">Header</span></span>       | <span data-ttu-id="1bab9-121">值</span><span class="sxs-lookup"><span data-stu-id="1bab9-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1bab9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bab9-122">Authorization</span></span>  | <span data-ttu-id="1bab9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1bab9-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1bab9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bab9-125">Request body</span></span>
<span data-ttu-id="1bab9-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1bab9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1bab9-127">响应</span><span class="sxs-lookup"><span data-stu-id="1bab9-127">Response</span></span>
<span data-ttu-id="1bab9-128">如果成功，此方法返回`200 OK`响应代码和响应正文中的[chatmessage](../resources/channel.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="1bab9-128">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1bab9-129">示例</span><span class="sxs-lookup"><span data-stu-id="1bab9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1bab9-130">请求</span><span class="sxs-lookup"><span data-stu-id="1bab9-130">Request</span></span>
<span data-ttu-id="1bab9-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bab9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message_replies"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}/replies
```
##### <a name="response"></a><span data-ttu-id="1bab9-132">响应</span><span class="sxs-lookup"><span data-stu-id="1bab9-132">Response</span></span>
<span data-ttu-id="1bab9-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1bab9-133">Here is an example of the response.</span></span> 

><span data-ttu-id="1bab9-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1bab9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "value": [
    {
        "id": "id-value",
        "replyToId": "id-value",
        "from" : {
            "user": { 
            "id":  "id-value",
            "displayName": "John Doe"
            }  
        },
        "etag": "id-value",
        "messageType": "message",
        "createdDateTime": "2018-07-09T07:40:20.152Z",
        "lastModifiedDateTime": "2018-07-09T07:40:20.152Z",
        "body": {
            "content": "This is a response to a message.",
            "contentType": "Text"
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
                "type": "user",
                "id": "id-value ",
                "mentionText": "Test User"
            }
        ],
        "importance": "normal",
        "reactions": [
            {
                "reactionType": "like",
                "user": {
                    "id": "id-value",
                    "displayName": "John Doe"
                },
                "createdDateTime": "2018-07-09T07:40:20.152Z"
            }
        ],
        "locale": "en-us"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get channel message replies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list-messagereplies.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
