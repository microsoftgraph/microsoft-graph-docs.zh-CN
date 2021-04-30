---
title: 更新事件
description: 更新 event 对象。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: ec162826d35b21c858eb69c17c97ee0d8b39f8a3
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080524"
---
# <a name="update-event"></a><span data-ttu-id="4e0b4-103">更新事件</span><span class="sxs-lookup"><span data-stu-id="4e0b4-103">Update event</span></span>

<span data-ttu-id="4e0b4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e0b4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4e0b4-105">更新 [event](../resources/event.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4e0b4-105">Update an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e0b4-106">权限</span><span class="sxs-lookup"><span data-stu-id="4e0b4-106">Permissions</span></span>
<span data-ttu-id="4e0b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e0b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e0b4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e0b4-109">Permission type</span></span>      | <span data-ttu-id="4e0b4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e0b4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e0b4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e0b4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4e0b4-112">Calendars.ReadWrite、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e0b4-112">Calendars.ReadWrite, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e0b4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e0b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e0b4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e0b4-114">Not supported.</span></span>    |
|<span data-ttu-id="4e0b4-115">Application</span><span class="sxs-lookup"><span data-stu-id="4e0b4-115">Application</span></span> | <span data-ttu-id="4e0b4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e0b4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e0b4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e0b4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/events/{id}
PATCH /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4e0b4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e0b4-118">Request headers</span></span>
| <span data-ttu-id="4e0b4-119">名称</span><span class="sxs-lookup"><span data-stu-id="4e0b4-119">Name</span></span>       | <span data-ttu-id="4e0b4-120">类型</span><span class="sxs-lookup"><span data-stu-id="4e0b4-120">Type</span></span> | <span data-ttu-id="4e0b4-121">说明</span><span class="sxs-lookup"><span data-stu-id="4e0b4-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4e0b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e0b4-122">Authorization</span></span>  | <span data-ttu-id="4e0b4-123">string</span><span class="sxs-lookup"><span data-stu-id="4e0b4-123">string</span></span>  | <span data-ttu-id="4e0b4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e0b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e0b4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e0b4-126">Request body</span></span>
<span data-ttu-id="4e0b4-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4e0b4-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="4e0b4-130">响应</span><span class="sxs-lookup"><span data-stu-id="4e0b4-130">Response</span></span>
<span data-ttu-id="4e0b4-131">如果成功，此方法返回 `200 OK` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4e0b4-131">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4e0b4-132">示例</span><span class="sxs-lookup"><span data-stu-id="4e0b4-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4e0b4-133">请求</span><span class="sxs-lookup"><span data-stu-id="4e0b4-133">Request</span></span>
<span data-ttu-id="4e0b4-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4e0b4-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="4e0b4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e0b4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["01d4ee64-15ce-491e-bad1-b91aa3223df4", "AAMkADZlAAAAABERAAA="],
  "name": "update_group_event"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/calendar/events/AAMkADZlAAAAABERAAA=
Content-type: application/json

{ 
  "location":{
      "displayName":"Conf Room 2"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="4e0b4-136">C#</span><span class="sxs-lookup"><span data-stu-id="4e0b4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-group-event-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e0b4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e0b4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-group-event-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e0b4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e0b4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-group-event-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e0b4-139">Java</span><span class="sxs-lookup"><span data-stu-id="4e0b4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-group-event-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="4e0b4-140">响应</span><span class="sxs-lookup"><span data-stu-id="4e0b4-140">Response</span></span>
<span data-ttu-id="4e0b4-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4e0b4-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.event",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups('01d4ee64-15ce-491e-bad1-b91aa3223df4')/calendar/events/$entity",
    "@odata.etag": "W/\"Na8DfbsBGUG8JeyvlwNi5wAAHMKyZg==\"",
    "id": "AAMkADZlAAAAABERAAA=",
    "createdDateTime": "2019-04-06T13:19:09.2517612Z",
    "lastModifiedDateTime": "2019-05-20T00:14:51.2677891Z",
    "changeKey": "Na8DfbsBGUG8JeyvlwNi5wAAHMKyZg==",
    "categories": [],
    "originalStartTimeZone": "Pacific Standard Time",
    "originalEndTimeZone": "Pacific Standard Time",
    "iCalUId": "040000008200E00074C5B7101A82E00800000000B7CA7D517BECD40100000000000000001000000011E38F935AD4FF41BDAB12A2F3E15103",
    "reminderMinutesBeforeStart": 15,
    "isReminderOn": true,
    "hasAttachments": false,
    "subject": "Planogram Training",
    "bodyPreview": "Need more help with visual merchandising?",
    "importance": "normal",
    "sensitivity": "normal",
    "isAllDay": false,
    "isCancelled": false,
    "isOrganizer": true,
    "responseRequested": true,
    "seriesMasterId": null,
    "showAs": "busy",
    "type": "singleInstance",
    "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADZlAAAAABERAAA%3D&exvsurl=1&path=/calendar/item",
    "onlineMeetingUrl": null,
    "recurrence": null,
    "responseStatus": {
        "response": "organizer",
        "time": "0001-01-01T00:00:00Z"
    },
    "body": {
        "contentType": "html",
        "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n<meta content=\"text/html; charset=us-ascii\">\r\n</head>\r\n<body>\r\n<div>Need more help with visual merchandising?\r\n</div>\r\n</body>\r\n</html>\r\n"
    },
    "start": {
        "dateTime": "2019-04-16T22:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2019-04-16T23:00:00.0000000",
        "timeZone": "UTC"
    },
    "location": {
        "displayName": "Conf Room 2",
        "locationType": "default",
        "uniqueId": "Conf Room 2",
        "uniqueIdType": "private"
    },
    "locations": [
        {
            "displayName": "Conf Room 2",
            "locationType": "default",
            "uniqueId": "Conf Room 2",
            "uniqueIdType": "private"
        }
    ],
    "attendees": [
        {
            "type": "required",
            "status": {
                "response": "accepted",
                "time": "2019-04-06T13:19:12.1060982Z"
            },
            "emailAddress": {
                "name": "Johanna Lorenz",
                "address": "JohannaL@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Retail",
                "address": "Retail@contoso.onmicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Alex Wilber",
                "address": "AlexW@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Megan Bowen",
                "address": "MeganB@contoso.OnMicrosoft.com"
            }
        },
        {
            "type": "required",
            "status": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "emailAddress": {
                "name": "Nestor Wilke",
                "address": "NestorW@contoso.OnMicrosoft.com"
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
<!-- {
  "type": "#page.annotation",
  "description": "Update event",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

