---
title: 获取频道消息
description: 检索单个邮件 （不带及其答复） 中的工作组的通道。
author: nkramer
localization_priority: Priority
ms.openlocfilehash: 202e2c341e58175e1807e1aa47c120f6c829a7c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829118"
---
# <a name="get-channel-message"></a><span data-ttu-id="806ee-103">获取频道消息</span><span class="sxs-lookup"><span data-stu-id="806ee-103">Get channel message</span></span>

> <span data-ttu-id="806ee-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="806ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="806ee-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="806ee-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="806ee-106">检索单个[邮件](../resources/chatmessage.md)（不带及其答复） 中的工作组[通道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="806ee-106">Retrieve a single [message](../resources/chatmessage.md) (without its replies) in a [channel](../resources/channel.md) of a team.</span></span>

## <a name="permissions"></a><span data-ttu-id="806ee-107">权限</span><span class="sxs-lookup"><span data-stu-id="806ee-107">Permissions</span></span>
<span data-ttu-id="806ee-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="806ee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="806ee-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="806ee-110">Permission Type</span></span>|<span data-ttu-id="806ee-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="806ee-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="806ee-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="806ee-112">Delegated (work or school account)</span></span>|<span data-ttu-id="806ee-113">Group.Read.All,Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="806ee-113">Group.Read.All,Group.ReadWrite.All</span></span>|
|<span data-ttu-id="806ee-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="806ee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="806ee-115">不支持</span><span class="sxs-lookup"><span data-stu-id="806ee-115">Not supported</span></span>|
|<span data-ttu-id="806ee-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="806ee-116">Application</span></span>| <span data-ttu-id="806ee-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="806ee-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="806ee-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="806ee-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /teams/{id}/channels/{id}/messages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="806ee-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="806ee-119">Optional query parameters</span></span>
<span data-ttu-id="806ee-120">目前不支持的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)。</span><span class="sxs-lookup"><span data-stu-id="806ee-120">The [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) are not currently supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="806ee-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="806ee-121">Request headers</span></span>
| <span data-ttu-id="806ee-122">标头</span><span class="sxs-lookup"><span data-stu-id="806ee-122">Header</span></span>       | <span data-ttu-id="806ee-123">值</span><span class="sxs-lookup"><span data-stu-id="806ee-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="806ee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="806ee-124">Authorization</span></span>  | <span data-ttu-id="806ee-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="806ee-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="806ee-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="806ee-127">Request body</span></span>
<span data-ttu-id="806ee-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="806ee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="806ee-129">响应</span><span class="sxs-lookup"><span data-stu-id="806ee-129">Response</span></span>

<span data-ttu-id="806ee-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[chatmessage](../resources/chatmessage.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="806ee-130">If successful, this method returns a `200 OK` response code and a collection of [chatmessage](../resources/chatmessage.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="806ee-131">示例</span><span class="sxs-lookup"><span data-stu-id="806ee-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="806ee-132">请求</span><span class="sxs-lookup"><span data-stu-id="806ee-132">Request</span></span>
<span data-ttu-id="806ee-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="806ee-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_channel_message"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages/{id}
```
##### <a name="response"></a><span data-ttu-id="806ee-134">响应</span><span class="sxs-lookup"><span data-stu-id="806ee-134">Response</span></span>
<span data-ttu-id="806ee-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="806ee-135">Here is an example of the response.</span></span> 

><span data-ttu-id="806ee-136">**注意：** 为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="806ee-136">**Note:** The response object shown here are shortened for readability.</span></span> <span data-ttu-id="806ee-137">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="806ee-137">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get channel message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
