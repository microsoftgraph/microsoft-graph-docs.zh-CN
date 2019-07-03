---
title: 获取联机会议
description: 检索**onlineMeeting**对象的属性和关系。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e762035192bb3387f916e2bd7cf1772478952808
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450252"
---
# <a name="get-online-meeting"></a><span data-ttu-id="1b5de-103">获取联机会议</span><span class="sxs-lookup"><span data-stu-id="1b5de-103">Get Online Meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b5de-104">检索**onlineMeeting**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b5de-104">Retrieve the properties and relationships of an **onlineMeeting** object.</span></span>

> <span data-ttu-id="1b5de-105">**注意:** 此`GET`方法限制为[VTC 会议 id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up)。这些 Id 是为云-视频互操作许可的用户生成的, 此方法用于获取加入会议的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1b5de-105">**Note:** The `GET` method is limited to a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>
> <span data-ttu-id="1b5de-106">对于常规流, bot 可以使用`joinURL`加入会议, 而无需进行查找。</span><span class="sxs-lookup"><span data-stu-id="1b5de-106">For regular flows, the bot can use the `joinURL` to join a meeting and no lookup is necessary.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b5de-107">权限</span><span class="sxs-lookup"><span data-stu-id="1b5de-107">Permissions</span></span>

<span data-ttu-id="1b5de-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b5de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1b5de-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b5de-110">Permission type</span></span>                        | <span data-ttu-id="1b5de-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b5de-111">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="1b5de-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b5de-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1b5de-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b5de-113">Not Supported.</span></span>                                        |
| <span data-ttu-id="1b5de-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b5de-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b5de-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b5de-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="1b5de-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b5de-116">Application</span></span>                            | <span data-ttu-id="1b5de-117">OnlineMeetings、OnlineMeetings 和所有</span><span class="sxs-lookup"><span data-stu-id="1b5de-117">OnlineMeetings.Read.All, OnlineMeetings.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b5de-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b5de-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/{id}
GET /applications/{id}/onlineMeetings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1b5de-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1b5de-119">Optional query parameters</span></span>
<span data-ttu-id="1b5de-120">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1b5de-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1b5de-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b5de-121">Request headers</span></span>
| <span data-ttu-id="1b5de-122">名称</span><span class="sxs-lookup"><span data-stu-id="1b5de-122">Name</span></span>          | <span data-ttu-id="1b5de-123">说明</span><span class="sxs-lookup"><span data-stu-id="1b5de-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="1b5de-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b5de-124">Authorization</span></span> | <span data-ttu-id="1b5de-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b5de-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b5de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b5de-127">Request body</span></span>
<span data-ttu-id="1b5de-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1b5de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1b5de-129">响应</span><span class="sxs-lookup"><span data-stu-id="1b5de-129">Response</span></span>
<span data-ttu-id="1b5de-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[onlineMeeting](../resources/onlinemeeting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1b5de-130">If successful, this method returns a `200 OK` response code and [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b5de-131">示例</span><span class="sxs-lookup"><span data-stu-id="1b5de-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1b5de-132">请求</span><span class="sxs-lookup"><span data-stu-id="1b5de-132">Request</span></span>
<span data-ttu-id="1b5de-133">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="1b5de-133">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="1b5de-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="1b5de-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```http
GET https://graph.microsoft.com/beta/app/onlineMeetings/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="1b5de-135">C#</span><span class="sxs-lookup"><span data-stu-id="1b5de-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b5de-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="1b5de-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="1b5de-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="1b5de-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="1b5de-138">响应</span><span class="sxs-lookup"><span data-stu-id="1b5de-138">Response</span></span>

> <span data-ttu-id="1b5de-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1b5de-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
