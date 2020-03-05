---
title: 列出约会
description: 获取指定 bookingbusiness 的 bookingAppointment 对象的列表。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 1cc6fcf3889ffca8bdf6f41f14533487f96db798
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441268"
---
# <a name="list-appointments"></a><span data-ttu-id="d61d5-103">列出约会</span><span class="sxs-lookup"><span data-stu-id="d61d5-103">List appointments</span></span>

<span data-ttu-id="d61d5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d61d5-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d61d5-105">获取指定[bookingbusiness](../resources/bookingbusiness.md)的[bookingAppointment](../resources/bookingappointment.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d61d5-105">Get a list of [bookingAppointment](../resources/bookingappointment.md) objects for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d61d5-106">权限</span><span class="sxs-lookup"><span data-stu-id="d61d5-106">Permissions</span></span>
<span data-ttu-id="d61d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d61d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d61d5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d61d5-109">Permission type</span></span>      | <span data-ttu-id="d61d5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d61d5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d61d5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d61d5-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="d61d5-112">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="d61d5-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d61d5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d61d5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d61d5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d61d5-114">Not supported.</span></span>   |
|<span data-ttu-id="d61d5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d61d5-115">Application</span></span> | <span data-ttu-id="d61d5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d61d5-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d61d5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d61d5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d61d5-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d61d5-118">Optional query parameters</span></span>
<span data-ttu-id="d61d5-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d61d5-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d61d5-120">若要在日期范围内（而不是`$filter`）获取预订业务的约会集，请在该日期范围内[获取 calendarView](bookingbusiness-list-calendarview.md) 。</span><span class="sxs-lookup"><span data-stu-id="d61d5-120">To get the set of appointments of a Bookings business within a date range, instead of `$filter`, [get the calendarView](bookingbusiness-list-calendarview.md) for that date range.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d61d5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d61d5-121">Request headers</span></span>
| <span data-ttu-id="d61d5-122">名称</span><span class="sxs-lookup"><span data-stu-id="d61d5-122">Name</span></span>      |<span data-ttu-id="d61d5-123">说明</span><span class="sxs-lookup"><span data-stu-id="d61d5-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d61d5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d61d5-124">Authorization</span></span>  | <span data-ttu-id="d61d5-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d61d5-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d61d5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d61d5-126">Request body</span></span>
<span data-ttu-id="d61d5-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d61d5-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d61d5-128">响应</span><span class="sxs-lookup"><span data-stu-id="d61d5-128">Response</span></span>
<span data-ttu-id="d61d5-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[bookingAppointment](../resources/bookingappointment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d61d5-129">If successful, this method returns a `200 OK` response code and collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d61d5-130">示例</span><span class="sxs-lookup"><span data-stu-id="d61d5-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d61d5-131">请求</span><span class="sxs-lookup"><span data-stu-id="d61d5-131">Request</span></span>
<span data-ttu-id="d61d5-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d61d5-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d61d5-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d61d5-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appointments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
```
# <a name="c"></a>[<span data-ttu-id="d61d5-134">C#</span><span class="sxs-lookup"><span data-stu-id="d61d5-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appointments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d61d5-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d61d5-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appointments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d61d5-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d61d5-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appointments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d61d5-137">响应</span><span class="sxs-lookup"><span data-stu-id="d61d5-137">Response</span></span>
<span data-ttu-id="d61d5-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d61d5-138">The following is an example of the response.</span></span> <span data-ttu-id="d61d5-139">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d61d5-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d61d5-140">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d61d5-140">All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List appointments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
