---
title: 日历：getSchedule
description: 获取用户、通讯组列表或资源在指定时间段内的忙/闲状态信息。
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c359935d7a18c4ff94b2f037b37d52c675a4708b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419144"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="a4687-103">日历：getSchedule</span><span class="sxs-lookup"><span data-stu-id="a4687-103">calendar: getSchedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4687-104">获取用户、通讯组列表或资源（会议室或设备）在指定时间段内的忙/闲状态信息。</span><span class="sxs-lookup"><span data-stu-id="a4687-104">Get the free/busy availability information for a collection of users, distributions lists, or resources (rooms or equipment) for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4687-105">权限</span><span class="sxs-lookup"><span data-stu-id="a4687-105">Permissions</span></span>
<span data-ttu-id="a4687-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4687-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4687-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4687-108">Permission type</span></span>      | <span data-ttu-id="a4687-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4687-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4687-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4687-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a4687-111">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4687-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="a4687-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4687-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4687-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4687-113">Not supported.</span></span> |
|<span data-ttu-id="a4687-114">Application</span><span class="sxs-lookup"><span data-stu-id="a4687-114">Application</span></span> | <span data-ttu-id="a4687-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4687-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4687-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4687-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="a4687-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4687-117">Request headers</span></span>
| <span data-ttu-id="a4687-118">名称</span><span class="sxs-lookup"><span data-stu-id="a4687-118">Name</span></span>       | <span data-ttu-id="a4687-119">类型</span><span class="sxs-lookup"><span data-stu-id="a4687-119">Type</span></span> | <span data-ttu-id="a4687-120">说明</span><span class="sxs-lookup"><span data-stu-id="a4687-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a4687-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4687-121">Authorization</span></span>  | <span data-ttu-id="a4687-122">string</span><span class="sxs-lookup"><span data-stu-id="a4687-122">string</span></span>  | <span data-ttu-id="a4687-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4687-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a4687-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a4687-125">Content-Type</span></span>  | <span data-ttu-id="a4687-126">string</span><span class="sxs-lookup"><span data-stu-id="a4687-126">string</span></span> | <span data-ttu-id="a4687-127">实体正文中的数据性质（为 application/json）。</span><span class="sxs-lookup"><span data-stu-id="a4687-127">Nature of the data in the body of an entity, which is application/json.</span></span> <span data-ttu-id="a4687-128">必需。</span><span class="sxs-lookup"><span data-stu-id="a4687-128">Required.</span></span>  |
| <span data-ttu-id="a4687-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="a4687-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="a4687-130">string</span><span class="sxs-lookup"><span data-stu-id="a4687-130">string</span></span> | <span data-ttu-id="a4687-131">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="a4687-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="a4687-132">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a4687-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="a4687-133">可选。</span><span class="sxs-lookup"><span data-stu-id="a4687-133">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4687-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4687-134">Request body</span></span>
<span data-ttu-id="a4687-135">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a4687-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4687-136">属性</span><span class="sxs-lookup"><span data-stu-id="a4687-136">Property</span></span>     | <span data-ttu-id="a4687-137">类型</span><span class="sxs-lookup"><span data-stu-id="a4687-137">Type</span></span>   |<span data-ttu-id="a4687-138">说明</span><span class="sxs-lookup"><span data-stu-id="a4687-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4687-139">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="a4687-139">availabilityViewInterval</span></span>|<span data-ttu-id="a4687-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a4687-140">Int32</span></span>|<span data-ttu-id="a4687-141">表示响应中 **availabilityView** 中的时间段的持续时间。</span><span class="sxs-lookup"><span data-stu-id="a4687-141">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="a4687-142">默认值为 30 分钟，最小值为 6，最大值为 1440。</span><span class="sxs-lookup"><span data-stu-id="a4687-142">The default is 30 minutes, minimum is 6, maximum is 1440.</span></span> <span data-ttu-id="a4687-143">可选。</span><span class="sxs-lookup"><span data-stu-id="a4687-143">Optional.</span></span>|
|<span data-ttu-id="a4687-144">endTime</span><span class="sxs-lookup"><span data-stu-id="a4687-144">endTime</span></span>|[<span data-ttu-id="a4687-145">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a4687-145">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a4687-146">时间段结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="a4687-146">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="a4687-147">schedules</span><span class="sxs-lookup"><span data-stu-id="a4687-147">schedules</span></span>|<span data-ttu-id="a4687-148">String 集合</span><span class="sxs-lookup"><span data-stu-id="a4687-148">String collection</span></span>|<span data-ttu-id="a4687-149">要获取忙/闲状态信息的用户、通讯组列表或资源的 SMTP 地址集合。</span><span class="sxs-lookup"><span data-stu-id="a4687-149">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="a4687-150">startTime</span><span class="sxs-lookup"><span data-stu-id="a4687-150">startTime</span></span>|[<span data-ttu-id="a4687-151">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="a4687-151">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="a4687-152">时间段开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="a4687-152">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="a4687-153">响应</span><span class="sxs-lookup"><span data-stu-id="a4687-153">Response</span></span>

<span data-ttu-id="a4687-154">如果成功，此方法为 `schedules` 参数中的每个对象返回 `200 OK` 响应代码和 [scheduleInformation](../resources/scheduleinformation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a4687-154">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="a4687-155">示例</span><span class="sxs-lookup"><span data-stu-id="a4687-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4687-156">请求</span><span class="sxs-lookup"><span data-stu-id="a4687-156">Request</span></span>
<span data-ttu-id="a4687-157">以下示例将获取指定日期、时间和时区的两名用户的忙/闲状态信息。</span><span class="sxs-lookup"><span data-stu-id="a4687-157">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a4687-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="a4687-158">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "calendar_getSchedule"
}-->
```http
POST https://graph.microsoft.com/beta/me/calendar/getSchedule 
Prefer: outlook.timezone="Pacific Standard Time"
Content-Type: application/json

{        
    "schedules": ["adelev@contoso.onmicrosoft.com", "meganb@contoso.onmicrosoft.com"],
    "startTime": {
        "dateTime": "2019-03-15T09:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "endTime": {
        "dateTime": "2019-03-15T18:00:00",
        "timeZone": "Pacific Standard Time"
    },
    "availabilityViewInterval": 60
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a4687-159">C#</span><span class="sxs-lookup"><span data-stu-id="a4687-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-getschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4687-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a4687-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-getschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a4687-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a4687-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-getschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a4687-162">响应</span><span class="sxs-lookup"><span data-stu-id="a4687-162">Response</span></span>
<span data-ttu-id="a4687-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a4687-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scheduleInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.scheduleInformation)",
    "value": [
        {
            "scheduleId": "adelev@contoso.onmicrosoft.com",
            "availabilityView": "000220000",
            "scheduleItems": [
                {
                    "isPrivate": false,
                    "status": "busy",
                    "subject": "Let's go for lunch",
                    "location": "Harry's Bar",
                    "start": {
                        "dateTime": "2019-03-15T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                }
            ],
            "workingHours": {
                "daysOfWeek": [
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime": "08:00:00.0000000",
                "endTime": "17:00:00.0000000",
                "timeZone": {
                    "name": "Pacific Standard Time"
                }
            }
        },
        {
            "scheduleId": "meganb@contoso.onmicrosoft.com",
            "availabilityView": "200220010",
            "scheduleItems": [
                {
                    "status": "busy",
                    "start": {
                        "dateTime": "2019-03-15T08:30:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T09:30:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "busy",
                    "start": {
                        "dateTime": "2019-03-15T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "tentative",
                    "start": {
                        "dateTime": "2019-03-15T12:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T13:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "busy",
                    "start": {
                        "dateTime": "2019-03-15T13:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T14:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                },
                {
                    "status": "tentative",
                    "start": {
                        "dateTime": "2019-03-15T16:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    },
                    "end": {
                        "dateTime": "2019-03-15T17:00:00.0000000",
                        "timeZone": "Pacific Standard Time"
                    }
                }
            ],
            "workingHours": {
                "daysOfWeek": [
                    "monday",
                    "tuesday",
                    "wednesday",
                    "thursday",
                    "friday"
                ],
                "startTime": "08:00:00.0000000",
                "endTime": "17:00:00.0000000",
                "timeZone": {
                    "@odata.type": "#microsoft.graph.customTimeZone",
                    "bias": 480,
                    "name": "Customized Time Zone",
                    "standardOffset": {
                        "time": "02:00:00.0000000",
                        "dayOccurrence": 1,
                        "dayOfWeek": "sunday",
                        "month": 11,
                        "year": 0
                    },
                    "daylightOffset": {
                        "daylightBias": -60,
                        "time": "02:00:00.0000000",
                        "dayOccurrence": 2,
                        "dayOfWeek": "sunday",
                        "month": 3,
                        "year": 0
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
  "suppressions": []
}
-->
