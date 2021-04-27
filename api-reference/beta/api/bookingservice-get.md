---
title: 获取 bookingService
description: 获取指定 bookingbusiness 中的 bookingService 对象的属性和关系。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 75b3c4db0bc37dc71acefbf3d551221eac821303
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047803"
---
# <a name="get-bookingservice"></a><span data-ttu-id="07760-103">获取 bookingService</span><span class="sxs-lookup"><span data-stu-id="07760-103">Get bookingService</span></span>

<span data-ttu-id="07760-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07760-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07760-105">获取指定的 [bookingbusiness](../resources/bookingservice.md) 中的 bookingService 对象的属性 [和关系](../resources/bookingbusiness.md)。</span><span class="sxs-lookup"><span data-stu-id="07760-105">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="07760-106">权限</span><span class="sxs-lookup"><span data-stu-id="07760-106">Permissions</span></span>
<span data-ttu-id="07760-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07760-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07760-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="07760-109">Permission type</span></span>      | <span data-ttu-id="07760-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07760-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07760-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07760-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="07760-112">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="07760-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="07760-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07760-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07760-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="07760-114">Not supported.</span></span>   |
|<span data-ttu-id="07760-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="07760-115">Application</span></span> | <span data-ttu-id="07760-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="07760-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="07760-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07760-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="07760-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="07760-118">Optional query parameters</span></span>
<span data-ttu-id="07760-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="07760-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="07760-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="07760-120">Request headers</span></span>
| <span data-ttu-id="07760-121">名称</span><span class="sxs-lookup"><span data-stu-id="07760-121">Name</span></span>      |<span data-ttu-id="07760-122">说明</span><span class="sxs-lookup"><span data-stu-id="07760-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07760-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07760-123">Authorization</span></span>  | <span data-ttu-id="07760-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="07760-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="07760-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="07760-125">Request body</span></span>
<span data-ttu-id="07760-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="07760-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="07760-127">响应</span><span class="sxs-lookup"><span data-stu-id="07760-127">Response</span></span>
<span data-ttu-id="07760-128">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [bookingService](../resources/bookingservice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07760-128">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="07760-129">示例</span><span class="sxs-lookup"><span data-stu-id="07760-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07760-130">请求</span><span class="sxs-lookup"><span data-stu-id="07760-130">Request</span></span>
<span data-ttu-id="07760-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="07760-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="07760-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="07760-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
# <a name="c"></a>[<span data-ttu-id="07760-133">C#</span><span class="sxs-lookup"><span data-stu-id="07760-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="07760-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="07760-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="07760-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="07760-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="07760-136">Java</span><span class="sxs-lookup"><span data-stu-id="07760-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="07760-137">响应</span><span class="sxs-lookup"><span data-stu-id="07760-137">Response</span></span>
<span data-ttu-id="07760-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="07760-138">The following is an example of the response.</span></span> <span data-ttu-id="07760-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="07760-139">Note: The response object shown here might be shortened for readability.</span></span>
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
  ]
}
-->
