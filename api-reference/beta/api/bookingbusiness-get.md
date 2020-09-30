---
title: 获取 bookingBusiness
description: 获取 bookingBusiness 对象的属性和关系。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d82999eae9f55c21620ce10e4c44850a9e9fc4eb
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312412"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="560ec-103">获取 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="560ec-103">Get bookingBusiness</span></span>

<span data-ttu-id="560ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="560ec-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="560ec-105">获取 [bookingBusiness](../resources/bookingbusiness.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="560ec-105">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="560ec-106">权限</span><span class="sxs-lookup"><span data-stu-id="560ec-106">Permissions</span></span>
<span data-ttu-id="560ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="560ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="560ec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="560ec-109">Permission type</span></span>      | <span data-ttu-id="560ec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="560ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="560ec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="560ec-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="560ec-112">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="560ec-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="560ec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="560ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="560ec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="560ec-114">Not supported.</span></span>   |
|<span data-ttu-id="560ec-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="560ec-115">Application</span></span> | <span data-ttu-id="560ec-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="560ec-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="560ec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="560ec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="560ec-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="560ec-118">Optional query parameters</span></span>
<span data-ttu-id="560ec-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="560ec-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="560ec-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="560ec-120">Request headers</span></span>
| <span data-ttu-id="560ec-121">名称</span><span class="sxs-lookup"><span data-stu-id="560ec-121">Name</span></span>      |<span data-ttu-id="560ec-122">说明</span><span class="sxs-lookup"><span data-stu-id="560ec-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="560ec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="560ec-123">Authorization</span></span>  | <span data-ttu-id="560ec-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="560ec-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="560ec-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="560ec-125">Request body</span></span>
<span data-ttu-id="560ec-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="560ec-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="560ec-127">响应</span><span class="sxs-lookup"><span data-stu-id="560ec-127">Response</span></span>
<span data-ttu-id="560ec-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [bookingBusiness](../resources/bookingbusiness.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="560ec-128">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="560ec-129">示例</span><span class="sxs-lookup"><span data-stu-id="560ec-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="560ec-130">请求</span><span class="sxs-lookup"><span data-stu-id="560ec-130">Request</span></span>
<span data-ttu-id="560ec-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="560ec-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="560ec-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="560ec-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
# <a name="c"></a>[<span data-ttu-id="560ec-133">C#</span><span class="sxs-lookup"><span data-stu-id="560ec-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="560ec-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="560ec-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="560ec-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="560ec-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="560ec-136">响应</span><span class="sxs-lookup"><span data-stu-id="560ec-136">Response</span></span>
<span data-ttu-id="560ec-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="560ec-137">The following is an example of the response.</span></span> <span data-ttu-id="560ec-138">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="560ec-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="560ec-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="560ec-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses/$entity",
    "id":"Fabrikam@M365B489948.onmicrosoft.com",
    "displayName":"Fabrikam",
    "businessType":"",
    "phone":"206-555-0100",
    "email":"manager@fabrikam.com",
    "webSiteUrl":"https://www.fabrikam.com/",
    "defaultCurrencyIso":"USD",
    "isPublished":false,
    "publicUrl":null,
    "address":{
        "type":"home",
        "postOfficeBox":"",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "businessHours":[
        {
            "day":"monday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"tuesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"wednesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"thursday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"friday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"saturday",
            "timeSlots":[

            ]
        },
        {
            "day":"sunday",
            "timeSlots":[

            ]
        }
    ],
    "schedulingPolicy":{
        "timeSlotInterval":"PT30M",
        "minimumLeadTime":"P1D",
        "maximumAdvance":"P365D",
        "sendConfirmationsToOwner":true,
        "allowStaffSelection":true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->