---
title: 获取 bookingAppointment
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b97c1fc6b45a9380fa3fb37e092a2a11ac3437a5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951304"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="92595-104">获取 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="92595-104">Get bookingAppointment</span></span>

 > <span data-ttu-id="92595-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="92595-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="92595-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="92595-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="92595-107">指定[bookingbusiness](../resources/bookingbusiness.md)中获取的属性和[bookingAppointment](../resources/bookingappointment.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="92595-107">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="92595-108">采用 UTC 始终返回**start**和**end**属性。</span><span class="sxs-lookup"><span data-stu-id="92595-108">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="92595-109">权限</span><span class="sxs-lookup"><span data-stu-id="92595-109">Permissions</span></span>
<span data-ttu-id="92595-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92595-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92595-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="92595-112">Permission type</span></span>      | <span data-ttu-id="92595-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92595-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92595-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92595-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="92595-115">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="92595-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="92595-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92595-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92595-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="92595-117">Not supported.</span></span>   |
|<span data-ttu-id="92595-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="92595-118">Application</span></span> | <span data-ttu-id="92595-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="92595-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="92595-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92595-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="92595-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="92595-121">Optional query parameters</span></span>
<span data-ttu-id="92595-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="92595-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="92595-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="92595-123">Request headers</span></span>
| <span data-ttu-id="92595-124">名称</span><span class="sxs-lookup"><span data-stu-id="92595-124">Name</span></span>      |<span data-ttu-id="92595-125">说明</span><span class="sxs-lookup"><span data-stu-id="92595-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="92595-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="92595-126">Authorization</span></span>  | <span data-ttu-id="92595-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="92595-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="92595-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="92595-128">Request body</span></span>
<span data-ttu-id="92595-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="92595-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="92595-130">响应</span><span class="sxs-lookup"><span data-stu-id="92595-130">Response</span></span>
<span data-ttu-id="92595-131">如果成功，此方法返回`200 OK`响应正文中的响应代码和[bookingAppointment](../resources/bookingappointment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="92595-131">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="92595-132">示例</span><span class="sxs-lookup"><span data-stu-id="92595-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92595-133">请求</span><span class="sxs-lookup"><span data-stu-id="92595-133">Request</span></span>
<span data-ttu-id="92595-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="92595-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
##### <a name="response"></a><span data-ttu-id="92595-135">响应</span><span class="sxs-lookup"><span data-stu-id="92595-135">Response</span></span>
<span data-ttu-id="92595-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="92595-136">The following is an example of the response.</span></span> <span data-ttu-id="92595-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="92595-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="92595-138">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92595-138">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
