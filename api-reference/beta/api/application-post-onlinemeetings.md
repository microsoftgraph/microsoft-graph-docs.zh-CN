---
title: 创建联机会议
description: 代表请求正文中指定的用户创建联机会议。
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: dc6521a09bcfaf52b7240d5ad63129fa729d7899
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516866"
---
# <a name="create-online-meeting"></a><span data-ttu-id="880b3-103">创建联机会议</span><span class="sxs-lookup"><span data-stu-id="880b3-103">Create online meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="880b3-104">代表请求正文中指定的用户创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="880b3-104">Creates an online meeting on behalf of a user specified in the request body.</span></span>

> <span data-ttu-id="880b3-105">**注释**：会议不会显示在用户的日历上。</span><span class="sxs-lookup"><span data-stu-id="880b3-105">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="880b3-106">权限</span><span class="sxs-lookup"><span data-stu-id="880b3-106">Permissions</span></span>
<span data-ttu-id="880b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="880b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="880b3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="880b3-109">Permission type</span></span>                        | <span data-ttu-id="880b3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="880b3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="880b3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="880b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="880b3-112">不支持</span><span class="sxs-lookup"><span data-stu-id="880b3-112">Not Supported</span></span>                               |
| <span data-ttu-id="880b3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="880b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="880b3-114">不支持</span><span class="sxs-lookup"><span data-stu-id="880b3-114">Not Supported</span></span>                               |
| <span data-ttu-id="880b3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="880b3-115">Application</span></span>                            | <span data-ttu-id="880b3-116">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="880b3-116">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="880b3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="880b3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /applications/{id}/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="880b3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="880b3-118">Request headers</span></span>
| <span data-ttu-id="880b3-119">名称</span><span class="sxs-lookup"><span data-stu-id="880b3-119">Name</span></span>          | <span data-ttu-id="880b3-120">说明</span><span class="sxs-lookup"><span data-stu-id="880b3-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="880b3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="880b3-121">Authorization</span></span> | <span data-ttu-id="880b3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="880b3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="880b3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="880b3-124">Request body</span></span>
<span data-ttu-id="880b3-125">在请求正文中，提供 [onlineMeeting](../resources/onlinemeeting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="880b3-125">In the request body, supply a JSON representation of an [educationUser](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="880b3-126">响应</span><span class="sxs-lookup"><span data-stu-id="880b3-126">Response</span></span>
<span data-ttu-id="880b3-127">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="880b3-127">If successful, this method returns a `201 Created` response code and an updated [iosCompliancePolicy](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="880b3-128">示例</span><span class="sxs-lookup"><span data-stu-id="880b3-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="880b3-129">请求</span><span class="sxs-lookup"><span data-stu-id="880b3-129">Request</span></span>
<span data-ttu-id="880b3-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="880b3-130">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-from-application"
}-->
```http
POST https://graph.microsoft.com/beta/app/onlineMeetings
Content-Type: application/json
Content-Length: 1553

{
  "meetingType": "meetNow",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  },
  "subject": "subject-value"
}
```

<span data-ttu-id="880b3-131">在请求正文中，提供 [onlineMeeting](../resources/onlinemeeting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="880b3-131">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="880b3-132">响应</span><span class="sxs-lookup"><span data-stu-id="880b3-132">Response</span></span>

><span data-ttu-id="880b3-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="880b3-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1574

{
  "accessLevel": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "participantPasscode": "2425999",
    "leaderPasscode": null,
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "canceledDateTime": "2018-03-19T09:46:02Z",
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2018-03-19T09:46:02Z",
  "endDateTime": "2018-03-19T09:46:02Z",
  "entryExitAnnouncement": true,
  "expirationDateTime": "2018-03-19T09:46:02Z",
  "id": "013448345",
  "isCancelled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "meetingType": "meetNow",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "startDateTime": "2018-03-19T09:46:02Z",
  "subject": "Quarterly sales numbers"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-post-onlinemeetings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
