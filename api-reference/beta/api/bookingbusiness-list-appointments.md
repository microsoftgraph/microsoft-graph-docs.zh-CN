---
title: 列出约会
description: 获取指定 bookingbusiness 的 bookingAppointment 对象的列表。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 2f2f1b20506cfb6f01b81a1d259551135e227b88
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258175"
---
# <a name="list-appointments"></a><span data-ttu-id="6d172-103">列出约会</span><span class="sxs-lookup"><span data-stu-id="6d172-103">List appointments</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d172-104">获取指定[bookingbusiness](../resources/bookingbusiness.md)的[bookingAppointment](../resources/bookingappointment.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="6d172-104">Get a list of [bookingAppointment](../resources/bookingappointment.md) objects for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="6d172-105">权限</span><span class="sxs-lookup"><span data-stu-id="6d172-105">Permissions</span></span>
<span data-ttu-id="6d172-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d172-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d172-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d172-108">Permission type</span></span>      | <span data-ttu-id="6d172-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d172-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d172-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d172-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="6d172-111">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="6d172-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="6d172-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d172-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d172-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d172-113">Not supported.</span></span>   |
|<span data-ttu-id="6d172-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d172-114">Application</span></span> | <span data-ttu-id="6d172-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d172-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6d172-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d172-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6d172-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6d172-117">Optional query parameters</span></span>
<span data-ttu-id="6d172-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6d172-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="6d172-119">若要在日期范围内 (而不是`$filter`) 获取预订业务的约会集, 请在该日期范围内[获取 calendarView](bookingbusiness-list-calendarview.md) 。</span><span class="sxs-lookup"><span data-stu-id="6d172-119">To get the set of appointments of a Bookings business within a date range, instead of `$filter`, [get the calendarView](bookingbusiness-list-calendarview.md) for that date range.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6d172-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d172-120">Request headers</span></span>
| <span data-ttu-id="6d172-121">名称</span><span class="sxs-lookup"><span data-stu-id="6d172-121">Name</span></span>      |<span data-ttu-id="6d172-122">说明</span><span class="sxs-lookup"><span data-stu-id="6d172-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6d172-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d172-123">Authorization</span></span>  | <span data-ttu-id="6d172-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="6d172-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d172-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d172-125">Request body</span></span>
<span data-ttu-id="6d172-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6d172-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="6d172-127">响应</span><span class="sxs-lookup"><span data-stu-id="6d172-127">Response</span></span>
<span data-ttu-id="6d172-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[bookingAppointment](../resources/bookingappointment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="6d172-128">If successful, this method returns a `200 OK` response code and collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6d172-129">示例</span><span class="sxs-lookup"><span data-stu-id="6d172-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6d172-130">请求</span><span class="sxs-lookup"><span data-stu-id="6d172-130">Request</span></span>
<span data-ttu-id="6d172-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6d172-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appointments"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
```
##### <a name="response"></a><span data-ttu-id="6d172-132">响应</span><span class="sxs-lookup"><span data-stu-id="6d172-132">Response</span></span>
<span data-ttu-id="6d172-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6d172-133">The following is an example of the response.</span></span> <span data-ttu-id="6d172-134">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6d172-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6d172-135">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6d172-135">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6d172-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="6d172-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6d172-137">C#</span><span class="sxs-lookup"><span data-stu-id="6d172-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_appointments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d172-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="6d172-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_appointments-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6d172-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="6d172-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_appointments-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-list-appointments.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-list-appointments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-list-appointments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
