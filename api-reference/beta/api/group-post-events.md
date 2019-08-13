---
title: 创建事件
description: 使用此 API 创建新事件。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 1d8a8a6b86abe4f39602885e96d3690fd19d5240
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323274"
---
# <a name="create-event"></a><span data-ttu-id="fa49e-103">创建事件</span><span class="sxs-lookup"><span data-stu-id="fa49e-103">Create event</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa49e-104">使用此 API 新建[事件](../resources/event.md)。</span><span class="sxs-lookup"><span data-stu-id="fa49e-104">Use this API to create a new [event](../resources/event.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fa49e-105">权限</span><span class="sxs-lookup"><span data-stu-id="fa49e-105">Permissions</span></span>
<span data-ttu-id="fa49e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa49e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa49e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa49e-108">Permission type</span></span>      | <span data-ttu-id="fa49e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa49e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa49e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa49e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fa49e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa49e-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="fa49e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa49e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa49e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa49e-113">Not supported.</span></span>    |
|<span data-ttu-id="fa49e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa49e-114">Application</span></span> | <span data-ttu-id="fa49e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa49e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa49e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa49e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/events
POST /groups/{id}/calendar/events
```

## <a name="request-headers"></a><span data-ttu-id="fa49e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa49e-117">Request headers</span></span>
| <span data-ttu-id="fa49e-118">标头</span><span class="sxs-lookup"><span data-stu-id="fa49e-118">Header</span></span>       | <span data-ttu-id="fa49e-119">值</span><span class="sxs-lookup"><span data-stu-id="fa49e-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa49e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa49e-120">Authorization</span></span>  | <span data-ttu-id="fa49e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa49e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa49e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa49e-123">Request body</span></span>
<span data-ttu-id="fa49e-124">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa49e-124">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fa49e-125">响应</span><span class="sxs-lookup"><span data-stu-id="fa49e-125">Response</span></span>
<span data-ttu-id="fa49e-126">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fa49e-126">If successful, this method returns `201 Created` response code and [event](../resources/event.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa49e-127">示例</span><span class="sxs-lookup"><span data-stu-id="fa49e-127">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fa49e-128">请求</span><span class="sxs-lookup"><span data-stu-id="fa49e-128">Request</span></span>
<span data-ttu-id="fa49e-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fa49e-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fa49e-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fa49e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["01d4ee64-15ce-491e-bad1-b91aa3223df4"],
  "name": "create_event_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/events
Content-type: application/json

{
  "subject": "Let's go for lunch",
  "body": {
    "contentType": "HTML",
    "content": "Does late morning work for you?"
  },
  "start": {
      "dateTime": "2019-06-15T12:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2019-06-15T14:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "location":{
      "displayName":"Harry's Bar"
  },
  "attendees": [
    {
      "emailAddress": {
        "address":"adelev@contoso.onmicrosoft.com",
        "name": "Adele Vance"
      },
      "type": "required"
    }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa49e-131">C#</span><span class="sxs-lookup"><span data-stu-id="fa49e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-event-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa49e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa49e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-event-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa49e-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="fa49e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-event-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fa49e-134">Java</span><span class="sxs-lookup"><span data-stu-id="fa49e-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-event-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fa49e-135">在请求正文中，提供 [event](../resources/event.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa49e-135">In the request body, supply a JSON representation of [event](../resources/event.md) object.</span></span>

#### <a name="response"></a><span data-ttu-id="fa49e-136">响应</span><span class="sxs-lookup"><span data-stu-id="fa49e-136">Response</span></span>
<span data-ttu-id="fa49e-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fa49e-137">The following is an example of the response.</span></span>
><span data-ttu-id="fa49e-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fa49e-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="fa49e-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fa49e-139">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('01d4ee64-15ce-491e-bad1-b91aa3223df4')/events/$entity",
    "@odata.etag": "W/\"Na8DfbsBGUG8JeyvlwNi5wAAHMK0mg==\"",
    "id": "AAMkADZ_XA2LnAAAcwiSBAAA=",
    "createdDateTime": "2019-05-20T02:14:32.7419058Z",
    "lastModifiedDateTime": "2019-05-20T02:14:33.342409Z",
    "changeKey": "Na8DfbsBGUG8JeyvlwNi5wAAHMK0mg==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "uid": "040000008200E00074C5B7101A82E00800000000DE7664C3B10ED501000000000000000010000000EC2760BC8BC4AF4BAC1C9730C3E534AC",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Let's go for lunch",
    "bodyPreview": "Does late morning work for you?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADZ%2BXA2LnAAAcwiSBAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\nDoes late morning work for you?\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-06-15T12:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "end": {
        "dateTime": "2019-06-15T14:00:00.0000000",
        "timeZone": "Pacific Standard Time"
    },
    "location": {
        "displayName": "Harry's Bar",
        "locationType": "default",
        "uniqueId": "Harry's Bar",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Harry's Bar",
            "locationType": "default",
            "uniqueId": "Harry's Bar",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Adele Vance",
                "address": "adelev@contoso.onmicrosoft.com"
            }
        }
    ],
    "organizer": {
        "emailAddress": {
            "name": "Retail",
            "address": "Retail@contoso.onmicrosoft.com"
        }
    }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
