---
title: 获取 bookingService
description: 获取指定 bookingbusiness 中的 bookingService 对象的属性和关系。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9d868a383701fca5519c1c19b3dfe5ef5c2e7398
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35257916"
---
# <a name="get-bookingservice"></a><span data-ttu-id="8d4dc-103">获取 bookingService</span><span class="sxs-lookup"><span data-stu-id="8d4dc-103">Get bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d4dc-104">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingService](../resources/bookingservice.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8d4dc-104">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="8d4dc-105">权限</span><span class="sxs-lookup"><span data-stu-id="8d4dc-105">Permissions</span></span>
<span data-ttu-id="8d4dc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8d4dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d4dc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8d4dc-108">Permission type</span></span>      | <span data-ttu-id="8d4dc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8d4dc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8d4dc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8d4dc-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8d4dc-111">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="8d4dc-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8d4dc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8d4dc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8d4dc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d4dc-113">Not supported.</span></span>   |
|<span data-ttu-id="8d4dc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8d4dc-114">Application</span></span> | <span data-ttu-id="8d4dc-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8d4dc-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8d4dc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8d4dc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8d4dc-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8d4dc-117">Optional query parameters</span></span>
<span data-ttu-id="8d4dc-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8d4dc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8d4dc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8d4dc-119">Request headers</span></span>
| <span data-ttu-id="8d4dc-120">名称</span><span class="sxs-lookup"><span data-stu-id="8d4dc-120">Name</span></span>      |<span data-ttu-id="8d4dc-121">说明</span><span class="sxs-lookup"><span data-stu-id="8d4dc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8d4dc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d4dc-122">Authorization</span></span>  | <span data-ttu-id="8d4dc-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8d4dc-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d4dc-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8d4dc-124">Request body</span></span>
<span data-ttu-id="8d4dc-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8d4dc-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8d4dc-126">响应</span><span class="sxs-lookup"><span data-stu-id="8d4dc-126">Response</span></span>
<span data-ttu-id="8d4dc-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[bookingService](../resources/bookingservice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8d4dc-127">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8d4dc-128">示例</span><span class="sxs-lookup"><span data-stu-id="8d4dc-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8d4dc-129">请求</span><span class="sxs-lookup"><span data-stu-id="8d4dc-129">Request</span></span>
<span data-ttu-id="8d4dc-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8d4dc-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="8d4dc-131">响应</span><span class="sxs-lookup"><span data-stu-id="8d4dc-131">Response</span></span>
<span data-ttu-id="8d4dc-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8d4dc-132">The following is an example of the response.</span></span> <span data-ttu-id="8d4dc-133">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8d4dc-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8d4dc-134">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8d4dc-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services/$entity",
    "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "displayName": "Bento",
    "defaultDuration": "PT30M",
    "defaultPrice": 10,
    "defaultPriceType": "fixedPrice",
    "description": "Individual bento box lunch delivery",
    "isHiddenFromCustomers": false,
    "notes": "Home-cooked special",
    "preBuffer": "PT5M",
    "postBuffer": "PT10M",
    "staffMemberIds": [],
    "defaultLocation": {
        "displayName": "Contoso Lunch Delivery",
        "locationEmailAddress": null,
        "locationUri": "",
        "locationType": null,
        "uniqueId": null,
        "uniqueIdType": null,
        "address": {
            "type": "home",
            "postOfficeBox": "",
            "street": "4567 First Street",
            "city": "Buffalo",
            "state": "NY",
            "countryOrRegion": "USA",
            "postalCode": "98052"
        },
        "coordinates": {
            "altitude": null,
            "latitude": null,
            "longitude": null,
            "accuracy": null,
            "altitudeAccuracy": null
        }
    },
    "defaultReminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "Please be reminded that this service is tomorrow."
        }
    ],
    "schedulingPolicy": {
        "timeSlotInterval": "PT1H",
        "minimumLeadTime": "PT10H",
        "maximumAdvance": "P10D",
        "sendConfirmationsToOwner": true,
        "allowStaffSelection": true
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8d4dc-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8d4dc-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8d4dc-136">C#</span><span class="sxs-lookup"><span data-stu-id="8d4dc-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingservice-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8d4dc-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="8d4dc-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingservice-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8d4dc-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="8d4dc-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_bookingservice-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingservice-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingservice-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
