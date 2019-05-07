---
title: 获取呼叫
description: 检索 call 对象的属性和关系。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2accad64fabf12b578d1d455db08d6aa0b8539e6
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33635790"
---
# <a name="get-call"></a><span data-ttu-id="1cc7f-103">获取呼叫</span><span class="sxs-lookup"><span data-stu-id="1cc7f-103">Get call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cc7f-104">检索 call 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1cc7f-104">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cc7f-105">权限</span><span class="sxs-lookup"><span data-stu-id="1cc7f-105">Permissions</span></span>
<span data-ttu-id="1cc7f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1cc7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1cc7f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1cc7f-108">Permission type</span></span> | <span data-ttu-id="1cc7f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1cc7f-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="1cc7f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1cc7f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1cc7f-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="1cc7f-111">Not Supported.</span></span>                         |
| <span data-ttu-id="1cc7f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1cc7f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc7f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1cc7f-113">Not Supported.</span></span>                         |
| <span data-ttu-id="1cc7f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1cc7f-114">Application</span></span>                            | <span data-ttu-id="1cc7f-115">无。</span><span class="sxs-lookup"><span data-stu-id="1cc7f-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="1cc7f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1cc7f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /applications/{id}/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1cc7f-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1cc7f-117">Optional query parameters</span></span>
<span data-ttu-id="1cc7f-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1cc7f-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1cc7f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1cc7f-119">Request headers</span></span>
| <span data-ttu-id="1cc7f-120">名称</span><span class="sxs-lookup"><span data-stu-id="1cc7f-120">Name</span></span>          | <span data-ttu-id="1cc7f-121">说明</span><span class="sxs-lookup"><span data-stu-id="1cc7f-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1cc7f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cc7f-122">Authorization</span></span> | <span data-ttu-id="1cc7f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1cc7f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cc7f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1cc7f-125">Request body</span></span>
<span data-ttu-id="1cc7f-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1cc7f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cc7f-127">响应</span><span class="sxs-lookup"><span data-stu-id="1cc7f-127">Response</span></span>
<span data-ttu-id="1cc7f-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[call](../resources/call.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1cc7f-128">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cc7f-129">示例</span><span class="sxs-lookup"><span data-stu-id="1cc7f-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1cc7f-130">请求</span><span class="sxs-lookup"><span data-stu-id="1cc7f-130">Request</span></span>
<span data-ttu-id="1cc7f-131">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="1cc7f-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="1cc7f-132">响应</span><span class="sxs-lookup"><span data-stu-id="1cc7f-132">Response</span></span>

> <span data-ttu-id="1cc7f-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1cc7f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.call"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2821

{
  "activeModalities": [
    "unknown"
  ],
  "answeredBy": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "callRoutes": [
    {
      "final": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "original": {
        "phone": {
          "id": "+14258828080"
        }
      },
      "routingType": "forwarded"
    }
  ],
  "callbackUri": "callbackUri-value",
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "direction": "incoming",
  "id": "id-value",
  "mediaConfig": {
    "@odata.type": "#microsoft.graph.appHostedMediaConfig",
    "blob": "<media config blob>"
  },
  "meetingCapability": {
    "allowAnonymousUsersToDialOut": true,
    "allowAnonymousUsersToStartMeeting": true,
    "autoAdmittedUsers": "everyoneInCompany"
  },
  "meetingInfo": {
    "@odata.type": "#microsoft.graph.organizerMeetingInfo",
    "organizer": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "allowConversationWithoutHost": true
  },
  "myParticipantId": "myParticipantId-value",
  "requestedModalities": [
    "audio", "video"
  ],
  "ringingTimeoutInSeconds": 99,
  "routingPolicies": [
    "none"
  ],
  "source": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "state": "incoming",
  "subject": "subject-value",
  "targets": [
    {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value"
    }
  ],
  "tenantId": "tenantId-value",
  "terminationReason": "terminationReason-value",
  "toneInfo": {
    "sequenceId": 99,
    "tone": "tone0"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1cc7f-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1cc7f-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1cc7f-136">语言</span><span class="sxs-lookup"><span data-stu-id="1cc7f-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-call-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1cc7f-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="1cc7f-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-call-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/call-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/call-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
