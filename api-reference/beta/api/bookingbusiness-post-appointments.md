---
title: 创建 bookingAppointment
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: 436e0121a36fbc0dd0bf0d7cd3302d7999776d9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043676"
---
# <a name="create-bookingappointment"></a><span data-ttu-id="9dc9d-104">创建 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="9dc9d-104">Create bookingAppointment</span></span>

 > <span data-ttu-id="9dc9d-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9dc9d-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="9dc9d-107">创建新[bookingAppointment](../resources/bookingappointment.md)的指定[bookingbusiness](../resources/bookingbusiness.md)。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-107">Create a new [bookingAppointment](../resources/bookingappointment.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="9dc9d-108">权限</span><span class="sxs-lookup"><span data-stu-id="9dc9d-108">Permissions</span></span>
<span data-ttu-id="9dc9d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9dc9d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9dc9d-111">Permission type</span></span>      | <span data-ttu-id="9dc9d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9dc9d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dc9d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9dc9d-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="9dc9d-114">BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All，Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="9dc9d-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9dc9d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9dc9d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dc9d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-116">Not supported.</span></span>   |
|<span data-ttu-id="9dc9d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9dc9d-117">Application</span></span> | <span data-ttu-id="9dc9d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="9dc9d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9dc9d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments

```
## <a name="request-headers"></a><span data-ttu-id="9dc9d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9dc9d-120">Request headers</span></span>
| <span data-ttu-id="9dc9d-121">名称</span><span class="sxs-lookup"><span data-stu-id="9dc9d-121">Name</span></span>       | <span data-ttu-id="9dc9d-122">说明</span><span class="sxs-lookup"><span data-stu-id="9dc9d-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9dc9d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9dc9d-123">Authorization</span></span>  | <span data-ttu-id="9dc9d-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9dc9d-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9dc9d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9dc9d-125">Request body</span></span>
<span data-ttu-id="9dc9d-126">在请求正文中，提供[bookingAppointment](../resources/bookingappointment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-126">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="9dc9d-127">响应</span><span class="sxs-lookup"><span data-stu-id="9dc9d-127">Response</span></span>
<span data-ttu-id="9dc9d-128">如果成功，此方法返回`201, Created`响应正文中的响应代码和[bookingAppointment](../resources/bookingappointment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-128">If successful, this method returns `201, Created` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dc9d-129">示例</span><span class="sxs-lookup"><span data-stu-id="9dc9d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9dc9d-130">请求</span><span class="sxs-lookup"><span data-stu-id="9dc9d-130">Request</span></span>
<span data-ttu-id="9dc9d-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-131">The following is an example of the request.</span></span> <span data-ttu-id="9dc9d-132">该约会不涉及预订特定人员成员。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-132">This appointment does not involve booking specific staff members.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingappointment_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "customerEmailAddress":"jordanm@contoso.com",
    "customerLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"123 First Avenue",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Customer",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "customerName":"Jordan Miller",
    "customerNotes":"Please be on time.",
    "customerPhone":"213-555-0199",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceAmount":10.0,
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceId":"1001",
    "invoiceStatus@odata.type":"#microsoft.graph.bookingInvoiceStatus",
    "invoiceStatus":"open",
    "invoiceUrl":"theInvoiceUrl",
    "optOutOfCustomerEmail":false,
    "postBuffer":"PT10M",
    "preBuffer":"PT5M",
    "price":10.0,
    "priceType@odata.type":"#microsoft.graph.bookingPriceType",
    "priceType":"fixedPrice",
    "reminders@odata.type":"#Collection(microsoft.graph.bookingReminder)",
    "reminders":[
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"This service is tomorrow",
            "offset":"P1D",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"allAttendees"
        },
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please be available to enjoy your lunch service.",
            "offset":"PT1H",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"customer"
        },
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please check traffic for next cater.",
            "offset":"PT2H",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"staff"
        }
    ],
    "serviceId":"57da6774-a087-4d69-b0e6-6fb82c339976",
    "serviceLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"123 First Avenue",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Customer location",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "serviceName":"Catered bento",
    "serviceNotes":"Customer requires punctual service.",
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
<span data-ttu-id="9dc9d-133">在请求正文中，提供[bookingAppointment](../resources/bookingappointment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-133">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="9dc9d-134">响应</span><span class="sxs-lookup"><span data-stu-id="9dc9d-134">Response</span></span>
<span data-ttu-id="9dc9d-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-135">The following is an example of the response.</span></span> <span data-ttu-id="9dc9d-136">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9dc9d-137">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9dc9d-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments/$entity",
    "id": "AAMkADc7zF4J0AAA8v_KnAAA=",
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
        "dateTime": "2018-05-01T12:30:00.0000000Z",
        "timeZone": "UTC"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->