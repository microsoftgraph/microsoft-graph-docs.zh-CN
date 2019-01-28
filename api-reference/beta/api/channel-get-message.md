---
title: 获取通道消息
description: 检索团队通道中的单个消息（不包括其回复）。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 26b59ac395af3de314469fdb419095bcb6133d6b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523202"
---
# <a name="get-channel-message"></a><span data-ttu-id="a7166-103">获取通道消息</span><span class="sxs-lookup"><span data-stu-id="a7166-103">Get channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7166-104">检索团队[通道](../resources/channel.md)中的单个[消息](../resources/chatmessage.md)（不包括其回复）。</span><span class="sxs-lookup"><span data-stu-id="a7166-104">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7166-105">权限</span><span class="sxs-lookup"><span data-stu-id="a7166-105">Permissions</span></span>
<span data-ttu-id="a7166-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7166-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7166-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7166-108">Permission type</span></span>|<span data-ttu-id="a7166-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7166-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="a7166-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7166-110">Delegated (work or school account)</span></span>|<span data-ttu-id="a7166-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7166-111">Group.Read.All, Group.ReadWrite.All</span></span>|
|<span data-ttu-id="a7166-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7166-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7166-113">不支持</span><span class="sxs-lookup"><span data-stu-id="a7166-113">Not supported</span></span>|
|<span data-ttu-id="a7166-114">Application</span><span class="sxs-lookup"><span data-stu-id="a7166-114">Application</span></span>| <span data-ttu-id="a7166-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7166-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7166-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7166-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a7166-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a7166-117">Optional query parameters</span></span>
<span data-ttu-id="a7166-118">目前不支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="a7166-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7166-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7166-119">Request headers</span></span>
| <span data-ttu-id="a7166-120">标头</span><span class="sxs-lookup"><span data-stu-id="a7166-120">Header</span></span>       | <span data-ttu-id="a7166-121">值</span><span class="sxs-lookup"><span data-stu-id="a7166-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a7166-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7166-122">Authorization</span></span>  | <span data-ttu-id="a7166-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7166-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a7166-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7166-125">Request body</span></span>
<span data-ttu-id="a7166-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7166-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7166-127">响应</span><span class="sxs-lookup"><span data-stu-id="a7166-127">Response</span></span>

<span data-ttu-id="a7166-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a7166-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7166-129">示例</span><span class="sxs-lookup"><span data-stu-id="a7166-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7166-130">请求</span><span class="sxs-lookup"><span data-stu-id="a7166-130">Request</span></span>
<span data-ttu-id="a7166-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7166-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="a7166-132">响应</span><span class="sxs-lookup"><span data-stu-id="a7166-132">Response</span></span>
<span data-ttu-id="a7166-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a7166-133">Here is an example of the response.</span></span> 

><span data-ttu-id="a7166-134">**注意：** 为了提高可读性，缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a7166-134">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="a7166-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a7166-135">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "replyToId": "id-value",
  "from": {
      "user": { 
        "id": "id-value",
        "displayName": "John Doe"
      }  
  },
  "etag": "id-value",
  "messageType": "message",
  "createdDateTime": "2018-07-09T07:40:20.152Z",
  "lastModifiedDateTime": "2018-07-09T07:40:20.152Z",
  "body": {
      "content": "Hello World",
      "contentType": "text"
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
    "Error: /api-reference/beta/api/channel-get-message.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
