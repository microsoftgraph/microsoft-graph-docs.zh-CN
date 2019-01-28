---
title: 日历：getSchedule
description: 获取用户、通讯组列表或资源在指定时间段内的忙/闲状态信息。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 0c2f6a54664242831d7fd3f2ddfc6a44984674e0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530025"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="30740-103">日历：getSchedule</span><span class="sxs-lookup"><span data-stu-id="30740-103">calendar: getSchedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30740-104">获取用户、通讯组列表或资源在指定时间段内的忙/闲状态信息。</span><span class="sxs-lookup"><span data-stu-id="30740-104">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="30740-105">权限</span><span class="sxs-lookup"><span data-stu-id="30740-105">Permissions</span></span>
<span data-ttu-id="30740-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="30740-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30740-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="30740-108">Permission type</span></span>      | <span data-ttu-id="30740-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="30740-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="30740-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30740-110">Delegated (work or school account)</span></span> | <span data-ttu-id="30740-111">Calendar.Read、Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30740-111">Calendar.Read, Calendar.ReadWrite</span></span>    |
|<span data-ttu-id="30740-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30740-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30740-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="30740-113">Not supported.</span></span> |
|<span data-ttu-id="30740-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="30740-114">Application</span></span> | <span data-ttu-id="30740-115">Calendar.Read、Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="30740-115">Calendar.Read, Calendar.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="30740-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30740-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="30740-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="30740-117">Request headers</span></span>
| <span data-ttu-id="30740-118">名称</span><span class="sxs-lookup"><span data-stu-id="30740-118">Name</span></span>       | <span data-ttu-id="30740-119">类型</span><span class="sxs-lookup"><span data-stu-id="30740-119">Type</span></span> | <span data-ttu-id="30740-120">说明</span><span class="sxs-lookup"><span data-stu-id="30740-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="30740-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="30740-121">Authorization</span></span>  | <span data-ttu-id="30740-122">string</span><span class="sxs-lookup"><span data-stu-id="30740-122">string</span></span>  | <span data-ttu-id="30740-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="30740-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="30740-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="30740-125">Content-Type</span></span>  | <span data-ttu-id="30740-126">string</span><span class="sxs-lookup"><span data-stu-id="30740-126">string</span></span> | <span data-ttu-id="30740-127">实体正文中的数据性质（为 application/json）。</span><span class="sxs-lookup"><span data-stu-id="30740-127">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="30740-128">必需。</span><span class="sxs-lookup"><span data-stu-id="30740-128">Required.</span></span>  |
| <span data-ttu-id="30740-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="30740-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="30740-130">string</span><span class="sxs-lookup"><span data-stu-id="30740-130">string</span></span> | <span data-ttu-id="30740-131">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="30740-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="30740-132">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="30740-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="30740-133">可选。</span><span class="sxs-lookup"><span data-stu-id="30740-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="30740-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="30740-134">Request body</span></span>
<span data-ttu-id="30740-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="30740-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="30740-136">属性</span><span class="sxs-lookup"><span data-stu-id="30740-136">Property</span></span>     | <span data-ttu-id="30740-137">类型</span><span class="sxs-lookup"><span data-stu-id="30740-137">Type</span></span>   |<span data-ttu-id="30740-138">说明</span><span class="sxs-lookup"><span data-stu-id="30740-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30740-139">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="30740-139">availabilityViewInterval</span></span>|<span data-ttu-id="30740-140">String</span><span class="sxs-lookup"><span data-stu-id="30740-140">String</span></span>|<span data-ttu-id="30740-141">表示响应中 **availabilityView** 中的时间段的持续时间。</span><span class="sxs-lookup"><span data-stu-id="30740-141">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="30740-142">默认值为 30 分钟，最小值为 6，最大值为 1440。</span><span class="sxs-lookup"><span data-stu-id="30740-142">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="30740-143">可选。</span><span class="sxs-lookup"><span data-stu-id="30740-143">Optional.</span></span>|
|<span data-ttu-id="30740-144">endTime</span><span class="sxs-lookup"><span data-stu-id="30740-144">endTime</span></span>|[<span data-ttu-id="30740-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="30740-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="30740-146">时间段结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="30740-146">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="30740-147">schedules</span><span class="sxs-lookup"><span data-stu-id="30740-147">schedules</span></span>|<span data-ttu-id="30740-148">String 集合</span><span class="sxs-lookup"><span data-stu-id="30740-148">String collection</span></span>|<span data-ttu-id="30740-149">要获取忙/闲状态信息的用户、通讯组列表或资源的 SMTP 地址集合。</span><span class="sxs-lookup"><span data-stu-id="30740-149">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="30740-150">startTime</span><span class="sxs-lookup"><span data-stu-id="30740-150">startTime</span></span>|[<span data-ttu-id="30740-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="30740-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="30740-152">时间段开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="30740-152">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="30740-153">响应</span><span class="sxs-lookup"><span data-stu-id="30740-153">Response</span></span>

<span data-ttu-id="30740-154">如果成功，此方法为 `schedules` 参数中的每个对象返回 `200 OK` 响应代码和 [scheduleInformation](../resources/scheduleinformation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="30740-154">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="30740-155">示例</span><span class="sxs-lookup"><span data-stu-id="30740-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="30740-156">请求</span><span class="sxs-lookup"><span data-stu-id="30740-156">Request</span></span>
<span data-ttu-id="30740-157">以下示例将获取指定日期、时间和时区的两名用户的忙/闲状态信息。</span><span class="sxs-lookup"><span data-stu-id="30740-157">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "calendar_getSchedule"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getschedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "schedules": ["AdeleV@contoso.onmicrosoft.com", "AlexW@contoso.OnMicrosoft.com"],
    "startTime": {
        "dateTime": "2018-08-06T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "endTime": {
        "dateTime": "2018-08-06T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": "15"
}
```

##### <a name="response"></a><span data-ttu-id="30740-158">响应</span><span class="sxs-lookup"><span data-stu-id="30740-158">Response</span></span>
<span data-ttu-id="30740-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30740-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value":[
        {
            "scheduleId":"AdeleV@contoso.onmicrosoft.com",
            "availabilityView":"222222000022000000000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "subject":"Admininstrators debrief",
                    "location":"Foyer",
                    "start":{
                        "dateTime":"2018-08-06T09:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T10:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                },
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "subject":"Lunch yoga",
                    "location":"Courtyard",
                    "start":{
                        "dateTime":"2018-08-06T11:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T12:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                }
            ],
            "workingHours":{
                "daysOfWeek":[
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime":"08:00:00.0000000",
                "endTime":"17:00:00.0000000",
                "timeZone":{
                    "@odata.type":"#microsoft.graph.customTimeZone",
                    "bias":480,
                    "name":"Customized Time Zone",
                    "standardOffset":{
                        "time":"02:00:00.0000000",
                        "dayOccurrence":1,
                        "dayOfWeek":"sunday",
                        "month":11,
                        "year":0
                    },
                    "daylightOffset":{
                        "daylightBias":-60,
                        "time":"02:00:00.0000000",
                        "dayOccurrence":2,
                        "dayOfWeek":"sunday",
                        "month":3,
                        "year":0
                    }
                }
            }
        },
        {
            "scheduleId":"AlexW@contoso.OnMicrosoft.com",
            "availabilityView":"111111002222222200000000000000000000",
            "scheduleItems":[
                {
                    "isPrivate":false,
                    "status":"Tentative",
                    "subject":"Admininstrators debrief",
                    "location":"Foyer",
                    "start":{
                        "dateTime":"2018-08-06T09:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T10:30:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                },
                {
                    "isPrivate":false,
                    "status":"Busy",
                    "subject":"Q4 planning",
                    "location":"Big Bear",
                    "start":{
                        "dateTime":"2018-08-06T11:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    },
                    "end":{
                        "dateTime":"2018-08-06T13:00:00.0000000",
                        "timeZone":"Pacific Standard Time"
                    }
                }
            ],
            "workingHours":{
                "daysOfWeek":[
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime":"08:00:00.0000000",
                "endTime":"17:00:00.0000000",
                "timeZone":{
                    "@odata.type":"#microsoft.graph.customTimeZone",
                    "bias":480,
                    "name":"Customized Time Zone",
                    "standardOffset":{
                        "time":"02:00:00.0000000",
                        "dayOccurrence":1,
                        "dayOfWeek":"sunday",
                        "month":11,
                        "year":0
                    },
                    "daylightOffset":{
                        "daylightBias":-60,
                        "time":"02:00:00.0000000",
                        "dayOccurrence":2,
                        "dayOfWeek":"sunday",
                        "month":3,
                        "year":0
                    }
                }
            }
        }
    ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "calendar: getSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendar-getschedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
