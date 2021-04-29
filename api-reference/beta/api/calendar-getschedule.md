---
title: 日历：getSchedule
description: 获取用户、通讯组列表或资源在指定时间段内的忙/闲状态信息。
localization_priority: Priority
author: tariq-sharif
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1b91b0b0aad21c87d01ff813b85dc5b8861cff25
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047754"
---
# <a name="calendar-getschedule"></a><span data-ttu-id="08b95-103">日历：getSchedule</span><span class="sxs-lookup"><span data-stu-id="08b95-103">calendar: getSchedule</span></span>

<span data-ttu-id="08b95-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08b95-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08b95-105">获取用户、通讯组列表或资源（会议室或设备）在指定时间段内的忙/闲状态信息。</span><span class="sxs-lookup"><span data-stu-id="08b95-105">Get the free/busy availability information for a collection of users, distributions lists, or resources (rooms or equipment) for a specified time period.</span></span>

## <a name="permissions"></a><span data-ttu-id="08b95-106">权限</span><span class="sxs-lookup"><span data-stu-id="08b95-106">Permissions</span></span>
<span data-ttu-id="08b95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08b95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08b95-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="08b95-109">Permission type</span></span>      | <span data-ttu-id="08b95-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08b95-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08b95-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08b95-111">Delegated (work or school account)</span></span> | <span data-ttu-id="08b95-112">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08b95-112">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="08b95-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08b95-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08b95-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="08b95-114">Not supported.</span></span> |
|<span data-ttu-id="08b95-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="08b95-115">Application</span></span> | <span data-ttu-id="08b95-116">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="08b95-116">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="08b95-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08b95-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/calendar/getSchedule 
POST /users/{id|userPrincipalName}/calendar/getSchedule
```

## <a name="request-headers"></a><span data-ttu-id="08b95-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="08b95-118">Request headers</span></span>
| <span data-ttu-id="08b95-119">名称</span><span class="sxs-lookup"><span data-stu-id="08b95-119">Name</span></span>       | <span data-ttu-id="08b95-120">类型</span><span class="sxs-lookup"><span data-stu-id="08b95-120">Type</span></span> | <span data-ttu-id="08b95-121">说明</span><span class="sxs-lookup"><span data-stu-id="08b95-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="08b95-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08b95-122">Authorization</span></span>  | <span data-ttu-id="08b95-123">string</span><span class="sxs-lookup"><span data-stu-id="08b95-123">string</span></span>  | <span data-ttu-id="08b95-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08b95-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08b95-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08b95-126">Content-Type</span></span>  | <span data-ttu-id="08b95-127">string</span><span class="sxs-lookup"><span data-stu-id="08b95-127">string</span></span> | <span data-ttu-id="08b95-p103">实体正文中的数据性质（为 application/json）。必填。</span><span class="sxs-lookup"><span data-stu-id="08b95-p103">Nature of the data in the body of an entity, which is application/json. Required.</span></span>  |
| <span data-ttu-id="08b95-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="08b95-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="08b95-131">string</span><span class="sxs-lookup"><span data-stu-id="08b95-131">string</span></span> | <span data-ttu-id="08b95-132">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="08b95-132">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="08b95-133">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="08b95-133">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="08b95-134">可选。</span><span class="sxs-lookup"><span data-stu-id="08b95-134">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="08b95-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="08b95-135">Request body</span></span>
<span data-ttu-id="08b95-136">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="08b95-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="08b95-137">属性</span><span class="sxs-lookup"><span data-stu-id="08b95-137">Property</span></span>     | <span data-ttu-id="08b95-138">类型</span><span class="sxs-lookup"><span data-stu-id="08b95-138">Type</span></span>   |<span data-ttu-id="08b95-139">说明</span><span class="sxs-lookup"><span data-stu-id="08b95-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="08b95-140">availabilityViewInterval</span><span class="sxs-lookup"><span data-stu-id="08b95-140">availabilityViewInterval</span></span>|<span data-ttu-id="08b95-141">Int32</span><span class="sxs-lookup"><span data-stu-id="08b95-141">Int32</span></span>|<span data-ttu-id="08b95-142">表示响应中 **availabilityView** 中的时间段的持续时间。</span><span class="sxs-lookup"><span data-stu-id="08b95-142">Represents the duration of a time slot in an **availabilityView** in the response.</span></span> <span data-ttu-id="08b95-143">默认值为 30 分钟，最小值为 5，最大值为 1440。</span><span class="sxs-lookup"><span data-stu-id="08b95-143">The default is 30 minutes, minimum is 5, maximum is 1440.</span></span> <span data-ttu-id="08b95-144">可选。</span><span class="sxs-lookup"><span data-stu-id="08b95-144">Optional.</span></span>|
|<span data-ttu-id="08b95-145">endTime</span><span class="sxs-lookup"><span data-stu-id="08b95-145">endTime</span></span>|[<span data-ttu-id="08b95-146">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="08b95-146">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="08b95-147">时间段结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="08b95-147">The date, time, and time zone that the period ends.</span></span>|
|<span data-ttu-id="08b95-148">schedules</span><span class="sxs-lookup"><span data-stu-id="08b95-148">schedules</span></span>|<span data-ttu-id="08b95-149">String 集合</span><span class="sxs-lookup"><span data-stu-id="08b95-149">String collection</span></span>|<span data-ttu-id="08b95-150">要获取忙/闲状态信息的用户、通讯组列表或资源的 SMTP 地址集合。</span><span class="sxs-lookup"><span data-stu-id="08b95-150">A collection of SMTP addresses of users, distribution lists, or resources to get availability information for.</span></span>|
|<span data-ttu-id="08b95-151">startTime</span><span class="sxs-lookup"><span data-stu-id="08b95-151">startTime</span></span>|[<span data-ttu-id="08b95-152">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="08b95-152">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md)|<span data-ttu-id="08b95-153">时间段开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="08b95-153">The date, time, and time zone that the period starts.</span></span>|

## <a name="response"></a><span data-ttu-id="08b95-154">响应</span><span class="sxs-lookup"><span data-stu-id="08b95-154">Response</span></span>

<span data-ttu-id="08b95-155">如果成功，此方法为 `schedules` 参数中的每个对象返回 `200 OK` 响应代码和 [scheduleInformation](../resources/scheduleinformation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="08b95-155">If successful, this method returns a `200 OK` response code and a collection of [scheduleInformation](../resources/scheduleinformation.md) objects for each object in the `schedules` parameter.</span></span>
## <a name="example"></a><span data-ttu-id="08b95-156">示例</span><span class="sxs-lookup"><span data-stu-id="08b95-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08b95-157">请求</span><span class="sxs-lookup"><span data-stu-id="08b95-157">Request</span></span>
<span data-ttu-id="08b95-158">以下示例将获取指定日期、时间和时区的两名用户的忙/闲状态信息。</span><span class="sxs-lookup"><span data-stu-id="08b95-158">The following example gets the availability information for two users for the specified date, time, and time zone.</span></span>


# <a name="http"></a>[<span data-ttu-id="08b95-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="08b95-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="08b95-160">C#</span><span class="sxs-lookup"><span data-stu-id="08b95-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/calendar-getschedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="08b95-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="08b95-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/calendar-getschedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="08b95-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="08b95-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/calendar-getschedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="08b95-163">Java</span><span class="sxs-lookup"><span data-stu-id="08b95-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/calendar-getschedule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="08b95-164">响应</span><span class="sxs-lookup"><span data-stu-id="08b95-164">Response</span></span>
<span data-ttu-id="08b95-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="08b95-165">Here is an example of the response.</span></span> <span data-ttu-id="08b95-166">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="08b95-166">Note: The response object shown here might be shortened for readability.</span></span>
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


