---
title: 创建 onlineMeeting
description: 代表请求正文中指定的用户创建联机会议。
author: ananmishr
localization_priority: Priority
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: c13140c6afa175e47d68e4e744526fda8e7e70c1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42518866"
---
# <a name="create-onlinemeeting"></a><span data-ttu-id="85382-103">创建 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="85382-103">Create onlineMeeting</span></span>

<span data-ttu-id="85382-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85382-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85382-105">代表用户使用用户令牌中的对象 ID (OID) 创建联机会议。</span><span class="sxs-lookup"><span data-stu-id="85382-105">Create an online meeting on behalf of a user by using the object ID (OID) in the user token.</span></span>

> <span data-ttu-id="85382-106">**注意**：会议不会显示在用户的日历上。</span><span class="sxs-lookup"><span data-stu-id="85382-106">**Note**: The meeting does not show up on the user's calendar.</span></span>

## <a name="permissions"></a><span data-ttu-id="85382-107">权限</span><span class="sxs-lookup"><span data-stu-id="85382-107">Permissions</span></span>
<span data-ttu-id="85382-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85382-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85382-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="85382-110">Permission type</span></span>                        | <span data-ttu-id="85382-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85382-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="85382-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85382-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="85382-113">OnlineMeetings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="85382-113">OnlineMeetings.ReadWrite</span></span>                    |
| <span data-ttu-id="85382-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85382-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85382-115">不支持</span><span class="sxs-lookup"><span data-stu-id="85382-115">Not Supported</span></span>                               |
| <span data-ttu-id="85382-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="85382-116">Application</span></span>                            | <span data-ttu-id="85382-117">不支持</span><span class="sxs-lookup"><span data-stu-id="85382-117">Not Supported</span></span>                |

## <a name="http-request"></a><span data-ttu-id="85382-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85382-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/onlineMeetings
```

## <a name="request-headers"></a><span data-ttu-id="85382-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="85382-119">Request headers</span></span>
| <span data-ttu-id="85382-120">名称</span><span class="sxs-lookup"><span data-stu-id="85382-120">Name</span></span>          | <span data-ttu-id="85382-121">说明</span><span class="sxs-lookup"><span data-stu-id="85382-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="85382-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85382-122">Authorization</span></span> | <span data-ttu-id="85382-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="85382-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="85382-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="85382-125">Content-type</span></span>  | <span data-ttu-id="85382-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="85382-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85382-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="85382-128">Request body</span></span>
<span data-ttu-id="85382-129">在请求正文中，提供 [onlineMeeting](../resources/onlinemeeting.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85382-129">In the request body, supply a JSON representation of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="85382-130">响应</span><span class="sxs-lookup"><span data-stu-id="85382-130">Response</span></span>
<span data-ttu-id="85382-131">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85382-131">If successful, this method returns a `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85382-132">示例</span><span class="sxs-lookup"><span data-stu-id="85382-132">Examples</span></span> 

<span data-ttu-id="85382-133">以下示例会使用用户令牌创建一个联机会议。</span><span class="sxs-lookup"><span data-stu-id="85382-133">The following example creates an online meeting with a user token.</span></span>

### <a name="request"></a><span data-ttu-id="85382-134">请求</span><span class="sxs-lookup"><span data-stu-id="85382-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="85382-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="85382-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-onlinemeeting-user-token"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/onlineMeetings
Content-Type: application/json

{
  "startDateTime":"2019-07-12T14:30:34.2444915-07:00",
  "endDateTime":"2019-07-12T15:00:34.2464912-07:00",
  "subject":"User Token Meeting"
}
```
# <a name="c"></a>[<span data-ttu-id="85382-136">C#</span><span class="sxs-lookup"><span data-stu-id="85382-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-onlinemeeting-user-token-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85382-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85382-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onlinemeeting-user-token-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85382-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85382-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onlinemeeting-user-token-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85382-139">Java</span><span class="sxs-lookup"><span data-stu-id="85382-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-onlinemeeting-user-token-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="85382-140">响应</span><span class="sxs-lookup"><span data-stu-id="85382-140">Response</span></span>
><span data-ttu-id="85382-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="85382-141">**Note:** The response object shown here might be shortened for readability.</span></span> 

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f4053f86-17cc-42e7-85f4-f0389ac980d6')/onlineMeetings/$entity",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "2425999",
    "dialinUrl": "https://dialin.teams.microsoft.com/22f12fa0-499f-435b-bc69-b8de580ba330?id=2425999"
  },
  "chatInfo": {
    "threadId": "19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
    "messageId": "0",
    "replyChainMessageId": "0"
  },
  "creationDateTime": "2019-07-11T02:17:17.6491364Z",
  "startDateTime": "2019-07-11T02:17:17.6491364Z",
  "endDateTime": "2019-07-11T02:47:17.651138Z",
  "id": "550fae72-d251-43ec-868c-373732c2704f_19:meeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3ameeting_M2IzYzczNTItYmY3OC00MDlmLWJjMzUtYmFiMjNlOTY4MGEz%40thread.skype/0?context=%7b%22Tid%22%3a%2272f988bf-86f1-41af-91ab-2d7cd011db47%22%2c%22Oid%22%3a%22550fae72-d251-43ec-868c-373732c2704f%22%7d",
  "participants": {
    "organizer": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "displayName": "Heidi Steen"
        }
      },
      "upn": "upn-value"
    }
  },
  "subject": "User Token Meeting"
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
