---
title: 列出实例
description: 获取指定的时间范围的事件的实例（发生次数）。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 142e044e1d0181c9739f329cda976a2829b61abf
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259183"
---
# <a name="list-instances"></a><span data-ttu-id="6af2d-103">列出实例</span><span class="sxs-lookup"><span data-stu-id="6af2d-103">List instances</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6af2d-104">获取指定的时间范围的事件的实例（发生次数）。</span><span class="sxs-lookup"><span data-stu-id="6af2d-104">Get the instances (occurrences) of an event for a specified time range.</span></span> 

<span data-ttu-id="6af2d-105">如果事件的类型是 `seriesMaster`，这将返回在指定的时间范围内事件的发生次数和异常。</span><span class="sxs-lookup"><span data-stu-id="6af2d-105">If the event is a `seriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="6af2d-106">权限</span><span class="sxs-lookup"><span data-stu-id="6af2d-106">Permissions</span></span>
<span data-ttu-id="6af2d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6af2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6af2d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6af2d-109">Permission type</span></span>      | <span data-ttu-id="6af2d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6af2d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6af2d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6af2d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6af2d-112">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6af2d-112">Calendars.Read</span></span>    |
|<span data-ttu-id="6af2d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6af2d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6af2d-114">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6af2d-114">Calendars.Read</span></span>    |
|<span data-ttu-id="6af2d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6af2d-115">Application</span></span> | <span data-ttu-id="6af2d-116">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="6af2d-116">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="6af2d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6af2d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /groups/{id}/calendar/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="6af2d-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="6af2d-118">Query parameters</span></span>

<span data-ttu-id="6af2d-119">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="6af2d-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="6af2d-120">参数</span><span class="sxs-lookup"><span data-stu-id="6af2d-120">Parameter</span></span>    | <span data-ttu-id="6af2d-121">类型</span><span class="sxs-lookup"><span data-stu-id="6af2d-121">Type</span></span>   |<span data-ttu-id="6af2d-122">说明</span><span class="sxs-lookup"><span data-stu-id="6af2d-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6af2d-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6af2d-123">startDateTime</span></span>|<span data-ttu-id="6af2d-124">String</span><span class="sxs-lookup"><span data-stu-id="6af2d-124">String</span></span>|<span data-ttu-id="6af2d-p102">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="6af2d-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="6af2d-127">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6af2d-127">endDateTime</span></span>|<span data-ttu-id="6af2d-128">String</span><span class="sxs-lookup"><span data-stu-id="6af2d-128">String</span></span>|<span data-ttu-id="6af2d-p103">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="6af2d-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="6af2d-131">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6af2d-131">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6af2d-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="6af2d-132">Request headers</span></span>
| <span data-ttu-id="6af2d-133">名称</span><span class="sxs-lookup"><span data-stu-id="6af2d-133">Name</span></span>       | <span data-ttu-id="6af2d-134">类型</span><span class="sxs-lookup"><span data-stu-id="6af2d-134">Type</span></span> | <span data-ttu-id="6af2d-135">说明</span><span class="sxs-lookup"><span data-stu-id="6af2d-135">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="6af2d-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="6af2d-136">Authorization</span></span>  | <span data-ttu-id="6af2d-137">string</span><span class="sxs-lookup"><span data-stu-id="6af2d-137">string</span></span> | <span data-ttu-id="6af2d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6af2d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6af2d-140">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="6af2d-140">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="6af2d-141">string</span><span class="sxs-lookup"><span data-stu-id="6af2d-141">string</span></span> | <span data-ttu-id="6af2d-142">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="6af2d-142">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="6af2d-143">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="6af2d-143">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="6af2d-144">可选。</span><span class="sxs-lookup"><span data-stu-id="6af2d-144">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6af2d-145">请求正文</span><span class="sxs-lookup"><span data-stu-id="6af2d-145">Request body</span></span>
<span data-ttu-id="6af2d-146">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6af2d-146">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6af2d-147">响应</span><span class="sxs-lookup"><span data-stu-id="6af2d-147">Response</span></span>

<span data-ttu-id="6af2d-148">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6af2d-148">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6af2d-149">示例</span><span class="sxs-lookup"><span data-stu-id="6af2d-149">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6af2d-150">请求</span><span class="sxs-lookup"><span data-stu-id="6af2d-150">Request</span></span>
<span data-ttu-id="6af2d-151">下面的示例在指定的时间范围内, 事件是定期系列的主事件的事件发生和异常。</span><span class="sxs-lookup"><span data-stu-id="6af2d-151">The following example gets within the specified time range the occurrences and exceptions of an event which is the master event of a recurring series.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGUzYRgWAAA="],
  "name": "get_instances"
}-->
```http
GET https://graph.microsoft.com/beta/me/events/AAMkAGUzYRgWAAA=/instances?startDateTime=2019-04-08T09:00:00.0000000&endDateTime=2019-04-30T09:00:00.0000000&$select=subject,bodyPreview,seriesMasterId,type,recurrence,start,end
```
##### <a name="response"></a><span data-ttu-id="6af2d-152">响应</span><span class="sxs-lookup"><span data-stu-id="6af2d-152">Response</span></span>
<span data-ttu-id="6af2d-153">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6af2d-153">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "get_instances",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/events('AAMkAGUzYRgWAAA%3D')/instances(subject,bodyPreview,seriesMasterId,type,recurrence,start,end)",
    "value": [
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1sE1TatAAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "Changing meeting from 4/15 to 4/16.",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "exception",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-16T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-16T21:00:00.0000000",
                "timeZone": "UTC"
            }
        },
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1ru1JMcAAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "occurrence",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-08T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-08T21:00:00.0000000",
                "timeZone": "UTC"
            }
        },
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1sa1do_AAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "occurrence",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-22T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-22T21:00:00.0000000",
                "timeZone": "UTC"
            }
        },
        {
            "@odata.etag": "W/\"x3IAvB5fbUWf4XNcBFLNUwAAKuA3yQ==\"",
            "id": "AAMkAGUzYAgI1sw1n3PAAEYAAAAAlNFb2CNPe0ucP9you",
            "subject": "Review strategy for Q3",
            "bodyPreview": "",
            "seriesMasterId": "AAMkAGUzYRgWAAA=",
            "type": "occurrence",
            "recurrence": null,
            "start": {
                "dateTime": "2019-04-29T20:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2019-04-29T21:00:00.0000000",
                "timeZone": "UTC"
            }
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="6af2d-154">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6af2d-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6af2d-155">C#</span><span class="sxs-lookup"><span data-stu-id="6af2d-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_instances-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6af2d-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="6af2d-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_instances-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6af2d-157">目标-C</span><span class="sxs-lookup"><span data-stu-id="6af2d-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_instances-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/event-list-instances.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/event-list-instances.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/event-list-instances.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
