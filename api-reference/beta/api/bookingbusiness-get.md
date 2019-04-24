---
title: 获取 bookingBusiness
description: 获取 bookingBusiness 对象的属性和关系。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 229da03e377f1ff0add73195505c359c9fd68121
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462403"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="a77b9-103">获取 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="a77b9-103">Get bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a77b9-104">获取[bookingBusiness](../resources/bookingbusiness.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a77b9-104">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a77b9-105">权限</span><span class="sxs-lookup"><span data-stu-id="a77b9-105">Permissions</span></span>
<span data-ttu-id="a77b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a77b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a77b9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a77b9-108">Permission type</span></span>      | <span data-ttu-id="a77b9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a77b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a77b9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a77b9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a77b9-111">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="a77b9-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a77b9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a77b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a77b9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a77b9-113">Not supported.</span></span>   |
|<span data-ttu-id="a77b9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a77b9-114">Application</span></span> | <span data-ttu-id="a77b9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a77b9-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a77b9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a77b9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a77b9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a77b9-117">Optional query parameters</span></span>
<span data-ttu-id="a77b9-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a77b9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a77b9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a77b9-119">Request headers</span></span>
| <span data-ttu-id="a77b9-120">名称</span><span class="sxs-lookup"><span data-stu-id="a77b9-120">Name</span></span>      |<span data-ttu-id="a77b9-121">说明</span><span class="sxs-lookup"><span data-stu-id="a77b9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a77b9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a77b9-122">Authorization</span></span>  | <span data-ttu-id="a77b9-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a77b9-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a77b9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a77b9-124">Request body</span></span>
<span data-ttu-id="a77b9-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a77b9-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a77b9-126">响应</span><span class="sxs-lookup"><span data-stu-id="a77b9-126">Response</span></span>
<span data-ttu-id="a77b9-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[bookingBusiness](../resources/bookingbusiness.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a77b9-127">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a77b9-128">示例</span><span class="sxs-lookup"><span data-stu-id="a77b9-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a77b9-129">请求</span><span class="sxs-lookup"><span data-stu-id="a77b9-129">Request</span></span>
<span data-ttu-id="a77b9-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a77b9-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="a77b9-131">响应</span><span class="sxs-lookup"><span data-stu-id="a77b9-131">Response</span></span>
<span data-ttu-id="a77b9-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a77b9-132">The following is an example of the response.</span></span> <span data-ttu-id="a77b9-133">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a77b9-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a77b9-134">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a77b9-134">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
