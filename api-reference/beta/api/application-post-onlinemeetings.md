---
title: 创建联机会议
description: 创建一个代表指定在请求正文中的用户的联机会议。
author: lleonard-msft
ms.openlocfilehash: 4a68e25156353b41c3ff43685d7b021a2454a927
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331428"
---
# <a name="create-online-meeting"></a><span data-ttu-id="6ef40-103">创建联机会议</span><span class="sxs-lookup"><span data-stu-id="6ef40-103">Create online meeting</span></span>

> <span data-ttu-id="6ef40-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6ef40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ef40-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6ef40-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ef40-106">创建一个代表指定在请求正文中的用户的联机会议。</span><span class="sxs-lookup"><span data-stu-id="6ef40-106">Creates an online meeting on behalf of a user specified in the request body.</span></span>

> <span data-ttu-id="6ef40-107">**注意**： 会议不会显示在用户的日历。</span><span class="sxs-lookup"><span data-stu-id="6ef40-107">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ef40-108">权限</span><span class="sxs-lookup"><span data-stu-id="6ef40-108">Permissions</span></span>
<span data-ttu-id="6ef40-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ef40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6ef40-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ef40-111">Permission type</span></span>                        | <span data-ttu-id="6ef40-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ef40-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6ef40-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ef40-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6ef40-114">不支持</span><span class="sxs-lookup"><span data-stu-id="6ef40-114">Not Supported</span></span>                               |
| <span data-ttu-id="6ef40-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ef40-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ef40-116">不支持</span><span class="sxs-lookup"><span data-stu-id="6ef40-116">Not Supported</span></span>                               |
| <span data-ttu-id="6ef40-117">Application</span><span class="sxs-lookup"><span data-stu-id="6ef40-117">Application</span></span>                            | <span data-ttu-id="6ef40-118">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ef40-118">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="6ef40-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ef40-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /applications/{id}/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="6ef40-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ef40-120">Request headers</span></span>
| <span data-ttu-id="6ef40-121">Name</span><span class="sxs-lookup"><span data-stu-id="6ef40-121">Name</span></span>          | <span data-ttu-id="6ef40-122">说明</span><span class="sxs-lookup"><span data-stu-id="6ef40-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="6ef40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ef40-123">Authorization</span></span> | <span data-ttu-id="6ef40-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ef40-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ef40-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ef40-126">Request body</span></span>
<span data-ttu-id="6ef40-127">在请求正文中，提供[onlineMeeting](../resources/onlinemeeting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ef40-127">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6ef40-128">响应</span><span class="sxs-lookup"><span data-stu-id="6ef40-128">Response</span></span>
<span data-ttu-id="6ef40-129">如果成功，此方法返回`201 Created`响应代码和响应正文中的[onlineMeeting](../resources/onlinemeeting.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6ef40-129">If successful, this method returns `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ef40-130">示例</span><span class="sxs-lookup"><span data-stu-id="6ef40-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6ef40-131">请求</span><span class="sxs-lookup"><span data-stu-id="6ef40-131">Request</span></span>
<span data-ttu-id="6ef40-132">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ef40-132">The following example shows the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_onlineMeeting_from_application"
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

<span data-ttu-id="6ef40-133">在请求正文中，提供[onlineMeeting](../resources/onlinemeeting.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ef40-133">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="6ef40-134">响应</span><span class="sxs-lookup"><span data-stu-id="6ef40-134">Response</span></span>

><span data-ttu-id="6ef40-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6ef40-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create onlineMeeting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
