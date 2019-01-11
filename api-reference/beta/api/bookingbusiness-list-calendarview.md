---
title: 列表的预定 calendarView
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 5abf88b4d0f0f5721ba3bcbf467406cfedfbe9f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809462"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="1579c-104">列表的预定 calendarView</span><span class="sxs-lookup"><span data-stu-id="1579c-104">List Bookings calendarView</span></span>

 > <span data-ttu-id="1579c-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1579c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1579c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1579c-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="1579c-107">获得[bookingBusiness](../resources/bookingbusiness.md)，在指定的日期范围中出现[bookingAppointment](../resources/bookingappointment.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="1579c-107">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="1579c-108">权限</span><span class="sxs-lookup"><span data-stu-id="1579c-108">Permissions</span></span>
<span data-ttu-id="1579c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1579c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1579c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1579c-111">Permission type</span></span>      | <span data-ttu-id="1579c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1579c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1579c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1579c-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="1579c-114">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="1579c-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1579c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1579c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1579c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1579c-116">Not supported.</span></span>   |
|<span data-ttu-id="1579c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1579c-117">Application</span></span> | <span data-ttu-id="1579c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1579c-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="1579c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1579c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}

```
## <a name="request-headers"></a><span data-ttu-id="1579c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1579c-120">Request headers</span></span>
| <span data-ttu-id="1579c-121">名称</span><span class="sxs-lookup"><span data-stu-id="1579c-121">Name</span></span>       | <span data-ttu-id="1579c-122">说明</span><span class="sxs-lookup"><span data-stu-id="1579c-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1579c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1579c-123">Authorization</span></span>  | <span data-ttu-id="1579c-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1579c-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1579c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1579c-125">Request body</span></span>
<span data-ttu-id="1579c-126">在请求 URL 中，提供以下查询参数（含值）。</span><span class="sxs-lookup"><span data-stu-id="1579c-126">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="1579c-127">参数</span><span class="sxs-lookup"><span data-stu-id="1579c-127">Parameter</span></span>    | <span data-ttu-id="1579c-128">类型</span><span class="sxs-lookup"><span data-stu-id="1579c-128">Type</span></span>   |<span data-ttu-id="1579c-129">Description</span><span class="sxs-lookup"><span data-stu-id="1579c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1579c-130">start</span><span class="sxs-lookup"><span data-stu-id="1579c-130">start</span></span>|<span data-ttu-id="1579c-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1579c-131">DateTimeOffset</span></span>|<span data-ttu-id="1579c-132">开始日期和时间的时间范围，表示以 ISO 8601 格式，为 UTC 或从 UTC 偏移量。</span><span class="sxs-lookup"><span data-stu-id="1579c-132">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="1579c-133">例如，午夜 UTC 2018 Jan 1，如下所示:"2018年-01-01T00:00:00Z'，和 PST 的同一时间将如下所示:"2017年-12-31T16:00:00-08:00。</span><span class="sxs-lookup"><span data-stu-id="1579c-133">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="1579c-134">end</span><span class="sxs-lookup"><span data-stu-id="1579c-134">end</span></span>|<span data-ttu-id="1579c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1579c-135">DateTimeOffset</span></span>|<span data-ttu-id="1579c-136">结束日期和时间的时间范围，表示 ISO 8601 格式，为 UTC 或从 UTC 偏移量。</span><span class="sxs-lookup"><span data-stu-id="1579c-136">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="1579c-137">例如，3 am UTC 上 2018 Jan 1，如下所示:"2018年-01-01T03:00:00Z'，和 PST 的同一时间将如下所示:"2017年-12-31T19:00:00-08:00。</span><span class="sxs-lookup"><span data-stu-id="1579c-137">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

## <a name="response"></a><span data-ttu-id="1579c-138">响应</span><span class="sxs-lookup"><span data-stu-id="1579c-138">Response</span></span>
<span data-ttu-id="1579c-139">如果成功，此方法返回`200, OK`响应正文中的响应代码和[bookingAppointment](../resources/bookingappointment.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="1579c-139">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1579c-140">示例</span><span class="sxs-lookup"><span data-stu-id="1579c-140">Example</span></span>
<span data-ttu-id="1579c-141">下面的示例展示了如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="1579c-141">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1579c-142">请求</span><span class="sxs-lookup"><span data-stu-id="1579c-142">Request</span></span>
<span data-ttu-id="1579c-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1579c-143">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```

##### <a name="response"></a><span data-ttu-id="1579c-144">响应</span><span class="sxs-lookup"><span data-stu-id="1579c-144">Response</span></span>
<span data-ttu-id="1579c-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1579c-145">The following is an example of the response.</span></span> <span data-ttu-id="1579c-146">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1579c-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1579c-147">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1579c-147">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "bookingBusiness: getCalendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
