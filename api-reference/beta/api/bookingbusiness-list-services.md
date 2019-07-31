---
title: 列出服务
description: 获取指定 bookingbusiness 中的 bookingService 对象的列表。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 5400a917a9e795fbb0e37f1c609ad06b3231407f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35945180"
---
# <a name="list-services"></a><span data-ttu-id="611e6-103">列出服务</span><span class="sxs-lookup"><span data-stu-id="611e6-103">List services</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="611e6-104">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingService](../resources/bookingservice.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="611e6-104">Get a list of [bookingService](../resources/bookingservice.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="611e6-105">权限</span><span class="sxs-lookup"><span data-stu-id="611e6-105">Permissions</span></span>
<span data-ttu-id="611e6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="611e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="611e6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="611e6-108">Permission type</span></span>      | <span data-ttu-id="611e6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="611e6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="611e6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="611e6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="611e6-111">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="611e6-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="611e6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="611e6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="611e6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="611e6-113">Not supported.</span></span>   |
|<span data-ttu-id="611e6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="611e6-114">Application</span></span> | <span data-ttu-id="611e6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="611e6-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="611e6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="611e6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a><span data-ttu-id="611e6-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="611e6-117">Optional query parameters</span></span>
<span data-ttu-id="611e6-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="611e6-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="611e6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="611e6-119">Request headers</span></span>
| <span data-ttu-id="611e6-120">名称</span><span class="sxs-lookup"><span data-stu-id="611e6-120">Name</span></span>      |<span data-ttu-id="611e6-121">说明</span><span class="sxs-lookup"><span data-stu-id="611e6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="611e6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="611e6-122">Authorization</span></span>  | <span data-ttu-id="611e6-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="611e6-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="611e6-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="611e6-124">Request body</span></span>
<span data-ttu-id="611e6-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="611e6-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="611e6-126">响应</span><span class="sxs-lookup"><span data-stu-id="611e6-126">Response</span></span>
<span data-ttu-id="611e6-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[bookingService](../resources/bookingservice.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="611e6-127">If successful, this method returns a `200 OK` response code and collection of [bookingService](../resources/bookingservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="611e6-128">示例</span><span class="sxs-lookup"><span data-stu-id="611e6-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="611e6-129">请求</span><span class="sxs-lookup"><span data-stu-id="611e6-129">Request</span></span>
<span data-ttu-id="611e6-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="611e6-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="611e6-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="611e6-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="611e6-132">C#</span><span class="sxs-lookup"><span data-stu-id="611e6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="611e6-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="611e6-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="611e6-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="611e6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="611e6-135">Java</span><span class="sxs-lookup"><span data-stu-id="611e6-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-services-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="611e6-136">响应</span><span class="sxs-lookup"><span data-stu-id="611e6-136">Response</span></span>
<span data-ttu-id="611e6-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="611e6-137">The following is an example of the response.</span></span> <span data-ttu-id="611e6-138">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="611e6-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="611e6-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="611e6-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services",
    "value": [
        {
            "id": "f9b9121f-aed7-4c8c-bb3a-a1796a0b0b2d",
            "displayName": "Initial service",
            "defaultDuration": "PT10M",
            "defaultPrice": 0,
            "defaultPriceType": "notSet",
            "description": "Not sure how to choose? Let us introduce you to our traditional family recipes.",
            "isHiddenFromCustomers": false,
            "notes": "This is where you can add notes about this service that only you and your staff see.",
            "preBuffer": "PT0S",
            "postBuffer": "PT0S",
            "staffMemberIds": [],
            "schedulingPolicy": null,
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
            "defaultReminders": []
        },
        {
            "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "displayName": "Catered bento",
            "defaultDuration": "PT30M",
            "defaultPrice": 10,
            "defaultPriceType": "fixedPrice",
            "description": "Catered individual bento box lunch",
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
            "defaultReminders": [],
            "schedulingPolicy": {
                "timeSlotInterval": "PT1H",
                "minimumLeadTime": "PT10H",
                "maximumAdvance": "P10D",
                "sendConfirmationsToOwner": true,
                "allowStaffSelection": true
            }
        },
        {
            "id": "635a7b7c-4230-4d3b-a42b-698e89927528",
            "displayName": "Kaiseki",
            "defaultDuration": "PT1H30M",
            "defaultPrice": 30,
            "defaultPriceType": "fixedPrice",
            "description": "Individual kaiseki lunch delivery",
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
            "defaultReminders": [],
            "schedulingPolicy": {
                "timeSlotInterval": "PT1H",
                "minimumLeadTime": "PT10H",
                "maximumAdvance": "P10D",
                "sendConfirmationsToOwner": true,
                "allowStaffSelection": true
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
