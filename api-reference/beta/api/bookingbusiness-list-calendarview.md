---
title: 列出 Bookings 日历视图
description: 获取 bookingBusiness 的 bookingAppointment 对象的集合, 该集合在指定的日期范围内发生。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 95a72cacef1ca2c52f0bf6c80b9428eeb99f5d19
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439285"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="faf6f-103">列出 Bookings 日历视图</span><span class="sxs-lookup"><span data-stu-id="faf6f-103">List Bookings calendarView</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="faf6f-104">获取[bookingBusiness](../resources/bookingbusiness.md)的[bookingAppointment](../resources/bookingappointment.md)对象的集合, 该集合在指定的日期范围内发生。</span><span class="sxs-lookup"><span data-stu-id="faf6f-104">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="faf6f-105">权限</span><span class="sxs-lookup"><span data-stu-id="faf6f-105">Permissions</span></span>
<span data-ttu-id="faf6f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="faf6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="faf6f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="faf6f-108">Permission type</span></span>      | <span data-ttu-id="faf6f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="faf6f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="faf6f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="faf6f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="faf6f-111">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="faf6f-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="faf6f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="faf6f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="faf6f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="faf6f-113">Not supported.</span></span>   |
|<span data-ttu-id="faf6f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="faf6f-114">Application</span></span> | <span data-ttu-id="faf6f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="faf6f-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="faf6f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="faf6f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}

```
## <a name="request-headers"></a><span data-ttu-id="faf6f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="faf6f-117">Request headers</span></span>
| <span data-ttu-id="faf6f-118">名称</span><span class="sxs-lookup"><span data-stu-id="faf6f-118">Name</span></span>       | <span data-ttu-id="faf6f-119">说明</span><span class="sxs-lookup"><span data-stu-id="faf6f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="faf6f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="faf6f-120">Authorization</span></span>  | <span data-ttu-id="faf6f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="faf6f-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="faf6f-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="faf6f-122">Request body</span></span>
<span data-ttu-id="faf6f-123">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="faf6f-123">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="faf6f-124">参数</span><span class="sxs-lookup"><span data-stu-id="faf6f-124">Parameter</span></span>    | <span data-ttu-id="faf6f-125">类型</span><span class="sxs-lookup"><span data-stu-id="faf6f-125">Type</span></span>   |<span data-ttu-id="faf6f-126">说明</span><span class="sxs-lookup"><span data-stu-id="faf6f-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="faf6f-127">start</span><span class="sxs-lookup"><span data-stu-id="faf6f-127">start</span></span>|<span data-ttu-id="faf6f-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faf6f-128">DateTimeOffset</span></span>|<span data-ttu-id="faf6f-129">时间范围的开始日期和时间, 以 ISO 8601 格式表示, 如 UTC 或 UTC 时差。</span><span class="sxs-lookup"><span data-stu-id="faf6f-129">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="faf6f-130">例如, 2018 年1月1日午夜 UTC 将如下所示: ' 2018-01-01T00:00: 00Z ', PST 的相同时间如下所示: ' 2017-12-31T16:00:00-08:00 '。</span><span class="sxs-lookup"><span data-stu-id="faf6f-130">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="faf6f-131">end</span><span class="sxs-lookup"><span data-stu-id="faf6f-131">end</span></span>|<span data-ttu-id="faf6f-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="faf6f-132">DateTimeOffset</span></span>|<span data-ttu-id="faf6f-133">时间范围的结束日期和时间, 以 ISO 8601 格式表示, 即 UTC 或 UTC 时差。</span><span class="sxs-lookup"><span data-stu-id="faf6f-133">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="faf6f-134">例如, 2018 年1月1日的 3am UTC 如下所示: ' 2018-01-01T03:00: 00Z ', PST 中的相同时间如下所示: ' 2017-12-31T19:00:00-08:00 '。</span><span class="sxs-lookup"><span data-stu-id="faf6f-134">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

## <a name="response"></a><span data-ttu-id="faf6f-135">响应</span><span class="sxs-lookup"><span data-stu-id="faf6f-135">Response</span></span>
<span data-ttu-id="faf6f-136">如果成功, 此方法在`200, OK`响应正文中返回响应代码和[bookingAppointment](../resources/bookingappointment.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="faf6f-136">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faf6f-137">示例</span><span class="sxs-lookup"><span data-stu-id="faf6f-137">Example</span></span>
<span data-ttu-id="faf6f-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="faf6f-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="faf6f-139">请求</span><span class="sxs-lookup"><span data-stu-id="faf6f-139">Request</span></span>
<span data-ttu-id="faf6f-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="faf6f-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="faf6f-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="faf6f-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="faf6f-142">C#</span><span class="sxs-lookup"><span data-stu-id="faf6f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-getcalendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="faf6f-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="faf6f-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-getcalendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="faf6f-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="faf6f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-getcalendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="faf6f-145">响应</span><span class="sxs-lookup"><span data-stu-id="faf6f-145">Response</span></span>
<span data-ttu-id="faf6f-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="faf6f-146">The following is an example of the response.</span></span> <span data-ttu-id="faf6f-147">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="faf6f-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="faf6f-148">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="faf6f-148">All of the properties will be returned from an actual call.</span></span>
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
