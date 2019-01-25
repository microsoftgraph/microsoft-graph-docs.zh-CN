---
title: 获取 bookingAppointment
description: 指定 bookingbusiness 中获取的属性和 bookingAppointment 对象的关系。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: e9e9fffa3101656d4e426578185683065b4f5e5a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525267"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="ec48b-103">获取 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="ec48b-103">Get bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec48b-104">指定[bookingbusiness](../resources/bookingbusiness.md)中获取的属性和[bookingAppointment](../resources/bookingappointment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="ec48b-104">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="ec48b-105">采用 UTC 始终返回**start**和**end**属性。</span><span class="sxs-lookup"><span data-stu-id="ec48b-105">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec48b-106">权限</span><span class="sxs-lookup"><span data-stu-id="ec48b-106">Permissions</span></span>
<span data-ttu-id="ec48b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec48b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec48b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec48b-109">Permission type</span></span>      | <span data-ttu-id="ec48b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec48b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec48b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec48b-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="ec48b-112">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ec48b-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ec48b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec48b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec48b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec48b-114">Not supported.</span></span>   |
|<span data-ttu-id="ec48b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec48b-115">Application</span></span> | <span data-ttu-id="ec48b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec48b-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="ec48b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec48b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec48b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ec48b-118">Optional query parameters</span></span>
<span data-ttu-id="ec48b-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ec48b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec48b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec48b-120">Request headers</span></span>
| <span data-ttu-id="ec48b-121">名称</span><span class="sxs-lookup"><span data-stu-id="ec48b-121">Name</span></span>      |<span data-ttu-id="ec48b-122">说明</span><span class="sxs-lookup"><span data-stu-id="ec48b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec48b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec48b-123">Authorization</span></span>  | <span data-ttu-id="ec48b-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ec48b-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec48b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec48b-125">Request body</span></span>
<span data-ttu-id="ec48b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec48b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ec48b-127">响应</span><span class="sxs-lookup"><span data-stu-id="ec48b-127">Response</span></span>
<span data-ttu-id="ec48b-128">如果成功，此方法返回`200 OK`响应正文中的响应代码和[bookingAppointment](../resources/bookingappointment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ec48b-128">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ec48b-129">示例</span><span class="sxs-lookup"><span data-stu-id="ec48b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec48b-130">请求</span><span class="sxs-lookup"><span data-stu-id="ec48b-130">Request</span></span>
<span data-ttu-id="ec48b-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ec48b-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
##### <a name="response"></a><span data-ttu-id="ec48b-132">响应</span><span class="sxs-lookup"><span data-stu-id="ec48b-132">Response</span></span>
<span data-ttu-id="ec48b-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ec48b-133">The following is an example of the response.</span></span> <span data-ttu-id="ec48b-134">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ec48b-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ec48b-135">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec48b-135">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments/$entity",
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
    "serviceNotes": "Customer requires punctual service.",
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
    "reminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "This service is tomorrow"
        },
        {
            "offset": "PT1H",
            "recipients": "customer",
            "message": "Please be available to enjoy your lunch service."
        },
        {
            "offset": "PT2H",
            "recipients": "staff",
            "message": "Please check traffic for next cater."
        }
    ],
    "invoiceDate": {
        "dateTime": "2018-05-06T12:30:00.0000000Z",
        "timeZone": "UTC"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
