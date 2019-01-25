---
title: Get 联机会议
description: 检索的属性和**onlineMeeting**对象的关系。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ef45d73aef8124d962d05ea84117c93bac16f0a2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510650"
---
# <a name="get-online-meeting"></a><span data-ttu-id="94f88-103">Get 联机会议</span><span class="sxs-lookup"><span data-stu-id="94f88-103">Get Online Meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94f88-104">检索的属性和**onlineMeeting**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="94f88-104">Retrieve the properties and relationships of an **onlineMeeting** object.</span></span>

> <span data-ttu-id="94f88-105">**注意：**`GET`方法仅限于[VTC 会议 id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up)。云视频互操作许可用户并使用此方法来获取要加入会议的详细信息，将生成这些 Id。</span><span class="sxs-lookup"><span data-stu-id="94f88-105">**Note:** The `GET` method is limited to a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>
> <span data-ttu-id="94f88-106">对于正则流，自动程序可以使用`joinURL`要加入会议时，没有查阅有必要。</span><span class="sxs-lookup"><span data-stu-id="94f88-106">For regular flows, the bot can use the `joinURL` to join a meeting and no lookup is necessary.</span></span>

## <a name="permissions"></a><span data-ttu-id="94f88-107">权限</span><span class="sxs-lookup"><span data-stu-id="94f88-107">Permissions</span></span>

<span data-ttu-id="94f88-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94f88-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="94f88-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="94f88-110">Permission type</span></span>                        | <span data-ttu-id="94f88-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94f88-111">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="94f88-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94f88-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="94f88-113">不受支持。</span><span class="sxs-lookup"><span data-stu-id="94f88-113">Not Supported.</span></span>                                        |
| <span data-ttu-id="94f88-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94f88-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94f88-115">不受支持。</span><span class="sxs-lookup"><span data-stu-id="94f88-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="94f88-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="94f88-116">Application</span></span>                            | <span data-ttu-id="94f88-117">OnlineMeetings.Read.All OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94f88-117">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94f88-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94f88-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/{id}
GET /applications/{id}/onlineMeetings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="94f88-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="94f88-119">Optional query parameters</span></span>
<span data-ttu-id="94f88-120">此方法支持[OData 查询参数](/graph/query-parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="94f88-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94f88-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="94f88-121">Request headers</span></span>
| <span data-ttu-id="94f88-122">名称</span><span class="sxs-lookup"><span data-stu-id="94f88-122">Name</span></span>          | <span data-ttu-id="94f88-123">说明</span><span class="sxs-lookup"><span data-stu-id="94f88-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="94f88-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="94f88-124">Authorization</span></span> | <span data-ttu-id="94f88-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94f88-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94f88-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="94f88-127">Request body</span></span>
<span data-ttu-id="94f88-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94f88-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="94f88-129">响应</span><span class="sxs-lookup"><span data-stu-id="94f88-129">Response</span></span>
<span data-ttu-id="94f88-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和[onlineMeeting](../resources/onlinemeeting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94f88-130">If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94f88-131">示例</span><span class="sxs-lookup"><span data-stu-id="94f88-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="94f88-132">请求</span><span class="sxs-lookup"><span data-stu-id="94f88-132">Request</span></span>
<span data-ttu-id="94f88-133">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="94f88-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```http
GET https://graph.microsoft.com/beta/app/onlineMeetings/{id}
```

##### <a name="response"></a><span data-ttu-id="94f88-134">响应</span><span class="sxs-lookup"><span data-stu-id="94f88-134">Response</span></span>

> <span data-ttu-id="94f88-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="94f88-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 200 OK
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
  "meetingType": "scheduled",
  "participants": {
    "attendees": [
      {
        "identity": {
          "user": {
            "id": "550fae72-d251-43ec-868c-373732c2704f",
            "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
            "displayName": "Heidi Steen"
          }
        },
        "upn": "upn-value"
      }
    ],
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
  "description": "Get onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/onlinemeeting-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
