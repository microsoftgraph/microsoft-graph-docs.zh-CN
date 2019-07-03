---
title: 列出约会
description: 获取指定 bookingbusiness 的 bookingAppointment 对象的列表。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: fceed2834463497291e6c3bc661b237562da76ef
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439313"
---
# <a name="list-appointments"></a><span data-ttu-id="a116e-103">列出约会</span><span class="sxs-lookup"><span data-stu-id="a116e-103">List appointments</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a116e-104">获取指定[bookingbusiness](../resources/bookingbusiness.md)的[bookingAppointment](../resources/bookingappointment.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a116e-104">Get a list of [bookingAppointment](../resources/bookingappointment.md) objects for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a116e-105">权限</span><span class="sxs-lookup"><span data-stu-id="a116e-105">Permissions</span></span>
<span data-ttu-id="a116e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a116e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a116e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a116e-108">Permission type</span></span>      | <span data-ttu-id="a116e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a116e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a116e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a116e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a116e-111">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="a116e-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a116e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a116e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a116e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a116e-113">Not supported.</span></span>   |
|<span data-ttu-id="a116e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a116e-114">Application</span></span> | <span data-ttu-id="a116e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a116e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a116e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a116e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a116e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a116e-117">Optional query parameters</span></span>
<span data-ttu-id="a116e-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a116e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a116e-119">若要在日期范围内 (而不是`$filter`) 获取预订业务的约会集, 请在该日期范围内[获取 calendarView](bookingbusiness-list-calendarview.md) 。</span><span class="sxs-lookup"><span data-stu-id="a116e-119">To get the set of appointments of a Bookings business within a date range, instead of `$filter`, [get the calendarView](bookingbusiness-list-calendarview.md) for that date range.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a116e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a116e-120">Request headers</span></span>
| <span data-ttu-id="a116e-121">名称</span><span class="sxs-lookup"><span data-stu-id="a116e-121">Name</span></span>      |<span data-ttu-id="a116e-122">说明</span><span class="sxs-lookup"><span data-stu-id="a116e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a116e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a116e-123">Authorization</span></span>  | <span data-ttu-id="a116e-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a116e-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a116e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a116e-125">Request body</span></span>
<span data-ttu-id="a116e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a116e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a116e-127">响应</span><span class="sxs-lookup"><span data-stu-id="a116e-127">Response</span></span>
<span data-ttu-id="a116e-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[bookingAppointment](../resources/bookingappointment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="a116e-128">If successful, this method returns a `200 OK` response code and collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a116e-129">示例</span><span class="sxs-lookup"><span data-stu-id="a116e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a116e-130">请求</span><span class="sxs-lookup"><span data-stu-id="a116e-130">Request</span></span>
<span data-ttu-id="a116e-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a116e-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a116e-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a116e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appointments"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a116e-133">C#</span><span class="sxs-lookup"><span data-stu-id="a116e-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appointments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a116e-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="a116e-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appointments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a116e-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="a116e-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appointments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a116e-136">响应</span><span class="sxs-lookup"><span data-stu-id="a116e-136">Response</span></span>
<span data-ttu-id="a116e-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a116e-137">The following is an example of the response.</span></span> <span data-ttu-id="a116e-138">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a116e-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a116e-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a116e-139">All of the properties will be returned from an actual call.</span></span>
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
