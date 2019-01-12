---
title: 列表通道消息
description: '检索 （不带答复） 中的工作组的通道的邮件的列表。 若要获取答复一条消息，请调用列表邮件答复或获取邮件答复 API。 '
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 1af48a84d6ffd39d8e592fa6db54388f4c9460a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966592"
---
# <a name="list-channel-messages"></a><span data-ttu-id="a1aae-104">列表通道消息</span><span class="sxs-lookup"><span data-stu-id="a1aae-104">List channel messages</span></span>

> <span data-ttu-id="a1aae-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a1aae-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1aae-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a1aae-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a1aae-107">检索的[团队](../resources/team.md)[通道](../resources/channel.md)（不带答复） 为[邮件](../resources/chatmessage.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="a1aae-107">Retrieve the list of [messages](../resources/chatmessage.md) (without the replies) in a [channel](../resources/channel.md) of a [team](../resources/team.md).</span></span> <span data-ttu-id="a1aae-108">若要获取答复一条消息，请调用[列表邮件答复](channel-get-messagereply.md)或[获取邮件答复](channel-list-messagereplies.md)API。</span><span class="sxs-lookup"><span data-stu-id="a1aae-108">To get the replies for a message, call the [list message replies](channel-get-messagereply.md) or the [get message reply](channel-list-messagereplies.md) API.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a1aae-109">权限</span><span class="sxs-lookup"><span data-stu-id="a1aae-109">Permissions</span></span>
<span data-ttu-id="a1aae-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1aae-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1aae-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1aae-112">Permission Type</span></span>|<span data-ttu-id="a1aae-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1aae-113">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="a1aae-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1aae-114">Delegated (work or school account)</span></span>|<span data-ttu-id="a1aae-115">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1aae-115">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="a1aae-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1aae-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1aae-117">不支持</span><span class="sxs-lookup"><span data-stu-id="a1aae-117">Not supported</span></span>|
|<span data-ttu-id="a1aae-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1aae-118">Application</span></span>| <span data-ttu-id="a1aae-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1aae-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1aae-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1aae-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1aae-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a1aae-121">Optional query parameters</span></span>
<span data-ttu-id="a1aae-122">目前不支持的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="a1aae-122">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1aae-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1aae-123">Request headers</span></span>
| <span data-ttu-id="a1aae-124">标头</span><span class="sxs-lookup"><span data-stu-id="a1aae-124">Header</span></span>       | <span data-ttu-id="a1aae-125">值</span><span class="sxs-lookup"><span data-stu-id="a1aae-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a1aae-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1aae-126">Authorization</span></span>  | <span data-ttu-id="a1aae-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1aae-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a1aae-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1aae-129">Request body</span></span>
<span data-ttu-id="a1aae-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1aae-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1aae-131">响应</span><span class="sxs-lookup"><span data-stu-id="a1aae-131">Response</span></span>

<span data-ttu-id="a1aae-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[chatmessage](../resources/channel.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a1aae-132">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/channel.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a1aae-133">示例</span><span class="sxs-lookup"><span data-stu-id="a1aae-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1aae-134">请求</span><span class="sxs-lookup"><span data-stu-id="a1aae-134">Request</span></span>
<span data-ttu-id="a1aae-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1aae-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_messages"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
```
##### <a name="response"></a><span data-ttu-id="a1aae-136">响应</span><span class="sxs-lookup"><span data-stu-id="a1aae-136">Response</span></span>
<span data-ttu-id="a1aae-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a1aae-137">Here is an example of the response.</span></span> 

><span data-ttu-id="a1aae-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a1aae-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get channel messages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
