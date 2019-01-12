---
title: 日历： getSchedule
description: 获取闲/忙时间集的用户、 通讯组列表或资源的信息指定的时间段。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 9089489d2b26b3dd4cd56b950538a72ab533c933
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956953"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="96dd6-103">日历： getSchedule</span><span class="sxs-lookup"><span data-stu-id="96dd6-103">calendar: getSchedule</span></span>

> <span data-ttu-id="96dd6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="96dd6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96dd6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="96dd6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96dd6-106">获取闲/忙时间集的用户、 通讯组列表或资源的信息指定的时间段。</span><span class="sxs-lookup"><span data-stu-id="96dd6-106">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="96dd6-107">权限</span><span class="sxs-lookup"><span data-stu-id="96dd6-107">Permissions</span></span>
<span data-ttu-id="96dd6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96dd6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96dd6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="96dd6-110">Permission type</span></span>      | <span data-ttu-id="96dd6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96dd6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96dd6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96dd6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="96dd6-113">Calendar.Read Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96dd6-113">Calendar.Read, Calendar.ReadWrite</span></span>    |
|<span data-ttu-id="96dd6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96dd6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96dd6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="96dd6-115">Not supported.</span></span> |
|<span data-ttu-id="96dd6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="96dd6-116">Application</span></span> | <span data-ttu-id="96dd6-117">Calendar.Read Calendar.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="96dd6-117">Calendar.Read, Calendar.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="96dd6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96dd6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="96dd6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="96dd6-119">Request headers</span></span>
| <span data-ttu-id="96dd6-120">名称</span><span class="sxs-lookup"><span data-stu-id="96dd6-120">Name</span></span>       | <span data-ttu-id="96dd6-121">类型</span><span class="sxs-lookup"><span data-stu-id="96dd6-121">Type</span></span> | <span data-ttu-id="96dd6-122">说明</span><span class="sxs-lookup"><span data-stu-id="96dd6-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="96dd6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96dd6-123">Authorization</span></span>  | <span data-ttu-id="96dd6-124">string</span><span class="sxs-lookup"><span data-stu-id="96dd6-124">string</span></span>  | <span data-ttu-id="96dd6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96dd6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="96dd6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="96dd6-127">Content-Type</span></span>  | <span data-ttu-id="96dd6-128">string</span><span class="sxs-lookup"><span data-stu-id="96dd6-128">string</span></span> | <span data-ttu-id="96dd6-129">实体，即 application/json 的正文中的数据的性质。</span><span class="sxs-lookup"><span data-stu-id="96dd6-129">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="96dd6-130">必需。</span><span class="sxs-lookup"><span data-stu-id="96dd6-130">Required.</span></span>  |
| <span data-ttu-id="96dd6-131">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="96dd6-131">Prefer: outlook.timezone</span></span> | <span data-ttu-id="96dd6-132">string</span><span class="sxs-lookup"><span data-stu-id="96dd6-132">string</span></span> | <span data-ttu-id="96dd6-133">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="96dd6-133">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="96dd6-134">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="96dd6-134">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="96dd6-135">可选。</span><span class="sxs-lookup"><span data-stu-id="96dd6-135">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96dd6-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="96dd6-136">Request body</span></span>
<span data-ttu-id="96dd6-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="96dd6-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="96dd6-138">属性</span><span class="sxs-lookup"><span data-stu-id="96dd6-138">Property</span></span>     | <span data-ttu-id="96dd6-139">类型</span><span class="sxs-lookup"><span data-stu-id="96dd6-139">Type</span></span>   |<span data-ttu-id="96dd6-140">说明</span><span class="sxs-lookup"><span data-stu-id="96dd6-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96dd6-141">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="96dd6-141">availabilityViewInterval</span></span>|<span data-ttu-id="96dd6-142">字符串</span><span class="sxs-lookup"><span data-stu-id="96dd6-142">String</span></span>|<span data-ttu-id="96dd6-143">表示在响应中**availabilityView**中的时间段的持续时间。</span><span class="sxs-lookup"><span data-stu-id="96dd6-143">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="96dd6-144">默认值为 30 分钟，最小值为 6，最大值是 1440年。</span><span class="sxs-lookup"><span data-stu-id="96dd6-144">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="96dd6-145">可选。</span><span class="sxs-lookup"><span data-stu-id="96dd6-145">Optional.</span></span>|
|<span data-ttu-id="96dd6-146">endTime</span><span class="sxs-lookup"><span data-stu-id="96dd6-146">endTime</span></span>|[<span data-ttu-id="96dd6-147">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="96dd6-147">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="96dd6-148">日期、 时间和时区期的结束。</span><span class="sxs-lookup"><span data-stu-id="96dd6-148">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="96dd6-149">计划</span><span class="sxs-lookup"><span data-stu-id="96dd6-149">schedules</span></span>|<span data-ttu-id="96dd6-150">String 集合</span><span class="sxs-lookup"><span data-stu-id="96dd6-150">String collection</span></span>|<span data-ttu-id="96dd6-151">若要获取的可用性信息的用户、 通讯组列表或资源的 SMTP 地址的集合。</span><span class="sxs-lookup"><span data-stu-id="96dd6-151">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="96dd6-152">startTime</span><span class="sxs-lookup"><span data-stu-id="96dd6-152">startTime</span></span>|[<span data-ttu-id="96dd6-153">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="96dd6-153">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="96dd6-154">日期、 时间和时区期的开始。</span><span class="sxs-lookup"><span data-stu-id="96dd6-154">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="96dd6-155">响应</span><span class="sxs-lookup"><span data-stu-id="96dd6-155">Response</span></span>

<span data-ttu-id="96dd6-156">如果成功，此方法返回`200 OK`响应代码和[scheduleInformation](../resources/scheduleinformation.md)对象中每个对象的集合`schedules`参数。</span><span class="sxs-lookup"><span data-stu-id="96dd6-156">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="96dd6-157">示例</span><span class="sxs-lookup"><span data-stu-id="96dd6-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="96dd6-158">请求</span><span class="sxs-lookup"><span data-stu-id="96dd6-158">Request</span></span>
<span data-ttu-id="96dd6-159">下面的示例获取指定的日期、 时间和时区的两个用户的可用性信息。</span><span class="sxs-lookup"><span data-stu-id="96dd6-159">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>

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

##### <a name="response"></a><span data-ttu-id="96dd6-160">响应</span><span class="sxs-lookup"><span data-stu-id="96dd6-160">Response</span></span>
<span data-ttu-id="96dd6-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96dd6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "calendar: getSchedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
