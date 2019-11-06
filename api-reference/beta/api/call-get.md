---
title: 获取呼叫
description: 检索 call 对象的属性和关系。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: b157f6b5233b7f83ed5530239478dd1858273d6f
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006338"
---
# <a name="get-call"></a><span data-ttu-id="a4ad1-103">获取呼叫</span><span class="sxs-lookup"><span data-stu-id="a4ad1-103">Get call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4ad1-104">检索 call 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a4ad1-104">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4ad1-105">Permissions</span><span class="sxs-lookup"><span data-stu-id="a4ad1-105">Permissions</span></span>
<span data-ttu-id="a4ad1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4ad1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4ad1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4ad1-108">Permission type</span></span> | <span data-ttu-id="a4ad1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4ad1-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="a4ad1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4ad1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a4ad1-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4ad1-111">Not Supported.</span></span>                         |
| <span data-ttu-id="a4ad1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4ad1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4ad1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4ad1-113">Not Supported.</span></span>                         |
| <span data-ttu-id="a4ad1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4ad1-114">Application</span></span>                            | <span data-ttu-id="a4ad1-115">无。</span><span class="sxs-lookup"><span data-stu-id="a4ad1-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="a4ad1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4ad1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /communications/calls/{id}
```
> <span data-ttu-id="a4ad1-117">**注意：**`/app`路径已被弃用。</span><span class="sxs-lookup"><span data-stu-id="a4ad1-117">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="a4ad1-118">接下来，请使用`/communications`路径。</span><span class="sxs-lookup"><span data-stu-id="a4ad1-118">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="a4ad1-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a4ad1-119">Optional query parameters</span></span>
<span data-ttu-id="a4ad1-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a4ad1-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4ad1-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4ad1-121">Request headers</span></span>
| <span data-ttu-id="a4ad1-122">名称</span><span class="sxs-lookup"><span data-stu-id="a4ad1-122">Name</span></span>          | <span data-ttu-id="a4ad1-123">说明</span><span class="sxs-lookup"><span data-stu-id="a4ad1-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="a4ad1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4ad1-124">Authorization</span></span> | <span data-ttu-id="a4ad1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4ad1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4ad1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4ad1-127">Request body</span></span>
<span data-ttu-id="a4ad1-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a4ad1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4ad1-129">响应</span><span class="sxs-lookup"><span data-stu-id="a4ad1-129">Response</span></span>
<span data-ttu-id="a4ad1-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[call](../resources/call.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a4ad1-130">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a4ad1-131">示例</span><span class="sxs-lookup"><span data-stu-id="a4ad1-131">Examples</span></span>

### <a name="example-1-getting-a-peer-to-peer-call"></a><span data-ttu-id="a4ad1-132">示例1：获取对等呼叫</span><span class="sxs-lookup"><span data-stu-id="a4ad1-132">Example 1: Getting a Peer-to-Peer call</span></span>

##### <a name="request"></a><span data-ttu-id="a4ad1-133">请求</span><span class="sxs-lookup"><span data-stu-id="a4ad1-133">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a4ad1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4ad1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/calls/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4ad1-135">C#</span><span class="sxs-lookup"><span data-stu-id="a4ad1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4ad1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4ad1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4ad1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4ad1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a4ad1-138">响应</span><span class="sxs-lookup"><span data-stu-id="a4ad1-138">Response</span></span>

> <span data-ttu-id="a4ad1-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a4ad1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "established",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6",
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [
    {
      "@odata.type": "#microsoft.graph.participantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      },
      "region": null,
      "languageId": null
    }
  ],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "subject": null,
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "meetingCapability": null,
  "toneInfo": null
}
```
### <a name="example-2-getting-a-group-call"></a><span data-ttu-id="a4ad1-141">示例2：获取组呼叫</span><span class="sxs-lookup"><span data-stu-id="a4ad1-141">Example 2: Getting a group call</span></span>

##### <a name="request"></a><span data-ttu-id="a4ad1-142">请求</span><span class="sxs-lookup"><span data-stu-id="a4ad1-142">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```http
GET https://graph.microsoft.com/beta/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
```

##### <a name="response"></a><span data-ttu-id="a4ad1-143">响应</span><span class="sxs-lookup"><span data-stu-id="a4ad1-143">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": "true",
  "@odata.type": "microsoft.graph.call"
}-->
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.call",
  "state": "established",
  "direction": "outgoing",
  "callbackUri": "https://bot.contoso.com/callback",
  "callRoutes": [],
  "source": {
    "@odata.type": "#microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "#microsoft.graph.identitySet",
      "application": {
        "@odata.type": "#microsoft.graph.identity",
        "displayName": "Calling Bot",
        "id": "2891555a-92ff-42e6-80fa-6e1300c6b5c6",
      }
    },
    "region": null,
    "languageId": null
  },
  "targets": [],
  "requestedModalities": [
    "audio"
  ],
  "activeModalities": [],
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.serviceHostedMediaConfig",
    "preFetchMedia": [
     {
       "uri": "https://cdn.contoso.com/beep.wav",
       "resourceId": "f8971b04-b53e-418c-9222-c82ce681a582"
     },
     {
       "uri": "https://cdn.contoso.com/cool.wav",
       "resourceId": "86dc814b-c172-4428-9112-60f8ecae1edb"
     }
    ],
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:meeting_Win6Ydo4wsMijFjZS00ZGVjLTk5MGUtOTRjNWY2NmNkYTFm@thread.v2",
    "messageId": "0",
    "replyChainMessageId": null
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "user": {
        "@odata.type": "#microsoft.graph.identity",
        "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
        "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
        "displayName": null
      }
    },
    "allowConversationWithoutHost": true
  },
  "routingPolicies": [],
  "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
  "myParticipantId": "05491616-385f-44a8-9974-18cc5f9933c1",
  "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#app/calls/$entity",
  "terminationReason": null,
  "ringingTimeoutInSeconds": null,
  "subject": null,
  "resultInfo": null,
  "answeredBy": null,
  "meetingCapability": null,
  "toneInfo": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
