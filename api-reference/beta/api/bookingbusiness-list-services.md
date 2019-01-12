---
title: 列表服务
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 9f00ca7be7c3e6e3633a69a4a21df5e9a556096d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941707"
---
# <a name="list-services"></a><span data-ttu-id="c5d5a-104">列表服务</span><span class="sxs-lookup"><span data-stu-id="c5d5a-104">List services</span></span>

 > <span data-ttu-id="c5d5a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5d5a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="c5d5a-107">指定[bookingbusiness](../resources/bookingbusiness.md)中获取[bookingService](../resources/bookingservice.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-107">Get a list of [bookingService](../resources/bookingservice.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c5d5a-108">权限</span><span class="sxs-lookup"><span data-stu-id="c5d5a-108">Permissions</span></span>
<span data-ttu-id="c5d5a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5d5a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5d5a-111">Permission type</span></span>      | <span data-ttu-id="c5d5a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5d5a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5d5a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5d5a-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c5d5a-114">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c5d5a-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c5d5a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5d5a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5d5a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-116">Not supported.</span></span>   |
|<span data-ttu-id="c5d5a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5d5a-117">Application</span></span> | <span data-ttu-id="c5d5a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="c5d5a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5d5a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5d5a-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c5d5a-120">Optional query parameters</span></span>
<span data-ttu-id="c5d5a-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5d5a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5d5a-122">Request headers</span></span>
| <span data-ttu-id="c5d5a-123">名称</span><span class="sxs-lookup"><span data-stu-id="c5d5a-123">Name</span></span>      |<span data-ttu-id="c5d5a-124">说明</span><span class="sxs-lookup"><span data-stu-id="c5d5a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c5d5a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5d5a-125">Authorization</span></span>  | <span data-ttu-id="c5d5a-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c5d5a-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5d5a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5d5a-127">Request body</span></span>
<span data-ttu-id="c5d5a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c5d5a-129">响应</span><span class="sxs-lookup"><span data-stu-id="c5d5a-129">Response</span></span>
<span data-ttu-id="c5d5a-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[bookingService](../resources/bookingservice.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-130">If successful, this method returns a `200 OK` response code and collection of [bookingService](../resources/bookingservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5d5a-131">示例</span><span class="sxs-lookup"><span data-stu-id="c5d5a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5d5a-132">请求</span><span class="sxs-lookup"><span data-stu-id="c5d5a-132">Request</span></span>
<span data-ttu-id="c5d5a-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
```
##### <a name="response"></a><span data-ttu-id="c5d5a-134">响应</span><span class="sxs-lookup"><span data-stu-id="c5d5a-134">Response</span></span>
<span data-ttu-id="c5d5a-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-135">The following is an example of the response.</span></span> <span data-ttu-id="c5d5a-136">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c5d5a-137">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5d5a-137">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
