---
title: 获取呼叫
description: 检索 call 对象的属性和关系。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 27e6ed2cb7edf7988ef9afc5702a8237b9b219f5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328125"
---
# <a name="get-call"></a><span data-ttu-id="96a7e-103">获取呼叫</span><span class="sxs-lookup"><span data-stu-id="96a7e-103">Get call</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96a7e-104">检索 call 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="96a7e-104">Retrieve the properties and relationships of a call object.</span></span>

## <a name="permissions"></a><span data-ttu-id="96a7e-105">权限</span><span class="sxs-lookup"><span data-stu-id="96a7e-105">Permissions</span></span>
<span data-ttu-id="96a7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96a7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96a7e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="96a7e-108">Permission type</span></span> | <span data-ttu-id="96a7e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96a7e-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="96a7e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96a7e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="96a7e-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="96a7e-111">Not Supported.</span></span>                         |
| <span data-ttu-id="96a7e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96a7e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96a7e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="96a7e-113">Not Supported.</span></span>                         |
| <span data-ttu-id="96a7e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="96a7e-114">Application</span></span>                            | <span data-ttu-id="96a7e-115">无。</span><span class="sxs-lookup"><span data-stu-id="96a7e-115">None.</span></span>                                  |

## <a name="http-request"></a><span data-ttu-id="96a7e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96a7e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}
GET /applications/{id}/calls/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96a7e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="96a7e-117">Optional query parameters</span></span>
<span data-ttu-id="96a7e-118">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="96a7e-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96a7e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="96a7e-119">Request headers</span></span>
| <span data-ttu-id="96a7e-120">名称</span><span class="sxs-lookup"><span data-stu-id="96a7e-120">Name</span></span>          | <span data-ttu-id="96a7e-121">说明</span><span class="sxs-lookup"><span data-stu-id="96a7e-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="96a7e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96a7e-122">Authorization</span></span> | <span data-ttu-id="96a7e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96a7e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96a7e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="96a7e-125">Request body</span></span>
<span data-ttu-id="96a7e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96a7e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96a7e-127">响应</span><span class="sxs-lookup"><span data-stu-id="96a7e-127">Response</span></span>
<span data-ttu-id="96a7e-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[call](../resources/call.md)对象。</span><span class="sxs-lookup"><span data-stu-id="96a7e-128">If successful, this method returns a `200 OK` response code and a [call](../resources/call.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96a7e-129">示例</span><span class="sxs-lookup"><span data-stu-id="96a7e-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="96a7e-130">请求</span><span class="sxs-lookup"><span data-stu-id="96a7e-130">Request</span></span>
<span data-ttu-id="96a7e-131">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="96a7e-131">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-call"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}
```

##### <a name="response"></a><span data-ttu-id="96a7e-132">响应</span><span class="sxs-lookup"><span data-stu-id="96a7e-132">Response</span></span>

> <span data-ttu-id="96a7e-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="96a7e-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
