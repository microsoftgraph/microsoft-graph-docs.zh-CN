---
title: 获取 bookingAppointment
description: 获取指定 bookingbusiness 中的 bookingAppointment 对象的属性和关系。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 951ccbd2865b53bb8ec5d082b857221612986dbd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047929"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="86986-103">获取 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="86986-103">Get bookingAppointment</span></span>

<span data-ttu-id="86986-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86986-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86986-105">获取指定的 [bookingbusiness 中的 bookingAppointment](../resources/bookingappointment.md) 对象 [的属性和关系](../resources/bookingbusiness.md)。</span><span class="sxs-lookup"><span data-stu-id="86986-105">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="86986-106">**start** 和 **end** 属性始终以 UTC 格式返回。</span><span class="sxs-lookup"><span data-stu-id="86986-106">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="86986-107">权限</span><span class="sxs-lookup"><span data-stu-id="86986-107">Permissions</span></span>
<span data-ttu-id="86986-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86986-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86986-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="86986-110">Permission type</span></span>      | <span data-ttu-id="86986-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86986-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86986-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86986-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="86986-113">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="86986-113">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="86986-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86986-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86986-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="86986-115">Not supported.</span></span>   |
|<span data-ttu-id="86986-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="86986-116">Application</span></span> | <span data-ttu-id="86986-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="86986-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="86986-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86986-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="86986-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="86986-119">Optional query parameters</span></span>
<span data-ttu-id="86986-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="86986-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86986-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="86986-121">Request headers</span></span>
| <span data-ttu-id="86986-122">名称</span><span class="sxs-lookup"><span data-stu-id="86986-122">Name</span></span>      |<span data-ttu-id="86986-123">说明</span><span class="sxs-lookup"><span data-stu-id="86986-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86986-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="86986-124">Authorization</span></span>  | <span data-ttu-id="86986-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="86986-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="86986-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="86986-126">Request body</span></span>
<span data-ttu-id="86986-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86986-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="86986-128">响应</span><span class="sxs-lookup"><span data-stu-id="86986-128">Response</span></span>
<span data-ttu-id="86986-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [bookingAppointment](../resources/bookingappointment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86986-129">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86986-130">示例</span><span class="sxs-lookup"><span data-stu-id="86986-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86986-131">请求</span><span class="sxs-lookup"><span data-stu-id="86986-131">Request</span></span>
<span data-ttu-id="86986-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="86986-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="86986-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="86986-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
# <a name="c"></a>[<span data-ttu-id="86986-134">C#</span><span class="sxs-lookup"><span data-stu-id="86986-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingappointment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="86986-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86986-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingappointment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="86986-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="86986-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingappointment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="86986-137">Java</span><span class="sxs-lookup"><span data-stu-id="86986-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingappointment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="86986-138">响应</span><span class="sxs-lookup"><span data-stu-id="86986-138">Response</span></span>
<span data-ttu-id="86986-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86986-139">The following is an example of the response.</span></span> <span data-ttu-id="86986-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="86986-140">Note: The response object shown here might be shortened for readability.</span></span>
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
  ]
}
-->
