---
title: 创建联机会议
description: 代表请求正文中指定的用户创建联机会议。
author: VinodRavichandran
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: e487025cbf9dd5e4a91ad4962f218e25adc7118b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856928"
---
# <a name="create-online-meeting"></a><span data-ttu-id="68d6d-103">创建联机会议</span><span class="sxs-lookup"><span data-stu-id="68d6d-103">Create online meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68d6d-104">代表请求正文中指定的用户创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="68d6d-104">Creates an online meeting on behalf of a user specified in the request body.</span></span>

> <span data-ttu-id="68d6d-105">**注释**：会议不会显示在用户的日历上。</span><span class="sxs-lookup"><span data-stu-id="68d6d-105">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="68d6d-106">权限</span><span class="sxs-lookup"><span data-stu-id="68d6d-106">Permissions</span></span>
<span data-ttu-id="68d6d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68d6d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68d6d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="68d6d-109">Permission type</span></span>                        | <span data-ttu-id="68d6d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68d6d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="68d6d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68d6d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="68d6d-112">不支持</span><span class="sxs-lookup"><span data-stu-id="68d6d-112">Not Supported</span></span>                               |
| <span data-ttu-id="68d6d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68d6d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68d6d-114">不支持</span><span class="sxs-lookup"><span data-stu-id="68d6d-114">Not Supported</span></span>                               |
| <span data-ttu-id="68d6d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="68d6d-115">Application</span></span>                            | <span data-ttu-id="68d6d-116">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68d6d-116">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="68d6d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68d6d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /applications/{id}/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="68d6d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="68d6d-118">Request headers</span></span>
| <span data-ttu-id="68d6d-119">名称</span><span class="sxs-lookup"><span data-stu-id="68d6d-119">Name</span></span>          | <span data-ttu-id="68d6d-120">说明</span><span class="sxs-lookup"><span data-stu-id="68d6d-120">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="68d6d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="68d6d-121">Authorization</span></span> | <span data-ttu-id="68d6d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68d6d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68d6d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="68d6d-124">Request body</span></span>
<span data-ttu-id="68d6d-125">在请求正文中，提供 [onlineMeeting](../resources/onlinemeeting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68d6d-125">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="68d6d-126">响应</span><span class="sxs-lookup"><span data-stu-id="68d6d-126">Response</span></span>
<span data-ttu-id="68d6d-127">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="68d6d-127">If successful, this method returns `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68d6d-128">示例</span><span class="sxs-lookup"><span data-stu-id="68d6d-128">Example</span></span>

##### <a name="request"></a><span data-ttu-id="68d6d-129">请求</span><span class="sxs-lookup"><span data-stu-id="68d6d-129">Request</span></span>
<span data-ttu-id="68d6d-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="68d6d-130">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="68d6d-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="68d6d-131">--Http</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="68d6d-132">C#</span><span class="sxs-lookup"><span data-stu-id="68d6d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68d6d-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="68d6d-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68d6d-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68d6d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="68d6d-135">Java</span><span class="sxs-lookup"><span data-stu-id="68d6d-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-onlinemeeting-from-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="68d6d-136">在请求正文中，提供 [onlineMeeting](../resources/onlinemeeting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68d6d-136">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="68d6d-137">响应</span><span class="sxs-lookup"><span data-stu-id="68d6d-137">Response</span></span>

><span data-ttu-id="68d6d-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="68d6d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  ]
}
-->
