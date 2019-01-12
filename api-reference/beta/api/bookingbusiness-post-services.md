---
title: 创建 bookingService
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 13a180a74866d79ecf4540a0feac58d044082a04
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990346"
---
# <a name="create-bookingservice"></a><span data-ttu-id="53df2-104">创建 bookingService</span><span class="sxs-lookup"><span data-stu-id="53df2-104">Create bookingService</span></span>

 > <span data-ttu-id="53df2-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="53df2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53df2-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="53df2-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="53df2-107">创建新[bookingService](../resources/bookingservice.md)的指定[bookingbusiness](../resources/bookingbusiness.md)。</span><span class="sxs-lookup"><span data-stu-id="53df2-107">Create a new [bookingService](../resources/bookingservice.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="53df2-108">权限</span><span class="sxs-lookup"><span data-stu-id="53df2-108">Permissions</span></span>
<span data-ttu-id="53df2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53df2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53df2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="53df2-111">Permission type</span></span>      | <span data-ttu-id="53df2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53df2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53df2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53df2-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="53df2-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="53df2-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="53df2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53df2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53df2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="53df2-116">Not supported.</span></span>   |
|<span data-ttu-id="53df2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="53df2-117">Application</span></span> | <span data-ttu-id="53df2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="53df2-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="53df2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53df2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/services

```
## <a name="request-headers"></a><span data-ttu-id="53df2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="53df2-120">Request headers</span></span>
| <span data-ttu-id="53df2-121">名称</span><span class="sxs-lookup"><span data-stu-id="53df2-121">Name</span></span>       | <span data-ttu-id="53df2-122">说明</span><span class="sxs-lookup"><span data-stu-id="53df2-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="53df2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="53df2-123">Authorization</span></span>  | <span data-ttu-id="53df2-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="53df2-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="53df2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="53df2-125">Request body</span></span>
<span data-ttu-id="53df2-126">在请求正文中，提供[bookingService](../resources/bookingservice.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53df2-126">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="53df2-127">响应</span><span class="sxs-lookup"><span data-stu-id="53df2-127">Response</span></span>
<span data-ttu-id="53df2-128">如果成功，此方法返回`201, Created`响应正文中的响应代码和[bookingService](../resources/bookingservice.md)对象。</span><span class="sxs-lookup"><span data-stu-id="53df2-128">If successful, this method returns `201, Created` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53df2-129">示例</span><span class="sxs-lookup"><span data-stu-id="53df2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53df2-130">请求</span><span class="sxs-lookup"><span data-stu-id="53df2-130">Request</span></span>
<span data-ttu-id="53df2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="53df2-131">The following is an example of the request.</span></span>
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
<span data-ttu-id="53df2-132">在请求正文中，提供[bookingService](../resources/bookingservice.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53df2-132">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="53df2-133">响应</span><span class="sxs-lookup"><span data-stu-id="53df2-133">Response</span></span>
<span data-ttu-id="53df2-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="53df2-134">The following is an example of the response.</span></span> <span data-ttu-id="53df2-135">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="53df2-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="53df2-136">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53df2-136">All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
