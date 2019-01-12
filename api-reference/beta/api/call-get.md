---
title: 获取呼叫
description: 检索的属性和呼叫对象的关系。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 20243a003cccfc5b39e0aad600afa887e5803849
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966529"
---
# <a name="get-call"></a><span data-ttu-id="dfa78-103">获取呼叫</span><span class="sxs-lookup"><span data-stu-id="dfa78-103">Get call</span></span>

> <span data-ttu-id="dfa78-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dfa78-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfa78-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dfa78-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dfa78-106">检索的属性和呼叫对象的关系。</span><span class="sxs-lookup"><span data-stu-id="dfa78-106">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfa78-107">权限</span><span class="sxs-lookup"><span data-stu-id="dfa78-107">Permissions</span></span>
<span data-ttu-id="dfa78-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfa78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfa78-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfa78-110">Permission type</span></span> | <span data-ttu-id="dfa78-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dfa78-111">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="dfa78-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfa78-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfa78-113">不受支持。</span><span class="sxs-lookup"><span data-stu-id="dfa78-113">Not Supported.</span></span>                         |
| <span data-ttu-id="dfa78-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfa78-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfa78-115">不受支持。</span><span class="sxs-lookup"><span data-stu-id="dfa78-115">Not Supported.</span></span>                         |
| <span data-ttu-id="dfa78-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfa78-116">Application</span></span>                            | <span data-ttu-id="dfa78-117">无。</span><span class="sxs-lookup"><span data-stu-id="dfa78-117">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="dfa78-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfa78-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /applications/{id}/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dfa78-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dfa78-119">Optional query parameters</span></span>
<span data-ttu-id="dfa78-120">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="dfa78-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfa78-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfa78-121">Request headers</span></span>
| <span data-ttu-id="dfa78-122">名称</span><span class="sxs-lookup"><span data-stu-id="dfa78-122">Name</span></span>          | <span data-ttu-id="dfa78-123">说明</span><span class="sxs-lookup"><span data-stu-id="dfa78-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="dfa78-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfa78-124">Authorization</span></span> | <span data-ttu-id="dfa78-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dfa78-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfa78-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfa78-127">Request body</span></span>
<span data-ttu-id="dfa78-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dfa78-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfa78-129">响应</span><span class="sxs-lookup"><span data-stu-id="dfa78-129">Response</span></span>
<span data-ttu-id="dfa78-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[呼叫](../resources/call.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dfa78-130">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfa78-131">示例</span><span class="sxs-lookup"><span data-stu-id="dfa78-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dfa78-132">请求</span><span class="sxs-lookup"><span data-stu-id="dfa78-132">Request</span></span>
<span data-ttu-id="dfa78-133">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="dfa78-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="dfa78-134">响应</span><span class="sxs-lookup"><span data-stu-id="dfa78-134">Response</span></span>

> <span data-ttu-id="dfa78-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dfa78-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
