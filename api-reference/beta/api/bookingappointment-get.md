---
title: 获取 bookingAppointment
description: 获取指定 bookingbusiness 中的 bookingAppointment 对象的属性和关系。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3f21d9b57f0ef692db80e42f40a152d3bdc29bfa
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636518"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="73c6c-103">获取 bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="73c6c-103">Get bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73c6c-104">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingAppointment](../resources/bookingappointment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73c6c-104">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="73c6c-105">**开始**和**结束**属性总是以 UTC 形式返回。</span><span class="sxs-lookup"><span data-stu-id="73c6c-105">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="73c6c-106">权限</span><span class="sxs-lookup"><span data-stu-id="73c6c-106">Permissions</span></span>
<span data-ttu-id="73c6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73c6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73c6c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73c6c-109">Permission type</span></span>      | <span data-ttu-id="73c6c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73c6c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73c6c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73c6c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="73c6c-112">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="73c6c-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="73c6c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73c6c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73c6c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73c6c-114">Not supported.</span></span>   |
|<span data-ttu-id="73c6c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="73c6c-115">Application</span></span> | <span data-ttu-id="73c6c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="73c6c-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="73c6c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73c6c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="73c6c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="73c6c-118">Optional query parameters</span></span>
<span data-ttu-id="73c6c-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="73c6c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73c6c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="73c6c-120">Request headers</span></span>
| <span data-ttu-id="73c6c-121">名称</span><span class="sxs-lookup"><span data-stu-id="73c6c-121">Name</span></span>      |<span data-ttu-id="73c6c-122">说明</span><span class="sxs-lookup"><span data-stu-id="73c6c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="73c6c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="73c6c-123">Authorization</span></span>  | <span data-ttu-id="73c6c-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="73c6c-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="73c6c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="73c6c-125">Request body</span></span>
<span data-ttu-id="73c6c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="73c6c-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="73c6c-127">响应</span><span class="sxs-lookup"><span data-stu-id="73c6c-127">Response</span></span>
<span data-ttu-id="73c6c-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[bookingAppointment](../resources/bookingappointment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="73c6c-128">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73c6c-129">示例</span><span class="sxs-lookup"><span data-stu-id="73c6c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73c6c-130">请求</span><span class="sxs-lookup"><span data-stu-id="73c6c-130">Request</span></span>
<span data-ttu-id="73c6c-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73c6c-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
##### <a name="response"></a><span data-ttu-id="73c6c-132">响应</span><span class="sxs-lookup"><span data-stu-id="73c6c-132">Response</span></span>
<span data-ttu-id="73c6c-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="73c6c-133">The following is an example of the response.</span></span> <span data-ttu-id="73c6c-134">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="73c6c-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="73c6c-135">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73c6c-135">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="73c6c-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="73c6c-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="73c6c-137">语言</span><span class="sxs-lookup"><span data-stu-id="73c6c-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingappointment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73c6c-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="73c6c-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingappointment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingappointment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingappointment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
