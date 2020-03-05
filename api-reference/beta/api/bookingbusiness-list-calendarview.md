---
title: 列出 Bookings 日历视图
description: 获取 bookingBusiness 的 bookingAppointment 对象的集合，该集合在指定的日期范围内发生。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 65840517f1029c06ac819ec54a9f2897d440cd1d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441254"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="4dc0c-103">列出 Bookings 日历视图</span><span class="sxs-lookup"><span data-stu-id="4dc0c-103">List Bookings calendarView</span></span>

<span data-ttu-id="4dc0c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4dc0c-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4dc0c-105">获取[bookingBusiness](../resources/bookingbusiness.md)的[bookingAppointment](../resources/bookingappointment.md)对象的集合，该集合在指定的日期范围内发生。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-105">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="4dc0c-106">权限</span><span class="sxs-lookup"><span data-stu-id="4dc0c-106">Permissions</span></span>
<span data-ttu-id="4dc0c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4dc0c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4dc0c-109">Permission type</span></span>      | <span data-ttu-id="4dc0c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4dc0c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4dc0c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4dc0c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="4dc0c-112">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="4dc0c-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4dc0c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4dc0c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4dc0c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-114">Not supported.</span></span>   |
|<span data-ttu-id="4dc0c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4dc0c-115">Application</span></span> | <span data-ttu-id="4dc0c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4dc0c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4dc0c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}
```

## <a name="query-parameters"></a><span data-ttu-id="4dc0c-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="4dc0c-118">Query parameters</span></span>

<span data-ttu-id="4dc0c-119">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="4dc0c-120">参数</span><span class="sxs-lookup"><span data-stu-id="4dc0c-120">Parameter</span></span>    | <span data-ttu-id="4dc0c-121">类型</span><span class="sxs-lookup"><span data-stu-id="4dc0c-121">Type</span></span>   |<span data-ttu-id="4dc0c-122">说明</span><span class="sxs-lookup"><span data-stu-id="4dc0c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4dc0c-123">start</span><span class="sxs-lookup"><span data-stu-id="4dc0c-123">start</span></span>|<span data-ttu-id="4dc0c-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dc0c-124">DateTimeOffset</span></span>|<span data-ttu-id="4dc0c-125">时间范围的开始日期和时间，以 ISO 8601 格式表示，如 UTC 或 UTC 时差。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-125">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="4dc0c-126">例如，2018年1月1日午夜 UTC 将如下所示： ' 2018-01-01T00：00： 00Z '，PST 的相同时间如下所示： ' 2017-12-31T16：00： 00-08： 00 '。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-126">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="4dc0c-127">end</span><span class="sxs-lookup"><span data-stu-id="4dc0c-127">end</span></span>|<span data-ttu-id="4dc0c-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4dc0c-128">DateTimeOffset</span></span>|<span data-ttu-id="4dc0c-129">时间范围的结束日期和时间，以 ISO 8601 格式表示，即 UTC 或 UTC 时差。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-129">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="4dc0c-130">例如，2018年1月1日的 3am UTC 如下所示： ' 2018-01-01T03：00： 00Z '，PST 中的相同时间如下所示： ' 2017-12-31T19：00： 00-08： 00 '。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-130">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

<span data-ttu-id="4dc0c-131">和的值使用其对应的值中指定的时区偏移量进行解释，如果存在，则不受`Prefer: outlook.timezone`标头值的影响。 `end` `start`</span><span class="sxs-lookup"><span data-stu-id="4dc0c-131">The values of `start` and `end` are interpreted using the timezone offset specified in their corresponding values and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span>

<span data-ttu-id="4dc0c-132">此方法还支持一些 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-132">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4dc0c-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="4dc0c-133">Request headers</span></span>
| <span data-ttu-id="4dc0c-134">名称</span><span class="sxs-lookup"><span data-stu-id="4dc0c-134">Name</span></span>       | <span data-ttu-id="4dc0c-135">说明</span><span class="sxs-lookup"><span data-stu-id="4dc0c-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4dc0c-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="4dc0c-136">Authorization</span></span>  | <span data-ttu-id="4dc0c-137">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4dc0c-137">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4dc0c-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="4dc0c-138">Request body</span></span>
<span data-ttu-id="4dc0c-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4dc0c-140">响应</span><span class="sxs-lookup"><span data-stu-id="4dc0c-140">Response</span></span>
<span data-ttu-id="4dc0c-141">如果成功，此方法在`200, OK`响应正文中返回响应代码和[bookingAppointment](../resources/bookingappointment.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-141">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4dc0c-142">示例</span><span class="sxs-lookup"><span data-stu-id="4dc0c-142">Example</span></span>
<span data-ttu-id="4dc0c-143">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-143">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4dc0c-144">请求</span><span class="sxs-lookup"><span data-stu-id="4dc0c-144">Request</span></span>
<span data-ttu-id="4dc0c-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4dc0c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="4dc0c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="4dc0c-147">C#</span><span class="sxs-lookup"><span data-stu-id="4dc0c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-getcalendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4dc0c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4dc0c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-getcalendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4dc0c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4dc0c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-getcalendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4dc0c-150">响应</span><span class="sxs-lookup"><span data-stu-id="4dc0c-150">Response</span></span>
<span data-ttu-id="4dc0c-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-151">The following is an example of the response.</span></span> <span data-ttu-id="4dc0c-152">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4dc0c-153">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4dc0c-153">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/calendarView",
    "value": [
        {
            "id": "AAMkADKpAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "customerId": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "customerName": "Adele Vance",
            "customerEmailAddress": "adelev@proseware.com",
            "customerPhone": "213-555-0156",
            "customerNotes": null,
            "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "serviceName": "Catered bento",
            "duration": "PT30M",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "priceType": "fixedPrice",
            "price": 10,
            "serviceNotes": null,
            "optOutOfCustomerEmail": false,
            "staffMemberIds": [],
            "invoiceAmount": 10,
            "invoiceId": "1003",
            "invoiceStatus": "open",
            "invoiceUrl": "theInvoiceUrl",
            "customerLocation": {
                "displayName": "Customer",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "",
                    "city": "",
                    "state": "",
                    "countryOrRegion": "",
                    "postalCode": ""
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "start": {
                "dateTime": "2018-05-05T12:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-05-05T12:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (876 Tenth Avenue, Buffalo, NY 98052, USA)",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "",
                    "city": "",
                    "state": "",
                    "countryOrRegion": "",
                    "postalCode": ""
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-05-05T12:30:00.0000000Z",
                "timeZone": "UTC"
            }
        },
        {
            "id": "AAMkADKnAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "customerId": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "customerName": "Jordan Miller",
            "customerEmailAddress": "jordanm@contoso.com",
            "customerPhone": "213-555-0199",
            "customerNotes": null,
            "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "serviceName": "Catered bento",
            "duration": "PT30M",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "priceType": "fixedPrice",
            "price": 10,
            "serviceNotes": null,
            "optOutOfCustomerEmail": false,
            "staffMemberIds": [],
            "invoiceAmount": 10,
            "invoiceId": "1001",
            "invoiceStatus": "open",
            "invoiceUrl": "theInvoiceUrl",
            "customerLocation": {
                "displayName": "Customer",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "",
                    "city": "",
                    "state": "",
                    "countryOrRegion": "",
                    "postalCode": ""
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "start": {
                "dateTime": "2018-05-06T12:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-05-06T12:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (123 First Avenue, Buffalo, NY 98052, USA)",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "",
                    "city": "",
                    "state": "",
                    "countryOrRegion": "",
                    "postalCode": ""
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-05-06T12:30:00.0000000Z",
                "timeZone": "UTC"
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
  "description": "bookingBusiness: getCalendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
