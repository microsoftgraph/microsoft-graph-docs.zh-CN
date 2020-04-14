---
title: 列出服务
description: 获取指定 bookingbusiness 中的 bookingService 对象的列表。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: ccd8962ca1d34b62b60b6e2f50662e5a520b716f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43366758"
---
# <a name="list-services"></a><span data-ttu-id="1fc5b-103">列出服务</span><span class="sxs-lookup"><span data-stu-id="1fc5b-103">List services</span></span>

<span data-ttu-id="1fc5b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fc5b-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fc5b-105">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingService](../resources/bookingservice.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-105">Get a list of [bookingService](../resources/bookingservice.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="1fc5b-106">权限</span><span class="sxs-lookup"><span data-stu-id="1fc5b-106">Permissions</span></span>
<span data-ttu-id="1fc5b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1fc5b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1fc5b-109">Permission type</span></span>      | <span data-ttu-id="1fc5b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1fc5b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fc5b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fc5b-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="1fc5b-112">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="1fc5b-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="1fc5b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fc5b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fc5b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-114">Not supported.</span></span>   |
|<span data-ttu-id="1fc5b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1fc5b-115">Application</span></span> | <span data-ttu-id="1fc5b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1fc5b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fc5b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1fc5b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1fc5b-118">Optional query parameters</span></span>
<span data-ttu-id="1fc5b-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fc5b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fc5b-120">Request headers</span></span>
| <span data-ttu-id="1fc5b-121">名称</span><span class="sxs-lookup"><span data-stu-id="1fc5b-121">Name</span></span>      |<span data-ttu-id="1fc5b-122">说明</span><span class="sxs-lookup"><span data-stu-id="1fc5b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1fc5b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fc5b-123">Authorization</span></span>  | <span data-ttu-id="1fc5b-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="1fc5b-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="1fc5b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1fc5b-125">Request body</span></span>
<span data-ttu-id="1fc5b-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="1fc5b-127">响应</span><span class="sxs-lookup"><span data-stu-id="1fc5b-127">Response</span></span>
<span data-ttu-id="1fc5b-128">如果成功，此方法在响应`200 OK`正文中返回响应代码和[bookingService](../resources/bookingservice.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-128">If successful, this method returns a `200 OK` response code and collection of [bookingService](../resources/bookingservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1fc5b-129">示例</span><span class="sxs-lookup"><span data-stu-id="1fc5b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1fc5b-130">请求</span><span class="sxs-lookup"><span data-stu-id="1fc5b-130">Request</span></span>
<span data-ttu-id="1fc5b-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1fc5b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="1fc5b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
```
# <a name="c"></a>[<span data-ttu-id="1fc5b-133">C#</span><span class="sxs-lookup"><span data-stu-id="1fc5b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1fc5b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1fc5b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1fc5b-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1fc5b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="1fc5b-136">响应</span><span class="sxs-lookup"><span data-stu-id="1fc5b-136">Response</span></span>
<span data-ttu-id="1fc5b-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-137">The following is an example of the response.</span></span> <span data-ttu-id="1fc5b-138">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1fc5b-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1fc5b-139">All of the properties will be returned from an actual call.</span></span>
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
