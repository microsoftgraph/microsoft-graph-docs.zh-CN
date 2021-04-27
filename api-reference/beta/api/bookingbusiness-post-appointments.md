---
title: 创建 bookingAppointment
description: 为指定的 bookingbusiness 创建新的 bookingAppointment。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 02ad305da8c4d42e6d63e8d511380a707c806b2a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047887"
---
# <a name="create-bookingappointment"></a><span data-ttu-id="0580e-103">创建 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="0580e-103">Create bookingAppointment</span></span>

<span data-ttu-id="0580e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0580e-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0580e-105">为指定的[bookingbusiness 创建新的 bookingAppointment。](../resources/bookingappointment.md) [](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="0580e-105">Create a new [bookingAppointment](../resources/bookingappointment.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="0580e-106">权限</span><span class="sxs-lookup"><span data-stu-id="0580e-106">Permissions</span></span>
<span data-ttu-id="0580e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0580e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0580e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0580e-109">Permission type</span></span>      | <span data-ttu-id="0580e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0580e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0580e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0580e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="0580e-112">BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0580e-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0580e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0580e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0580e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0580e-114">Not supported.</span></span>   |
|<span data-ttu-id="0580e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0580e-115">Application</span></span> | <span data-ttu-id="0580e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0580e-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0580e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0580e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments

```
## <a name="request-headers"></a><span data-ttu-id="0580e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0580e-118">Request headers</span></span>
| <span data-ttu-id="0580e-119">名称</span><span class="sxs-lookup"><span data-stu-id="0580e-119">Name</span></span>       | <span data-ttu-id="0580e-120">说明</span><span class="sxs-lookup"><span data-stu-id="0580e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0580e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0580e-121">Authorization</span></span>  | <span data-ttu-id="0580e-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0580e-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0580e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0580e-123">Request body</span></span>
<span data-ttu-id="0580e-124">在请求正文中，提供 [bookingAppointment](../resources/bookingappointment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0580e-124">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="0580e-125">响应</span><span class="sxs-lookup"><span data-stu-id="0580e-125">Response</span></span>
<span data-ttu-id="0580e-126">如果成功，此方法在 `201, Created` 响应正文中返回 响应代码和 [bookingAppointment](../resources/bookingappointment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0580e-126">If successful, this method returns `201, Created` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0580e-127">示例</span><span class="sxs-lookup"><span data-stu-id="0580e-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0580e-128">请求</span><span class="sxs-lookup"><span data-stu-id="0580e-128">Request</span></span>
<span data-ttu-id="0580e-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0580e-129">The following is an example of the request.</span></span> <span data-ttu-id="0580e-130">此约会不涉及预订特定员工。</span><span class="sxs-lookup"><span data-stu-id="0580e-130">This appointment does not involve booking specific staff members.</span></span>

# <a name="http"></a>[<span data-ttu-id="0580e-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0580e-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0580e-132">C#</span><span class="sxs-lookup"><span data-stu-id="0580e-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingappointment-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0580e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0580e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingappointment-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0580e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0580e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingappointment-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0580e-135">Java</span><span class="sxs-lookup"><span data-stu-id="0580e-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingappointment-from-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0580e-136">在请求正文中，提供 [bookingAppointment](../resources/bookingappointment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0580e-136">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0580e-137">响应</span><span class="sxs-lookup"><span data-stu-id="0580e-137">Response</span></span>
<span data-ttu-id="0580e-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0580e-138">The following is an example of the response.</span></span> <span data-ttu-id="0580e-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0580e-139">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


