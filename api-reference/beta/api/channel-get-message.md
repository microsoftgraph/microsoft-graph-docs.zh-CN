---
title: 获取通道消息
description: 检索团队通道中的单个消息（不包括其回复）。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ffd472f93d278b2df09633a8d78733154963a5e2
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889931"
---
# <a name="get-channel-message"></a><span data-ttu-id="f1915-103">获取通道消息</span><span class="sxs-lookup"><span data-stu-id="f1915-103">Get channel message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1915-104">检索团队[通道](../resources/channel.md)中的单个[消息](../resources/chatmessage.md)（不包括其回复）。</span><span class="sxs-lookup"><span data-stu-id="f1915-104">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1915-105">权限</span><span class="sxs-lookup"><span data-stu-id="f1915-105">Permissions</span></span>
<span data-ttu-id="f1915-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1915-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1915-108">Permission Type</span></span>|<span data-ttu-id="f1915-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f1915-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="f1915-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1915-110">Delegated (work or school account)</span></span>|<span data-ttu-id="f1915-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1915-111">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="f1915-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1915-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1915-113">不支持</span><span class="sxs-lookup"><span data-stu-id="f1915-113">Not supported</span></span>|
|<span data-ttu-id="f1915-114">Application</span><span class="sxs-lookup"><span data-stu-id="f1915-114">Application</span></span>| <span data-ttu-id="f1915-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1915-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1915-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1915-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f1915-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f1915-117">Optional query parameters</span></span>
<span data-ttu-id="f1915-118">目前不支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="f1915-118">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1915-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1915-119">Request headers</span></span>
| <span data-ttu-id="f1915-120">标头</span><span class="sxs-lookup"><span data-stu-id="f1915-120">Header</span></span>       | <span data-ttu-id="f1915-121">值</span><span class="sxs-lookup"><span data-stu-id="f1915-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1915-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1915-122">Authorization</span></span>  | <span data-ttu-id="f1915-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f1915-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1915-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1915-125">Request body</span></span>
<span data-ttu-id="f1915-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f1915-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1915-127">响应</span><span class="sxs-lookup"><span data-stu-id="f1915-127">Response</span></span>

<span data-ttu-id="f1915-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [chatmessage](../resources/chatmessage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f1915-128">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1915-129">示例</span><span class="sxs-lookup"><span data-stu-id="f1915-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1915-130">请求</span><span class="sxs-lookup"><span data-stu-id="f1915-130">Request</span></span>
<span data-ttu-id="f1915-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f1915-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="f1915-132">响应</span><span class="sxs-lookup"><span data-stu-id="f1915-132">Response</span></span>
<span data-ttu-id="f1915-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f1915-133">Here is an example of the response.</span></span> 

><span data-ttu-id="f1915-134">**注意：** 为了提高可读性，缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f1915-134">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="f1915-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f1915-135">All the properties will be returned from an actual call.</span></span>
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
          "id": "id-value ",
          "mentionText": "Test User",
          "mentioned": {
          "user": {
            "id": "id-value",
            "displayName: "string"
          }
        }
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
