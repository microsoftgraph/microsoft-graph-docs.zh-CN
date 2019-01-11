---
title: 列表约会
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
ms.openlocfilehash: 920a0d53635e5d017ecd51ee75d3b244aafcb802
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839009"
---
# <a name="list-appointments"></a><span data-ttu-id="c32bb-104">列表约会</span><span class="sxs-lookup"><span data-stu-id="c32bb-104">List appointments</span></span>

 > <span data-ttu-id="c32bb-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c32bb-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c32bb-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c32bb-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="c32bb-107">获取指定[bookingbusiness](../resources/bookingbusiness.md) [bookingAppointment](../resources/bookingappointment.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c32bb-107">Get a list of [bookingAppointment](../resources/bookingappointment.md) objects for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c32bb-108">权限</span><span class="sxs-lookup"><span data-stu-id="c32bb-108">Permissions</span></span>
<span data-ttu-id="c32bb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c32bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c32bb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c32bb-111">Permission type</span></span>      | <span data-ttu-id="c32bb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c32bb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c32bb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c32bb-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c32bb-114">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c32bb-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c32bb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c32bb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c32bb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c32bb-116">Not supported.</span></span>   |
|<span data-ttu-id="c32bb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c32bb-117">Application</span></span> | <span data-ttu-id="c32bb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c32bb-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="c32bb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c32bb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c32bb-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c32bb-120">Optional query parameters</span></span>
<span data-ttu-id="c32bb-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c32bb-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c32bb-122">要获取一组约会的预订企业内的日期范围，而不是`$filter`，该日期范围内的[获取 calendarView](bookingbusiness-list-calendarview.md) 。</span><span class="sxs-lookup"><span data-stu-id="c32bb-122">To get the set of appointments of a Bookings business within a date range, instead of `$filter`, [get the calendarView](bookingbusiness-list-calendarview.md) for that date range.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="c32bb-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c32bb-123">Request headers</span></span>
| <span data-ttu-id="c32bb-124">名称</span><span class="sxs-lookup"><span data-stu-id="c32bb-124">Name</span></span>      |<span data-ttu-id="c32bb-125">说明</span><span class="sxs-lookup"><span data-stu-id="c32bb-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c32bb-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c32bb-126">Authorization</span></span>  | <span data-ttu-id="c32bb-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c32bb-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c32bb-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c32bb-128">Request body</span></span>
<span data-ttu-id="c32bb-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c32bb-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c32bb-130">响应</span><span class="sxs-lookup"><span data-stu-id="c32bb-130">Response</span></span>
<span data-ttu-id="c32bb-131">如果成功，此方法返回`200 OK`响应代码和响应正文中的[bookingAppointment](../resources/bookingappointment.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c32bb-131">If successful, this method returns a `200 OK` response code and collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c32bb-132">示例</span><span class="sxs-lookup"><span data-stu-id="c32bb-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c32bb-133">请求</span><span class="sxs-lookup"><span data-stu-id="c32bb-133">Request</span></span>
<span data-ttu-id="c32bb-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c32bb-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appointments"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
```
##### <a name="response"></a><span data-ttu-id="c32bb-135">响应</span><span class="sxs-lookup"><span data-stu-id="c32bb-135">Response</span></span>
<span data-ttu-id="c32bb-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c32bb-136">The following is an example of the response.</span></span> <span data-ttu-id="c32bb-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c32bb-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c32bb-138">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c32bb-138">All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments",
    "value": [
        {
            "id": "AAMkADKoAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "customerId": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "customerName": "Bob Kelly",
            "customerEmailAddress": "bobk@tailspintoys.com",
            "customerPhone": "213-555-0108",
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
            "invoiceId": "1002",
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
                "dateTime": "2018-04-30T13:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-04-30T13:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (987 Third Avenue, Buffalo, NY 98052, USA)",
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
                "dateTime": "2018-04-30T13:30:00.0000000Z",
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
                "dateTime": "2018-05-01T12:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-05-01T12:30:00.0000000Z",
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
                "dateTime": "2018-05-01T12:30:00.0000000Z",
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
  "description": "List appointments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
