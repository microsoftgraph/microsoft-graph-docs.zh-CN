---
title: 创建联机会议
description: 代表请求正文中指定的用户创建联机会议。
author: VinodRavichandran
localization_priority: Priority
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 7a2646ddb1caf4f4e5f4a18823441936f75eb2da
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006415"
---
# <a name="create-online-meeting"></a><span data-ttu-id="52014-103">创建联机会议</span><span class="sxs-lookup"><span data-stu-id="52014-103">Create online meeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52014-104">代表用户使用用户令牌中的对象 ID (oid) 创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="52014-104">Create an online meeting on behalf of a user by using the Object Id (oid) in the user token.</span></span>

> <span data-ttu-id="52014-105">**注意**：会议不会显示在用户的日历上。</span><span class="sxs-lookup"><span data-stu-id="52014-105">**Note**: The meeting does not show on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="52014-106">权限</span><span class="sxs-lookup"><span data-stu-id="52014-106">Permissions</span></span>
<span data-ttu-id="52014-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="52014-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="52014-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="52014-109">Permission type</span></span>                        | <span data-ttu-id="52014-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="52014-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="52014-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52014-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="52014-112">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="52014-112">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="52014-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52014-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52014-114">不支持</span><span class="sxs-lookup"><span data-stu-id="52014-114">Not Supported</span></span>                               |
| <span data-ttu-id="52014-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="52014-115">Application</span></span>                            | <span data-ttu-id="52014-116">OnlineMeetings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52014-116">OnlineMeetings.ReadWrite.All</span></span>                |

## <a name="http-request"></a><span data-ttu-id="52014-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52014-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/onlineMeetings
POST /communications/onlineMeetings
POST /me/onlineMeetings
```
> <span data-ttu-id="52014-118">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="52014-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="52014-119">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="52014-119">Going forward, use the `/communications` path.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52014-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="52014-120">Request headers</span></span>
| <span data-ttu-id="52014-121">名称</span><span class="sxs-lookup"><span data-stu-id="52014-121">Name</span></span>          | <span data-ttu-id="52014-122">说明</span><span class="sxs-lookup"><span data-stu-id="52014-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="52014-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52014-123">Authorization</span></span> | <span data-ttu-id="52014-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="52014-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="52014-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="52014-126">Content-type</span></span>  | <span data-ttu-id="52014-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="52014-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52014-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="52014-129">Request body</span></span>
<span data-ttu-id="52014-130">在请求正文中，提供 [onlineMeeting](../resources/onlinemeeting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52014-130">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="52014-131">响应</span><span class="sxs-lookup"><span data-stu-id="52014-131">Response</span></span>
<span data-ttu-id="52014-132">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="52014-132">If successful, this method returns `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52014-133">示例</span><span class="sxs-lookup"><span data-stu-id="52014-133">Example</span></span>

### <a name="example-1-create-an-online-meeting-with-application-token"></a><span data-ttu-id="52014-134">示例 1：使用应用程序令牌创建联机会议</span><span class="sxs-lookup"><span data-stu-id="52014-134">Example 1: Create an online meeting with application token</span></span>

#### <a name="request"></a><span data-ttu-id="52014-135">请求</span><span class="sxs-lookup"><span data-stu-id="52014-135">Request</span></span>

