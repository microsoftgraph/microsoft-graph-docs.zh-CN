---
title: 获取 onlineMeeting
description: 检索**联机会议**对象的属性和关系。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 42906632b4a8161966a04473fe7492049484d620
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869400"
---
# <a name="get-onlinemeeting"></a><span data-ttu-id="281e0-103">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="281e0-103">Get onlineMeeting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="281e0-104">检索[onlineMeeting](../resources/onlinemeeting.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="281e0-104">Retrieve the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

> <span data-ttu-id="281e0-105">**注意：** 目前`GET`仅[VTC 会议 id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up)支持此方法。这些 Id 是为云-视频互操作许可的用户生成的，此方法用于获取加入会议的详细信息。</span><span class="sxs-lookup"><span data-stu-id="281e0-105">**Note:** The `GET` method is currently only supported for a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="281e0-106">权限</span><span class="sxs-lookup"><span data-stu-id="281e0-106">Permissions</span></span>

<span data-ttu-id="281e0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="281e0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="281e0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="281e0-109">Permission type</span></span>                        | <span data-ttu-id="281e0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="281e0-110">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="281e0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="281e0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="281e0-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="281e0-112">Not Supported.</span></span>                                        |
| <span data-ttu-id="281e0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="281e0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="281e0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="281e0-114">Not Supported.</span></span>                                        |
| <span data-ttu-id="281e0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="281e0-115">Application</span></span>                            | <span data-ttu-id="281e0-116">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="281e0-116">OnlineMeetings.Read.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="281e0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="281e0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
```
> <span data-ttu-id="281e0-118">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="281e0-118">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="281e0-119">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="281e0-119">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="281e0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="281e0-120">Optional query parameters</span></span>
<span data-ttu-id="281e0-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="281e0-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="281e0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="281e0-122">Request headers</span></span>
| <span data-ttu-id="281e0-123">名称</span><span class="sxs-lookup"><span data-stu-id="281e0-123">Name</span></span>          | <span data-ttu-id="281e0-124">说明</span><span class="sxs-lookup"><span data-stu-id="281e0-124">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="281e0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="281e0-125">Authorization</span></span> | <span data-ttu-id="281e0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="281e0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="281e0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="281e0-128">Request body</span></span>
<span data-ttu-id="281e0-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="281e0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="281e0-130">响应</span><span class="sxs-lookup"><span data-stu-id="281e0-130">Response</span></span>
<span data-ttu-id="281e0-131">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="281e0-131">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="281e0-132">示例</span><span class="sxs-lookup"><span data-stu-id="281e0-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="281e0-133">请求</span><span class="sxs-lookup"><span data-stu-id="281e0-133">Request</span></span>
<span data-ttu-id="281e0-134">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="281e0-134">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="281e0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="281e0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="281e0-136">C#</span><span class="sxs-lookup"><span data-stu-id="281e0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="281e0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="281e0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="281e0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="281e0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="281e0-139">响应</span><span class="sxs-lookup"><span data-stu-id="281e0-139">Response</span></span>

> <span data-ttu-id="281e0-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="281e0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "attendees": [
      {
        "@odata.type": "#microsoft.graph.identitySet",
        "identity": {
          "user": {
            "@odata.type": "#microsoft.graph.identity",
            "id": "112f7296-5fa4-42ca-bae8-6a692b15d4b8",
            "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
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
          "tenantId": "aa67bd4c-8475-432d-bd41-39f255720e0a",
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
