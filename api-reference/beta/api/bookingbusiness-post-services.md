---
title: 创建 bookingService
description: 为指定的 bookingbusiness 创建新的 bookingService。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 5f790cdc87cc7beedb85421cffec8dfb65aa56e3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047859"
---
# <a name="create-bookingservice"></a><span data-ttu-id="0cead-103">创建 bookingService</span><span class="sxs-lookup"><span data-stu-id="0cead-103">Create bookingService</span></span>

<span data-ttu-id="0cead-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cead-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cead-105">为指定的[bookingbusiness](../resources/bookingbusiness.md)创建新的[bookingService。](../resources/bookingservice.md)</span><span class="sxs-lookup"><span data-stu-id="0cead-105">Create a new [bookingService](../resources/bookingservice.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="0cead-106">权限</span><span class="sxs-lookup"><span data-stu-id="0cead-106">Permissions</span></span>
<span data-ttu-id="0cead-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0cead-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cead-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cead-109">Permission type</span></span>      | <span data-ttu-id="0cead-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0cead-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cead-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cead-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="0cead-112">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0cead-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0cead-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cead-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cead-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cead-114">Not supported.</span></span>   |
|<span data-ttu-id="0cead-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0cead-115">Application</span></span> | <span data-ttu-id="0cead-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cead-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0cead-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cead-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/services

```
## <a name="request-headers"></a><span data-ttu-id="0cead-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cead-118">Request headers</span></span>
| <span data-ttu-id="0cead-119">名称</span><span class="sxs-lookup"><span data-stu-id="0cead-119">Name</span></span>       | <span data-ttu-id="0cead-120">说明</span><span class="sxs-lookup"><span data-stu-id="0cead-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0cead-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cead-121">Authorization</span></span>  | <span data-ttu-id="0cead-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0cead-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cead-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0cead-123">Request body</span></span>
<span data-ttu-id="0cead-124">在请求正文中，提供 [bookingService](../resources/bookingservice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0cead-124">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="0cead-125">响应</span><span class="sxs-lookup"><span data-stu-id="0cead-125">Response</span></span>
<span data-ttu-id="0cead-126">如果成功，此方法在 `201, Created` 响应正文中返回 响应代码和 [bookingService](../resources/bookingservice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0cead-126">If successful, this method returns `201, Created` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cead-127">示例</span><span class="sxs-lookup"><span data-stu-id="0cead-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cead-128">请求</span><span class="sxs-lookup"><span data-stu-id="0cead-128">Request</span></span>
<span data-ttu-id="0cead-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0cead-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0cead-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0cead-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0cead-131">C#</span><span class="sxs-lookup"><span data-stu-id="0cead-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingservice-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0cead-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cead-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingservice-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0cead-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0cead-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingservice-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0cead-134">Java</span><span class="sxs-lookup"><span data-stu-id="0cead-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bookingservice-from-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0cead-135">在请求正文中，提供 [bookingService](../resources/bookingservice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0cead-135">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0cead-136">响应</span><span class="sxs-lookup"><span data-stu-id="0cead-136">Response</span></span>
<span data-ttu-id="0cead-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0cead-137">The following is an example of the response.</span></span> <span data-ttu-id="0cead-138">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0cead-138">Note: The response object shown here might be shortened for readability.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


