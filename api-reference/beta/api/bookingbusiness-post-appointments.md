---
title: 创建 bookingAppointment
description: 为指定的 bookingbusiness 创建新的 bookingAppointment。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6bc67a6e33c860e003cdbc85cd1e0c402570a06c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865613"
---
# <a name="create-bookingappointment"></a><span data-ttu-id="5dfa6-103">创建 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="5dfa6-103">Create bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5dfa6-104">为指定的[bookingbusiness](../resources/bookingbusiness.md)创建新的[bookingAppointment](../resources/bookingappointment.md) 。</span><span class="sxs-lookup"><span data-stu-id="5dfa6-104">Create a new [bookingAppointment](../resources/bookingappointment.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5dfa6-105">权限</span><span class="sxs-lookup"><span data-stu-id="5dfa6-105">Permissions</span></span>
<span data-ttu-id="5dfa6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5dfa6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5dfa6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5dfa6-108">Permission type</span></span>      | <span data-ttu-id="5dfa6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5dfa6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5dfa6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5dfa6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5dfa6-111">BookingsAppointment, 全部, 全部登记, 全部, 预订。 All</span><span class="sxs-lookup"><span data-stu-id="5dfa6-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5dfa6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5dfa6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5dfa6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dfa6-113">Not supported.</span></span>   |
|<span data-ttu-id="5dfa6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5dfa6-114">Application</span></span> | <span data-ttu-id="5dfa6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dfa6-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5dfa6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5dfa6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments

```
## <a name="request-headers"></a><span data-ttu-id="5dfa6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5dfa6-117">Request headers</span></span>
| <span data-ttu-id="5dfa6-118">名称</span><span class="sxs-lookup"><span data-stu-id="5dfa6-118">Name</span></span>       | <span data-ttu-id="5dfa6-119">说明</span><span class="sxs-lookup"><span data-stu-id="5dfa6-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5dfa6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dfa6-120">Authorization</span></span>  | <span data-ttu-id="5dfa6-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5dfa6-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dfa6-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="5dfa6-122">Request body</span></span>
<span data-ttu-id="5dfa6-123">在请求正文中, 提供[bookingAppointment](../resources/bookingappointment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5dfa6-123">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="5dfa6-124">响应</span><span class="sxs-lookup"><span data-stu-id="5dfa6-124">Response</span></span>
<span data-ttu-id="5dfa6-125">如果成功, 此方法在`201, Created`响应正文中返回响应代码和[bookingAppointment](../resources/bookingappointment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5dfa6-125">If successful, this method returns `201, Created` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dfa6-126">示例</span><span class="sxs-lookup"><span data-stu-id="5dfa6-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5dfa6-127">请求</span><span class="sxs-lookup"><span data-stu-id="5dfa6-127">Request</span></span>
<span data-ttu-id="5dfa6-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5dfa6-128">The following is an example of the request.</span></span> <span data-ttu-id="5dfa6-129">此约会不涉及预订特定的教职员工成员。</span><span class="sxs-lookup"><span data-stu-id="5dfa6-129">This appointment does not involve booking specific staff members.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5dfa6-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5dfa6-130">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5dfa6-131">C#</span><span class="sxs-lookup"><span data-stu-id="5dfa6-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingappointment-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5dfa6-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="5dfa6-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingappointment-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5dfa6-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="5dfa6-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingappointment-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="5dfa6-134">Java</span><span class="sxs-lookup"><span data-stu-id="5dfa6-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingappointment-from-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="5dfa6-135">在请求正文中, 提供[bookingAppointment](../resources/bookingappointment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5dfa6-135">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5dfa6-136">响应</span><span class="sxs-lookup"><span data-stu-id="5dfa6-136">Response</span></span>
<span data-ttu-id="5dfa6-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5dfa6-137">The following is an example of the response.</span></span> <span data-ttu-id="5dfa6-138">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5dfa6-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5dfa6-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5dfa6-139">All of the properties will be returned from an actual call.</span></span>
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
