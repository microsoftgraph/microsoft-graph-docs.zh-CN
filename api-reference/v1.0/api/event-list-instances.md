---
title: 列出实例
description: 获取指定的时间范围的事件的实例（发生次数）。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b19b452f029b7d4223bcc150f184b805a311cecd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448289"
---
# <a name="list-instances"></a><span data-ttu-id="bfe9d-103">列表实例</span><span class="sxs-lookup"><span data-stu-id="bfe9d-103">List instances</span></span>

<span data-ttu-id="bfe9d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfe9d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bfe9d-105">获取指定的时间范围的事件的实例（发生次数）。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-105">Get the instances (occurrences) of an event for a specified time range.</span></span> 

<span data-ttu-id="bfe9d-106">如果事件的类型是 `seriesMaster`，这将返回在指定的时间范围内事件的发生次数和异常。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-106">If the event is a `seriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfe9d-107">权限</span><span class="sxs-lookup"><span data-stu-id="bfe9d-107">Permissions</span></span>
<span data-ttu-id="bfe9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfe9d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfe9d-110">Permission type</span></span>      | <span data-ttu-id="bfe9d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bfe9d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfe9d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfe9d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bfe9d-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bfe9d-113">Calendars.Read</span></span>    |
|<span data-ttu-id="bfe9d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfe9d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfe9d-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bfe9d-115">Calendars.Read</span></span>    |
|<span data-ttu-id="bfe9d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfe9d-116">Application</span></span> | <span data-ttu-id="bfe9d-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="bfe9d-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfe9d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfe9d-118">HTTP request</span></span>
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

GET /me/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances?startDateTime={start_datetime}&endDateTime={end_datetime}
```
## <a name="query-parameters"></a><span data-ttu-id="bfe9d-119">查询参数</span><span class="sxs-lookup"><span data-stu-id="bfe9d-119">Query parameters</span></span>

<span data-ttu-id="bfe9d-120">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-120">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="bfe9d-121">参数</span><span class="sxs-lookup"><span data-stu-id="bfe9d-121">Parameter</span></span>    | <span data-ttu-id="bfe9d-122">类型</span><span class="sxs-lookup"><span data-stu-id="bfe9d-122">Type</span></span>   |<span data-ttu-id="bfe9d-123">说明</span><span class="sxs-lookup"><span data-stu-id="bfe9d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfe9d-124">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bfe9d-124">startDateTime</span></span>|<span data-ttu-id="bfe9d-125">String</span><span class="sxs-lookup"><span data-stu-id="bfe9d-125">String</span></span>|<span data-ttu-id="bfe9d-p102">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-p102">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="bfe9d-128">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bfe9d-128">endDateTime</span></span>|<span data-ttu-id="bfe9d-129">String</span><span class="sxs-lookup"><span data-stu-id="bfe9d-129">String</span></span>|<span data-ttu-id="bfe9d-p103">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-p103">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|

<span data-ttu-id="bfe9d-132">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-132">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bfe9d-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfe9d-133">Request headers</span></span>
| <span data-ttu-id="bfe9d-134">名称</span><span class="sxs-lookup"><span data-stu-id="bfe9d-134">Name</span></span>       | <span data-ttu-id="bfe9d-135">类型</span><span class="sxs-lookup"><span data-stu-id="bfe9d-135">Type</span></span> | <span data-ttu-id="bfe9d-136">说明</span><span class="sxs-lookup"><span data-stu-id="bfe9d-136">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="bfe9d-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfe9d-137">Authorization</span></span>  | <span data-ttu-id="bfe9d-138">string</span><span class="sxs-lookup"><span data-stu-id="bfe9d-138">string</span></span> | <span data-ttu-id="bfe9d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bfe9d-141">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="bfe9d-141">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="bfe9d-142">string</span><span class="sxs-lookup"><span data-stu-id="bfe9d-142">string</span></span> | <span data-ttu-id="bfe9d-143">此选项可用于指定响应中开始时间和结束时间的时区。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-143">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="bfe9d-144">如果未指定，返回的这些时间值采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-144">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="bfe9d-145">可选。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-145">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bfe9d-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfe9d-146">Request body</span></span>
<span data-ttu-id="bfe9d-147">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfe9d-148">响应</span><span class="sxs-lookup"><span data-stu-id="bfe9d-148">Response</span></span>

<span data-ttu-id="bfe9d-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Event](../resources/event.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-149">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/event.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bfe9d-150">示例</span><span class="sxs-lookup"><span data-stu-id="bfe9d-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfe9d-151">请求</span><span class="sxs-lookup"><span data-stu-id="bfe9d-151">Request</span></span>
<span data-ttu-id="bfe9d-152">以下示例在指定的时间范围内获取作为定期系列的主事件的事件的发生次数和例外。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-152">The following example gets within the specified time range the occurrences and exceptions of an event which is the master event of a recurring series.</span></span>

# <a name="http"></a>[<span data-ttu-id="bfe9d-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="bfe9d-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkAGUzYRgWAAA="],
  "name": "get_instances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/events/AAMkAGUzYRgWAAA=/instances?startDateTime=2019-04-08T09:00:00.0000000&endDateTime=2019-04-30T09:00:00.0000000&$select=subject,bodyPreview,seriesMasterId,type,recurrence,start,end
```
# <a name="c"></a>[<span data-ttu-id="bfe9d-154">C#</span><span class="sxs-lookup"><span data-stu-id="bfe9d-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-instances-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bfe9d-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bfe9d-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-instances-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bfe9d-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bfe9d-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-instances-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="bfe9d-157">Java</span><span class="sxs-lookup"><span data-stu-id="bfe9d-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-instances-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bfe9d-158">响应</span><span class="sxs-lookup"><span data-stu-id="bfe9d-158">Response</span></span>
<span data-ttu-id="bfe9d-159">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bfe9d-159">Here is an example of the response.</span></span> 
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('bb8775a4-4d8c-42cf-a1d4-4d58c2bb668f')/events('AAMkAGUzYRgWAAA%3D')/instances(subject,bodyPreview,seriesMasterId,type,recurrence,start,end)",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List instances",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
