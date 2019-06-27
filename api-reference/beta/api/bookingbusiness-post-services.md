---
title: 创建 bookingService
description: 为指定的 bookingbusiness 创建新的 bookingService。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 346c165ec0341523c2f7d7becc84922b8943f846
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258133"
---
# <a name="create-bookingservice"></a><span data-ttu-id="3cd72-103">创建 bookingService</span><span class="sxs-lookup"><span data-stu-id="3cd72-103">Create bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cd72-104">为指定的[bookingbusiness](../resources/bookingbusiness.md)创建新的[bookingService](../resources/bookingservice.md) 。</span><span class="sxs-lookup"><span data-stu-id="3cd72-104">Create a new [bookingService](../resources/bookingservice.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3cd72-105">权限</span><span class="sxs-lookup"><span data-stu-id="3cd72-105">Permissions</span></span>
<span data-ttu-id="3cd72-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cd72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cd72-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cd72-108">Permission type</span></span>      | <span data-ttu-id="3cd72-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cd72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cd72-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cd72-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3cd72-111">全部预订. 全部, 全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="3cd72-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3cd72-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cd72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cd72-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cd72-113">Not supported.</span></span>   |
|<span data-ttu-id="3cd72-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cd72-114">Application</span></span> | <span data-ttu-id="3cd72-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cd72-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3cd72-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cd72-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/services

```
## <a name="request-headers"></a><span data-ttu-id="3cd72-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cd72-117">Request headers</span></span>
| <span data-ttu-id="3cd72-118">名称</span><span class="sxs-lookup"><span data-stu-id="3cd72-118">Name</span></span>       | <span data-ttu-id="3cd72-119">说明</span><span class="sxs-lookup"><span data-stu-id="3cd72-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3cd72-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cd72-120">Authorization</span></span>  | <span data-ttu-id="3cd72-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="3cd72-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cd72-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cd72-122">Request body</span></span>
<span data-ttu-id="3cd72-123">在请求正文中, 提供[bookingService](../resources/bookingservice.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3cd72-123">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="3cd72-124">响应</span><span class="sxs-lookup"><span data-stu-id="3cd72-124">Response</span></span>
<span data-ttu-id="3cd72-125">如果成功, 此方法在`201, Created`响应正文中返回响应代码和[bookingService](../resources/bookingservice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3cd72-125">If successful, this method returns `201, Created` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cd72-126">示例</span><span class="sxs-lookup"><span data-stu-id="3cd72-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3cd72-127">请求</span><span class="sxs-lookup"><span data-stu-id="3cd72-127">Request</span></span>
<span data-ttu-id="3cd72-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3cd72-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingservice_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT1H30M",
    "defaultLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"4567 First Street",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Contoso Lunch Delivery",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "defaultPrice":10.0,
    "defaultPriceType@odata.type":"#microsoft.graph.bookingPriceType",
    "defaultPriceType":"fixedPrice",
    "defaultReminders@odata.type":"#Collection(microsoft.graph.bookingReminder)",
    "defaultReminders":[
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please be reminded that this service is tomorrow.",
            "offset":"P1D",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"allAttendees"
        }
    ],
    "description":"Individual bento box lunch delivery",
    "displayName":"Bento",
    "isHiddenFromCustomers":false,
    "notes":"Home-cooked special",
    "postBuffer":"PT10M",
    "preBuffer":"PT5M",
    "schedulingPolicy":{
        "@odata.type":"#microsoft.graph.bookingSchedulingPolicy",
        "allowStaffSelection":true,
        "maximumAdvance":"P10D",
        "minimumLeadTime":"PT10H",
        "sendConfirmationsToOwner":true,
        "timeSlotInterval":"PT1H"
    },
    "staffMemberIds@odata.type":"#Collection(String)",
    "staffMemberIds":[
        "d90d1e8c-5cfe-48cf-a2d5-966267375b6a",
        "2f5f8794-0b29-45b5-b56a-2eb5ff7aa880"
    ]
}
```
<span data-ttu-id="3cd72-129">在请求正文中, 提供[bookingService](../resources/bookingservice.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3cd72-129">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3cd72-130">响应</span><span class="sxs-lookup"><span data-stu-id="3cd72-130">Response</span></span>
<span data-ttu-id="3cd72-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3cd72-131">The following is an example of the response.</span></span> <span data-ttu-id="3cd72-132">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3cd72-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3cd72-133">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3cd72-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services/$entity",
    "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "displayName": "Bento",
    "defaultDuration": "PT1H30M",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3cd72-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3cd72-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3cd72-135">C#</span><span class="sxs-lookup"><span data-stu-id="3cd72-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_bookingservice_from_bookingbusiness-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3cd72-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="3cd72-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_bookingservice_from_bookingbusiness-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3cd72-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="3cd72-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_bookingservice_from_bookingbusiness-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-services.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingbusiness-post-services.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-post-services.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
