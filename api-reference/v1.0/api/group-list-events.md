---
title: 列出事件
description: 检索事件对象列表。
author: dkershaw10
localization_priority: Priority
ms.prod: groups
ms.openlocfilehash: 3538eb955f20d453eaf1bd7f2c77a07a932c62de
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583534"
---
# <a name="list-events"></a><span data-ttu-id="429cd-103">列出事件</span><span class="sxs-lookup"><span data-stu-id="429cd-103">List events</span></span>
<span data-ttu-id="429cd-104">检索 [event](../resources/event.md) 对象列表.</span><span class="sxs-lookup"><span data-stu-id="429cd-104">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="429cd-105">权限</span><span class="sxs-lookup"><span data-stu-id="429cd-105">Permissions</span></span>
<span data-ttu-id="429cd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="429cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="429cd-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="429cd-108">Permission type</span></span>      | <span data-ttu-id="429cd-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="429cd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="429cd-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="429cd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="429cd-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="429cd-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="429cd-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="429cd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="429cd-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="429cd-113">Not supported.</span></span>    |
|<span data-ttu-id="429cd-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="429cd-114">Application</span></span> | <span data-ttu-id="429cd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="429cd-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="429cd-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="429cd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="429cd-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="429cd-117">Optional query parameters</span></span>
<span data-ttu-id="429cd-118">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="429cd-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="429cd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="429cd-119">Request headers</span></span>
| <span data-ttu-id="429cd-120">名称</span><span class="sxs-lookup"><span data-stu-id="429cd-120">Name</span></span>       | <span data-ttu-id="429cd-121">类型</span><span class="sxs-lookup"><span data-stu-id="429cd-121">Type</span></span> | <span data-ttu-id="429cd-122">说明</span><span class="sxs-lookup"><span data-stu-id="429cd-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="429cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="429cd-123">Authorization</span></span>  | <span data-ttu-id="429cd-124">string</span><span class="sxs-lookup"><span data-stu-id="429cd-124">string</span></span> | <span data-ttu-id="429cd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="429cd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="429cd-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="429cd-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="429cd-128">string</span><span class="sxs-lookup"><span data-stu-id="429cd-128">string</span></span> | <span data-ttu-id="429cd-129">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="429cd-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="429cd-130">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="429cd-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="429cd-131">可选。</span><span class="sxs-lookup"><span data-stu-id="429cd-131">Optional.</span></span> |
| <span data-ttu-id="429cd-132">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="429cd-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="429cd-133">string</span><span class="sxs-lookup"><span data-stu-id="429cd-133">string</span></span> | <span data-ttu-id="429cd-134">要返回的 **body** 属性的格式。</span><span class="sxs-lookup"><span data-stu-id="429cd-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="429cd-135">可取值为“text”或“html”。</span><span class="sxs-lookup"><span data-stu-id="429cd-135">Values can be "text" or "html".</span></span> <span data-ttu-id="429cd-136">如果指定此 `Preference-Applied` 头，返回 `Prefer` 头作为证明。</span><span class="sxs-lookup"><span data-stu-id="429cd-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="429cd-137">如果未指定此头，采用 HTML 格式返回 **body** 属性。</span><span class="sxs-lookup"><span data-stu-id="429cd-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="429cd-138">可选。</span><span class="sxs-lookup"><span data-stu-id="429cd-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="429cd-139">请求正文</span><span class="sxs-lookup"><span data-stu-id="429cd-139">Request body</span></span>
<span data-ttu-id="429cd-140">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="429cd-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="429cd-141">响应</span><span class="sxs-lookup"><span data-stu-id="429cd-141">Response</span></span>
<span data-ttu-id="429cd-142">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="429cd-142">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="429cd-143">示例</span><span class="sxs-lookup"><span data-stu-id="429cd-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="429cd-144">请求</span><span class="sxs-lookup"><span data-stu-id="429cd-144">Request</span></span>
<span data-ttu-id="429cd-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="429cd-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["02bd9fd6-8f93-4758-87c3-1fb73740a315"],
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events
```

#### <a name="response"></a><span data-ttu-id="429cd-146">响应</span><span class="sxs-lookup"><span data-stu-id="429cd-146">Response</span></span>
<span data-ttu-id="429cd-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="429cd-147">The following is an example of the response.</span></span>
><span data-ttu-id="429cd-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="429cd-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "id": "AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA==",
      "createdDateTime": "2017-07-31T18:59:01.982289Z",
      "lastModifiedDateTime": "2017-09-06T04:29:38.6647687Z",
      "changeKey": "xPZF2y46pEiVBni87OnrpgAAFq78Xw==",
      "categories": [],
      "originalStartTimeZone": "Eastern Standard Time",
      "originalEndTimeZone": "Eastern Standard Time",
      "iCalUId": "040000008200E00074C5B7101A82E00800000000824DDB122F0AD301000000000000000010000000824A8905B038D54AA7735F117B3442ED",
      "reminderMinutesBeforeStart": 15,
      "isReminderOn": true,
      "hasAttachments": false,
      "subject": "New Training Plans",
      "bodyPreview": "Meeting to plan new trainings.\r\n\r\n\r\n\r\nJoin Microsoft Teams Online Meeting<https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35>",
      "importance": "normal",
      "sensitivity": "normal",
      "isAllDay": false,
      "isCancelled": false,
      "isOrganizer": true,
      "responseRequested": true,
      "seriesMasterId": null,
      "showAs": "busy",
      "type": "seriesMaster",
      "webLink": "https://outlook.office365.com/owa/?itemid=AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA%2Bb2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOwAAAA%3D%3D&exvsurl=1&path=/calendar/item",
      "onlineMeetingUrl": null,
      "responseStatus": {
          "response": "organizer",
          "time": "0001-01-01T00:00:00Z"
      },
      "body": {
          "contentType": "html",
          "content": "<html>\r\n<head>\r\n<meta http-equiv=\"Content-Type\" content=\"text/html; charset=utf-8\">\r\n</head>\r\n<body>\r\n<div>Meeting to plan new trainings.</div>\r\n<div><br>\r\n<br>\r\n<br>\r\n<a href=\"https://teams.microsoft.com/l/meetup-join/19%3a900876baa3134907b0dcb41a0d220e31%40thread.skype/1501527539926?tenantId=dcd219dd-bc68-4b9b-bf0b-4a33a796be35\">Join Microsoft Teams Online Meeting</a></div>\r\n</body>\r\n</html>\r\n"
      },
      "start": {
          "dateTime": "2017-08-14T21:00:00.0000000",
          "timeZone": "UTC"
      },
      "end": {
          "dateTime": "2017-08-14T22:00:00.0000000",
          "timeZone": "UTC"
      },
      "location": {
          "displayName": "HR Taskforce / Facilities"
      },
      "recurrence": {
          "pattern": {
              "type": "weekly",
              "interval": 1,
              "month": 0,
              "dayOfMonth": 0,
              "daysOfWeek": [
                  "monday",
                  "wednesday",
                  "friday"
              ],
              "firstDayOfWeek": "sunday",
              "index": "first"
          },
          "range": {
              "type": "noEnd",
              "startDate": "2017-08-14",
              "endDate": "0001-01-01",
              "recurrenceTimeZone": "Eastern Standard Time",
              "numberOfOccurrences": 0
          }
      },
      "attendees": [
          {
              "type": "required",
              "status": {
                  "response": "accepted",
                  "time": "2017-07-31T18:59:06.4180028Z"
              },
              "emailAddress": {
                  "name": "Joni Sherman",
                  "address": "JoniS@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "HR Taskforce",
                  "address": "HRTaskforce@contoso.onmicrosoft.com"
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
                  "address": "MeganB@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Lidia Holloway",
                  "address": "LidiaH@contoso.onmicrosoft.com"
              }
          },
          {
              "type": "required",
              "status": {
                  "response": "none",
                  "time": "0001-01-01T00:00:00Z"
              },
              "emailAddress": {
                  "name": "Emily Braun",
                  "address": "EmilyB@contoso.onmicrosoft.com"
              }
          }
      ],
      "organizer": {
          "emailAddress": {
              "name": "HR Taskforce",
              "address": "HRTaskforce@contoso.onmicrosoft.com"
          }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
