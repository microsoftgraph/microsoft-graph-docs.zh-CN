---
title: 列出 Bookings 日历视图
description: 获取 bookingBusiness 的 bookingAppointment 对象的集合，该集合发生在指定的日期范围内。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d96e5b2f2c7f435a0ea8dcd39a4b58ae7657c222
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047908"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="ea9a8-103">列出 Bookings 日历视图</span><span class="sxs-lookup"><span data-stu-id="ea9a8-103">List Bookings calendarView</span></span>

<span data-ttu-id="ea9a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea9a8-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea9a8-105">获取[bookingBusiness](../resources/bookingbusiness.md)的[bookingAppointment](../resources/bookingappointment.md)对象的集合，该集合发生在指定的日期范围内。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-105">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea9a8-106">权限</span><span class="sxs-lookup"><span data-stu-id="ea9a8-106">Permissions</span></span>
<span data-ttu-id="ea9a8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea9a8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea9a8-109">Permission type</span></span>      | <span data-ttu-id="ea9a8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea9a8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea9a8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea9a8-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="ea9a8-112">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ea9a8-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ea9a8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea9a8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea9a8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-114">Not supported.</span></span>   |
|<span data-ttu-id="ea9a8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea9a8-115">Application</span></span> | <span data-ttu-id="ea9a8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ea9a8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea9a8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}
```

## <a name="query-parameters"></a><span data-ttu-id="ea9a8-118">查询参数</span><span class="sxs-lookup"><span data-stu-id="ea9a8-118">Query parameters</span></span>

<span data-ttu-id="ea9a8-119">在请求 URL 中，提供以下必要查询参数的值。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="ea9a8-120">参数</span><span class="sxs-lookup"><span data-stu-id="ea9a8-120">Parameter</span></span>    | <span data-ttu-id="ea9a8-121">类型</span><span class="sxs-lookup"><span data-stu-id="ea9a8-121">Type</span></span>   |<span data-ttu-id="ea9a8-122">说明</span><span class="sxs-lookup"><span data-stu-id="ea9a8-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea9a8-123">start</span><span class="sxs-lookup"><span data-stu-id="ea9a8-123">start</span></span>|<span data-ttu-id="ea9a8-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea9a8-124">DateTimeOffset</span></span>|<span data-ttu-id="ea9a8-125">一个时间范围的开始日期和时间，以 ISO 8601 格式表示，为 UTC 或与 UTC 的时差。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-125">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="ea9a8-126">例如，2018 年 1 月 1 日午夜 UTC 如下所示："2018-01-01T00：00：00Z"，PST 中的同一时间如下所示："2017-12-31T16：00：00-08：00"。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-126">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="ea9a8-127">end</span><span class="sxs-lookup"><span data-stu-id="ea9a8-127">end</span></span>|<span data-ttu-id="ea9a8-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea9a8-128">DateTimeOffset</span></span>|<span data-ttu-id="ea9a8-129">一个时间范围的结束日期和时间，以 ISO 8601 格式表示，采用 UTC 格式或与 UTC 的偏移量。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-129">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="ea9a8-130">例如，2018 年 1 月 1 日上午 3 点 UTC 如下所示："2018-01-01T03：00：00Z"，PST 中的同一时间如下所示："2017-12-31T19：00：00-08：00"。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-130">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

<span data-ttu-id="ea9a8-131">和 的值使用其相应值中指定的时区偏移量进行解释，如果存在，则不会影响 `start` `end` `Prefer: outlook.timezone` 标头的值。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-131">The values of `start` and `end` are interpreted using the timezone offset specified in their corresponding values and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span>

<span data-ttu-id="ea9a8-132">此方法还支持一些 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-132">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea9a8-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea9a8-133">Request headers</span></span>
| <span data-ttu-id="ea9a8-134">名称</span><span class="sxs-lookup"><span data-stu-id="ea9a8-134">Name</span></span>       | <span data-ttu-id="ea9a8-135">说明</span><span class="sxs-lookup"><span data-stu-id="ea9a8-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ea9a8-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea9a8-136">Authorization</span></span>  | <span data-ttu-id="ea9a8-137">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ea9a8-137">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea9a8-138">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea9a8-138">Request body</span></span>
<span data-ttu-id="ea9a8-139">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea9a8-140">响应</span><span class="sxs-lookup"><span data-stu-id="ea9a8-140">Response</span></span>
<span data-ttu-id="ea9a8-141">如果成功，此方法在 `200, OK` 响应正文中返回 响应代码和 [bookingAppointment](../resources/bookingappointment.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-141">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea9a8-142">示例</span><span class="sxs-lookup"><span data-stu-id="ea9a8-142">Example</span></span>
<span data-ttu-id="ea9a8-143">下面是如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-143">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ea9a8-144">请求</span><span class="sxs-lookup"><span data-stu-id="ea9a8-144">Request</span></span>
<span data-ttu-id="ea9a8-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ea9a8-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="ea9a8-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="ea9a8-147">C#</span><span class="sxs-lookup"><span data-stu-id="ea9a8-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-getcalendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ea9a8-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ea9a8-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-getcalendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ea9a8-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ea9a8-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-getcalendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ea9a8-150">Java</span><span class="sxs-lookup"><span data-stu-id="ea9a8-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-getcalendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ea9a8-151">响应</span><span class="sxs-lookup"><span data-stu-id="ea9a8-151">Response</span></span>
<span data-ttu-id="ea9a8-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-152">The following is an example of the response.</span></span> <span data-ttu-id="ea9a8-153">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ea9a8-153">Note: The response object shown here might be shortened for readability.</span></span>
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
