---
title: 获取呼叫
description: 检索 call 对象的属性和关系。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 5e7760516f248415139403cd404081839b0dbe5d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964490"
---
# <a name="get-call"></a><span data-ttu-id="e4688-103">获取呼叫</span><span class="sxs-lookup"><span data-stu-id="e4688-103">Get call</span></span>

<span data-ttu-id="e4688-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4688-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4688-105">检索 call 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e4688-105">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4688-106">权限</span><span class="sxs-lookup"><span data-stu-id="e4688-106">Permissions</span></span>
<span data-ttu-id="e4688-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4688-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4688-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4688-109">Permission type</span></span> | <span data-ttu-id="e4688-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4688-110">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="e4688-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4688-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4688-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4688-112">Not Supported.</span></span>                         |
| <span data-ttu-id="e4688-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4688-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4688-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4688-114">Not Supported.</span></span>                         |
| <span data-ttu-id="e4688-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4688-115">Application</span></span>                            | <span data-ttu-id="e4688-116">无。</span><span class="sxs-lookup"><span data-stu-id="e4688-116">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="e4688-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4688-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4688-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e4688-118">Optional query parameters</span></span>
<span data-ttu-id="e4688-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e4688-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4688-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4688-120">Request headers</span></span>
| <span data-ttu-id="e4688-121">名称</span><span class="sxs-lookup"><span data-stu-id="e4688-121">Name</span></span>          | <span data-ttu-id="e4688-122">说明</span><span class="sxs-lookup"><span data-stu-id="e4688-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="e4688-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4688-123">Authorization</span></span> | <span data-ttu-id="e4688-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e4688-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4688-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4688-126">Request body</span></span>
<span data-ttu-id="e4688-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e4688-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4688-128">响应</span><span class="sxs-lookup"><span data-stu-id="e4688-128">Response</span></span>
<span data-ttu-id="e4688-129">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/call.md) 代码和 call 对象。</span><span class="sxs-lookup"><span data-stu-id="e4688-129">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e4688-130">示例</span><span class="sxs-lookup"><span data-stu-id="e4688-130">Examples</span></span>

### <a name="example-1-getting-a-peer-to-peer-call"></a><span data-ttu-id="e4688-131">示例 1：获取对等呼叫</span><span class="sxs-lookup"><span data-stu-id="e4688-131">Example 1: Getting a Peer-to-Peer call</span></span>

##### <a name="request"></a><span data-ttu-id="e4688-132">请求</span><span class="sxs-lookup"><span data-stu-id="e4688-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e4688-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4688-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call-1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/{id}
```
# <a name="c"></a>[<span data-ttu-id="e4688-134">C#</span><span class="sxs-lookup"><span data-stu-id="e4688-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4688-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4688-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4688-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4688-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4688-137">Java</span><span class="sxs-lookup"><span data-stu-id="e4688-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e4688-138">响应</span><span class="sxs-lookup"><span data-stu-id="e4688-138">Response</span></span>

> <span data-ttu-id="e4688-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e4688-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.invitationParticipantInfo",
      "identity": {
        "@odata.type": "#microsoft.graph.identitySet",
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "displayName": "John",
          "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      }
    }
  ],
  "requestedModalities": [
    "audio"
  ],
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
  "myParticipantId": "499ff390-7a72-40e8-83a0-8fac6295ae7e",
  "id": "2e1a0b00-2db4-4022-9570-243709c565ab",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/calls/$entity",
  "subject": null,
  "ringingTimeoutInSeconds": null,
  "resultInfo": null,
  "answeredBy": null,
  "chatInfo": null,
  "meetingInfo": null,
  "transcription": null,
  "toneInfo": null
}
```
### <a name="example-2-getting-a-group-call"></a><span data-ttu-id="e4688-141">示例 2：获取组呼叫</span><span class="sxs-lookup"><span data-stu-id="e4688-141">Example 2: Getting a group call</span></span>

##### <a name="request"></a><span data-ttu-id="e4688-142">请求</span><span class="sxs-lookup"><span data-stu-id="e4688-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e4688-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="e4688-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-call-2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/calls/2f1a1100-b174-40a0-aba7-0b405e01ed92
```
# <a name="c"></a>[<span data-ttu-id="e4688-144">C#</span><span class="sxs-lookup"><span data-stu-id="e4688-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-call-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e4688-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e4688-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-call-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e4688-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e4688-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-call-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e4688-147">Java</span><span class="sxs-lookup"><span data-stu-id="e4688-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-call-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e4688-148">响应</span><span class="sxs-lookup"><span data-stu-id="e4688-148">Response</span></span>

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
        "displayName": null
      }
    },
    "allowConversationWithoutHost": true
  },
  "transcription": {
    "@odata.type": "#microsoft.graph.callTranscriptionInfo",
    "state": "inactive",
    "lastModifiedDateTime": "2020-05-28T00:10:54.104318Z"
  },
  "myParticipantId": "05491616-385f-44a8-9974-18cc5f9933c1",
  "id": "2f1a1100-b174-40a0-aba7-0b405e01ed92",
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#communications/calls/$entity",
  "ringingTimeoutInSeconds": null,
  "subject": null,
  "resultInfo": null,
  "answeredBy": null,
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

