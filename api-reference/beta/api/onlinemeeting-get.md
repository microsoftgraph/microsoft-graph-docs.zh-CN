---
title: 获取 onlineMeeting
description: 检索**联机会议**对象的属性和关系。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 58c995a9ca6be7029b1a5510023160c97cadb735
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456502"
---
# <a name="get-onlinemeeting"></a><span data-ttu-id="5501a-103">获取 onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="5501a-103">Get onlineMeeting</span></span>

<span data-ttu-id="5501a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5501a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5501a-105">检索[onlineMeeting](../resources/onlinemeeting.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5501a-105">Retrieve the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.</span></span>

> <span data-ttu-id="5501a-106">**注意：** 目前`GET`仅[VTC 会议 id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up)支持此方法。这些 Id 是为云-视频互操作许可的用户生成的，此方法用于获取加入会议的详细信息。</span><span class="sxs-lookup"><span data-stu-id="5501a-106">**Note:** The `GET` method is currently only supported for a [VTC conference id](https://docs.microsoft.com/microsoftteams/cloud-video-interop-for-teams-set-up). These IDs are generated for Cloud-Video-Interop licensed users and this method is used to get the details to join the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="5501a-107">权限</span><span class="sxs-lookup"><span data-stu-id="5501a-107">Permissions</span></span>

<span data-ttu-id="5501a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5501a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5501a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5501a-110">Permission type</span></span>                        | <span data-ttu-id="5501a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5501a-111">Permissions (from least to most privileged)</span></span>           |
|:---------------------------------------|:------------------------------------------------------|
| <span data-ttu-id="5501a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5501a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5501a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5501a-113">Not Supported.</span></span>                                        |
| <span data-ttu-id="5501a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5501a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5501a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5501a-115">Not Supported.</span></span>                                        |
| <span data-ttu-id="5501a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5501a-116">Application</span></span>                            | <span data-ttu-id="5501a-117">OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="5501a-117">OnlineMeetings.Read.All</span></span>                               |

## <a name="http-request"></a><span data-ttu-id="5501a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5501a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
GET /communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'{id}'
```
> <span data-ttu-id="5501a-119">**注意：**`/app` 路径已弃用。</span><span class="sxs-lookup"><span data-stu-id="5501a-119">**Note:** The `/app` path is deprecated.</span></span> <span data-ttu-id="5501a-120">今后将使用 `/communications` 路径。</span><span class="sxs-lookup"><span data-stu-id="5501a-120">Going forward, use the `/communications` path.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="5501a-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5501a-121">Optional query parameters</span></span>
<span data-ttu-id="5501a-122">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5501a-122">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5501a-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="5501a-123">Request headers</span></span>
| <span data-ttu-id="5501a-124">名称</span><span class="sxs-lookup"><span data-stu-id="5501a-124">Name</span></span>          | <span data-ttu-id="5501a-125">说明</span><span class="sxs-lookup"><span data-stu-id="5501a-125">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="5501a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="5501a-126">Authorization</span></span> | <span data-ttu-id="5501a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5501a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5501a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="5501a-129">Request body</span></span>
<span data-ttu-id="5501a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5501a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5501a-131">响应</span><span class="sxs-lookup"><span data-stu-id="5501a-131">Response</span></span>
<span data-ttu-id="5501a-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [onlineMeeting](../resources/onlinemeeting.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5501a-132">If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5501a-133">示例</span><span class="sxs-lookup"><span data-stu-id="5501a-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5501a-134">请求</span><span class="sxs-lookup"><span data-stu-id="5501a-134">Request</span></span>
<span data-ttu-id="5501a-135">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="5501a-135">The following example shows the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="5501a-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5501a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get-onlineMeeting"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/communications/onlineMeetings/?$filter=VideoTeleconferenceId%20eq%20'123456789'
```
# <a name="c"></a>[<span data-ttu-id="5501a-137">C#</span><span class="sxs-lookup"><span data-stu-id="5501a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-onlinemeeting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5501a-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5501a-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-onlinemeeting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5501a-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5501a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-onlinemeeting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5501a-140">响应</span><span class="sxs-lookup"><span data-stu-id="5501a-140">Response</span></span>

> <span data-ttu-id="5501a-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5501a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