><span data-ttu-id="52014-136">**注意：** 使用应用程序令牌创建联机会议的过程已弃用。</span><span class="sxs-lookup"><span data-stu-id="52014-136">**Note:** Online meeting creation using the application token is deprecated.</span></span> <span data-ttu-id="52014-137">今后，将 /me 路径与用户令牌结合使用来创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="52014-137">Use the /me path with a user token to create online meetings going forward.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="52014-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="52014-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-app-token"
}-->
```http
POST https://graph.microsoft.com/beta/communications/onlineMeetings
Content-Type: application/json

{
  "isBroadcast": "false",
  "startDateTime":"2019-09-09T14:33:30.8546353-07:00",
  "endDateTime":"2019-09-09T15:03:30.8566356-07:00",
  "subject":"Application Token Meeting",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f"
        }
      }
    }
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="52014-139">C#</span><span class="sxs-lookup"><span data-stu-id="52014-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-app-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52014-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52014-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-app-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="52014-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52014-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-app-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="52014-142">在请求正文中，提供 [onlineMeeting](../resources/onlinemeeting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52014-142">In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="52014-143">响应</span><span class="sxs-lookup"><span data-stu-id="52014-143">Response</span></span>

><span data-ttu-id="52014-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="52014-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "canceledDateTime": null,
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
  "isCanceled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "isBroadcast": false,
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
  "subject": "Application Token Meeting"
}
```

### <a name="example-2-create-an-online-meeting-with-user-token"></a><span data-ttu-id="52014-146">示例 2：使用用户令牌创建联机会议</span><span class="sxs-lookup"><span data-stu-id="52014-146">Example 2: Create an online meeting with user token</span></span>

#### <a name="request"></a><span data-ttu-id="52014-147">请求</span><span class="sxs-lookup"><span data-stu-id="52014-147">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="52014-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="52014-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-user-token"
}-->
```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User Token Meeting"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="52014-149">C#</span><span class="sxs-lookup"><span data-stu-id="52014-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-user-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52014-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="52014-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-user-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="52014-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="52014-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-user-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="52014-152">响应</span><span class="sxs-lookup"><span data-stu-id="52014-152">Response</span></span>
><span data-ttu-id="52014-153">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="52014-153">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f4053f86-17cc-42e7-85f4-f0389ac980d6')/onlineMeetings/$entity",
  "accessLevel": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "canceledDateTime": null,
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "entryExitAnnouncement": true,
  "expirationDateTime": "2019-09-14T18:37:29.1973954Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
  "isCanceled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "isBroadcast": false,
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
  "subject": "User Token Meeting"
}
```

### <a name="example-3-create-an-online-meeting-in-a-microsoft-teams-channel-with-a-user-token"></a><span data-ttu-id="52014-154">示例 3：使用用户令牌在 Microsoft Teams 频道中创建联机会议</span><span class="sxs-lookup"><span data-stu-id="52014-154">Example 3: Create an online meeting in a Microsoft Teams Channel with a user token</span></span>

#### <a name="request"></a><span data-ttu-id="52014-155">请求</span><span class="sxs-lookup"><span data-stu-id="52014-155">Request</span></span>
><span data-ttu-id="52014-156">**注意：** 传递的用户令牌的对象 ID 应当是有效负载中由 threadid 表示的频道的成员。</span><span class="sxs-lookup"><span data-stu-id="52014-156">**Note:** The Object ID of the user token passed should be a member of the channel represented by threadid in the payload.</span></span>

```http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User meeting in Microsoft Teams channel.",
  "chatInfo": {
    "threadId":"19%3A3b52398f3c524556894b776357c1dd79%40thread.skype"
  }
}
```
#### <a name="response"></a><span data-ttu-id="52014-157">响应</span><span class="sxs-lookup"><span data-stu-id="52014-157">Response</span></span>

><span data-ttu-id="52014-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="52014-158">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "example",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('f4053f86-17cc-42e7-85f4-f0389ac980d6')/onlineMeetings/$entity",
  "accessLevel": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "canceledDateTime": null,
  "chatInfo": {
    "threadId": "19%3A3b52398f3c524556894b776357c1dd79%40thread.skype",
    "messageId": "1563302249053",
    "replyChainMessageId": null
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "entryExitAnnouncement": true,
  "expirationDateTime": "2018-03-19T09:46:02Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19%3A3b52398f3c524556894b776357c1dd79%40thread.skype",
  "isCanceled": false,
  "joinUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "isBroadcast": false,
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
  "subject": "User meeting in Microsoft Teams channel."
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