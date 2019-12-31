---
title: 获取 onlineMeeting
description: 检索**联机会议**对象的属性和关系。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: cd2d6abb0131c7193c1504c58eb89e68520cea58
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912306"
---
# <a name="get-onlinemeeting"></a><span data-ttu-id="8cc3c-103">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="8cc3c-103">Get onlineMeeting</span></span>

<span data-ttu-id="8cc3c-104">检索[onlineMeeting](../resources/onlinemeeting.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8cc3c-104">Retrieve the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

> <span data-ttu-id="8cc3c-105">**注意：** 目前`GET`仅[VTC 会议 id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up)支持此方法。这些 Id 是为云-视频互操作许可的用户生成的，此方法用于获取加入会议的详细信息。</span><span class="sxs-lookup"><span data-stu-id="8cc3c-105">**Note:** The `GET` method is currently only supported for a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cc3c-106">权限</span><span class="sxs-lookup"><span data-stu-id="8cc3c-106">Permissions</span></span>

<span data-ttu-id="8cc3c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8cc3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8cc3c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8cc3c-109">Permission type</span></span>                        | <span data-ttu-id="8cc3c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8cc3c-110">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="8cc3c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8cc3c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8cc3c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cc3c-112">Not Supported.</span></span>                                        |
| <span data-ttu-id="8cc3c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8cc3c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cc3c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cc3c-114">Not Supported.</span></span>                                        |
| <span data-ttu-id="8cc3c-115">应用</span><span class="sxs-lookup"><span data-stu-id="8cc3c-115">Application</span></span>                            | <span data-ttu-id="8cc3c-116">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="8cc3c-116">OnlineMeetings.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cc3c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8cc3c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8cc3c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8cc3c-118">Optional query parameters</span></span>
<span data-ttu-id="8cc3c-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8cc3c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8cc3c-120">请求头</span><span class="sxs-lookup"><span data-stu-id="8cc3c-120">Request headers</span></span>
| <span data-ttu-id="8cc3c-121">名称</span><span class="sxs-lookup"><span data-stu-id="8cc3c-121">Name</span></span>          | <span data-ttu-id="8cc3c-122">说明</span><span class="sxs-lookup"><span data-stu-id="8cc3c-122">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="8cc3c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cc3c-123">Authorization</span></span> | <span data-ttu-id="8cc3c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8cc3c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cc3c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8cc3c-126">Request body</span></span>
<span data-ttu-id="8cc3c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8cc3c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8cc3c-128">响应</span><span class="sxs-lookup"><span data-stu-id="8cc3c-128">Response</span></span>
<span data-ttu-id="8cc3c-129">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8cc3c-129">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8cc3c-130">示例</span><span class="sxs-lookup"><span data-stu-id="8cc3c-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8cc3c-131">请求</span><span class="sxs-lookup"><span data-stu-id="8cc3c-131">Request</span></span>
<span data-ttu-id="8cc3c-132">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="8cc3c-132">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8cc3c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cc3c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8cc3c-134">C#</span><span class="sxs-lookup"><span data-stu-id="8cc3c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8cc3c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cc3c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8cc3c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cc3c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8cc3c-137">Java</span><span class="sxs-lookup"><span data-stu-id="8cc3c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-onlinemeeting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8cc3c-138">响应</span><span class="sxs-lookup"><span data-stu-id="8cc3c-138">Response</span></span>

> <span data-ttu-id="8cc3c-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8cc3c-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "autoAdmittedUsers": "everyone",
  "audioConferencing": {
    "tollNumber": "+12525634478",
    "tollFreeNumber": "+18666390588",
    "ConferenceId": "9999999",
    "dialinUrl": "https://dialin.teams.microsoft.com/6787A136-B9B8-4D39-846C-C0F1FF937F10?id=xxxxxxx"
  },
  "chatInfo": {
    "@odata.type": "#microsoft.graph.chatInfo",
    "threadId": "19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
    "messageId": "1533758867081"
  },
  "creationDateTime": "2018-05-30T00:12:19.0726086Z",
  "endDateTime": "2018-05-30T01:00:00Z",
  "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8_19:cbee7c1c860e465f8258e3cebf7bee0d@thread.skype",
  "joinWebUrl": "https://teams.microsoft.com/l/meetup-join/19%3a:meeting_NTg0NmQ3NTctZDVkZC00YzRhLThmNmEtOGQ3M2E0ODdmZDZk@thread.v2/0?context=%7b%22Tid%22%3a%aa67bd4c-8475-432d-bd41-39f255720e0a%22%2c%22Oid%22%3a%22112f7296-5fa4-42ca-bae8-6a692b15d4b8%22%7d",
  "participants": {
  "@odata.type": "#microsoft.graph.meetingParticipants",
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.identitySet",
        "identity": {
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8",
            "displayName": "John"
          }
        },
        "upn": "upn-value"
      }
    ],
    "organizer": {
      "@odata.type": "#microsoft.graph.identitySet",
      "identity": {
        "user": {
          "@odata.type": "#microsoft.graph.identity",
          "id": "5810cede-f3cc-42eb-b2c1-e9bd5d53ec96",
          "displayName": "Bob"
        }
      },
      "upn": "upn-value"
    }
  },
  "startDateTime": "2018-05-30T00:30:00Z",
  "subject": "Test Meeting.",
  "videoTeleconferenceId": "123456789"
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
