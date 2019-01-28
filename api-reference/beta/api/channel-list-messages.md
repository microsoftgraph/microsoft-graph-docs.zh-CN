---
title: 列出频道消息
description: '检索团队频道中的消息列表（无回复）。 若要获取消息的回复，请调用“列出消息回复”或“获取消息回复”API。 '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: bbd2020e85d011b4e94af1d0e56096d4375b41d3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529171"
---
# <a name="list-channel-messages"></a><span data-ttu-id="fea37-104">列出频道消息</span><span class="sxs-lookup"><span data-stu-id="fea37-104">List channel messages</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fea37-105">检索[团队](../resources/team.md)[频道](../resources/channel.md)中的[消息](../resources/chatmessage.md)列表（无回复）。</span><span class="sxs-lookup"><span data-stu-id="fea37-105">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="fea37-106">若要获取消息的回复，请调用[列出消息回复](channel-get-messagereply.md)或[获取消息回复](channel-list-messagereplies.md) API。</span><span class="sxs-lookup"><span data-stu-id="fea37-106">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fea37-107">权限</span><span class="sxs-lookup"><span data-stu-id="fea37-107">Permissions</span></span>
<span data-ttu-id="fea37-p103">需要以下权限之一才能调用此 API。若要了解详细信息（包括如何选择权限），请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fea37-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fea37-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fea37-110">Permission type</span></span>|<span data-ttu-id="fea37-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fea37-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="fea37-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fea37-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fea37-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fea37-113">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="fea37-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fea37-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fea37-115">不支持</span><span class="sxs-lookup"><span data-stu-id="fea37-115">Not supported</span></span>|
|<span data-ttu-id="fea37-116">Application</span><span class="sxs-lookup"><span data-stu-id="fea37-116">Application</span></span>| <span data-ttu-id="fea37-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fea37-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fea37-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fea37-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fea37-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fea37-119">Optional query parameters</span></span>
<span data-ttu-id="fea37-120">目前不支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="fea37-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fea37-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fea37-121">Request headers</span></span>
| <span data-ttu-id="fea37-122">标头</span><span class="sxs-lookup"><span data-stu-id="fea37-122">Header</span></span>       | <span data-ttu-id="fea37-123">值</span><span class="sxs-lookup"><span data-stu-id="fea37-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fea37-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fea37-124">Authorization</span></span>  | <span data-ttu-id="fea37-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fea37-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fea37-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fea37-127">Request body</span></span>
<span data-ttu-id="fea37-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fea37-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fea37-129">响应</span><span class="sxs-lookup"><span data-stu-id="fea37-129">Response</span></span>

<span data-ttu-id="fea37-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fea37-130">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/chatmessage.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fea37-131">示例</span><span class="sxs-lookup"><span data-stu-id="fea37-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fea37-132">请求</span><span class="sxs-lookup"><span data-stu-id="fea37-132">Request</span></span>
<span data-ttu-id="fea37-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fea37-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_messages"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="fea37-134">响应</span><span class="sxs-lookup"><span data-stu-id="fea37-134">Response</span></span>
<span data-ttu-id="fea37-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fea37-135">Here is an example of the response.</span></span> 

><span data-ttu-id="fea37-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fea37-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
            "content": "Hello World",
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
  "description": "Get channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/channel-list-messages.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
