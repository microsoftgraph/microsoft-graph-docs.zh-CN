---
title: 获取联机会议
description: 检索**onlineMeeting**对象的属性和关系。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: da94541540989ef8e85c89e5fd64ea4b75867d91
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265896"
---
# <a name="get-online-meeting"></a><span data-ttu-id="7b518-103">获取联机会议</span><span class="sxs-lookup"><span data-stu-id="7b518-103">Get Online Meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b518-104">检索**onlineMeeting**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7b518-104">Retrieve the properties and relationships of an **onlineMeeting** object.</span></span>

> <span data-ttu-id="7b518-105">**注意:** 此`GET`方法限制为[VTC 会议 id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up)。这些 Id 是为云-视频互操作许可的用户生成的, 此方法用于获取加入会议的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7b518-105">**Note:** The `GET` method is limited to a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>
> <span data-ttu-id="7b518-106">对于常规流, bot 可以使用`joinURL`加入会议, 而无需进行查找。</span><span class="sxs-lookup"><span data-stu-id="7b518-106">For regular flows, the bot can use the `joinURL` to join a meeting and no lookup is necessary.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b518-107">权限</span><span class="sxs-lookup"><span data-stu-id="7b518-107">Permissions</span></span>

<span data-ttu-id="7b518-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7b518-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b518-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7b518-110">Permission type</span></span>                        | <span data-ttu-id="7b518-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7b518-111">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="7b518-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7b518-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b518-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b518-113">Not Supported.</span></span>                                        |
| <span data-ttu-id="7b518-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7b518-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b518-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7b518-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="7b518-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7b518-116">Application</span></span>                            | <span data-ttu-id="7b518-117">OnlineMeetings、OnlineMeetings 和所有</span><span class="sxs-lookup"><span data-stu-id="7b518-117">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7b518-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7b518-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/{id}
GET /applications/{id}/onlineMeetings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b518-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7b518-119">Optional query parameters</span></span>
<span data-ttu-id="7b518-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7b518-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b518-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7b518-121">Request headers</span></span>
| <span data-ttu-id="7b518-122">名称</span><span class="sxs-lookup"><span data-stu-id="7b518-122">Name</span></span>          | <span data-ttu-id="7b518-123">说明</span><span class="sxs-lookup"><span data-stu-id="7b518-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="7b518-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b518-124">Authorization</span></span> | <span data-ttu-id="7b518-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7b518-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b518-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7b518-127">Request body</span></span>
<span data-ttu-id="7b518-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7b518-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b518-129">响应</span><span class="sxs-lookup"><span data-stu-id="7b518-129">Response</span></span>
<span data-ttu-id="7b518-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[onlineMeeting](../resources/onlinemeeting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7b518-130">If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b518-131">示例</span><span class="sxs-lookup"><span data-stu-id="7b518-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7b518-132">请求</span><span class="sxs-lookup"><span data-stu-id="7b518-132">Request</span></span>
<span data-ttu-id="7b518-133">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="7b518-133">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```http
GET https://graph.microsoft.com/beta/app/onlineMeetings/{id}
```

##### <a name="response"></a><span data-ttu-id="7b518-134">响应</span><span class="sxs-lookup"><span data-stu-id="7b518-134">Response</span></span>

> <span data-ttu-id="7b518-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7b518-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7b518-137">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7b518-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7b518-138">C#</span><span class="sxs-lookup"><span data-stu-id="7b518-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-onlineMeeting-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7b518-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="7b518-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-onlineMeeting-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7b518-140">目标-C</span><span class="sxs-lookup"><span data-stu-id="7b518-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-onlineMeeting-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/onlinemeeting-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/onlinemeeting-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/onlinemeeting-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
