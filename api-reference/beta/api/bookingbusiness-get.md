---
title: 获取 bookingBusiness
description: 获取 bookingBusiness 对象的属性和关系。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 47b7f974ee72d89c43a0d0663982bde4d64d38b9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047922"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="184ab-103">获取 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="184ab-103">Get bookingBusiness</span></span>

<span data-ttu-id="184ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="184ab-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="184ab-105">获取 [bookingBusiness](../resources/bookingbusiness.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="184ab-105">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="184ab-106">权限</span><span class="sxs-lookup"><span data-stu-id="184ab-106">Permissions</span></span>
<span data-ttu-id="184ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="184ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="184ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="184ab-109">Permission type</span></span>      | <span data-ttu-id="184ab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="184ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="184ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="184ab-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="184ab-112">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="184ab-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="184ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="184ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="184ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="184ab-114">Not supported.</span></span>   |
|<span data-ttu-id="184ab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="184ab-115">Application</span></span> | <span data-ttu-id="184ab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="184ab-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="184ab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="184ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="184ab-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="184ab-118">Optional query parameters</span></span>
<span data-ttu-id="184ab-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="184ab-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="184ab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="184ab-120">Request headers</span></span>
| <span data-ttu-id="184ab-121">名称</span><span class="sxs-lookup"><span data-stu-id="184ab-121">Name</span></span>      |<span data-ttu-id="184ab-122">说明</span><span class="sxs-lookup"><span data-stu-id="184ab-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="184ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="184ab-123">Authorization</span></span>  | <span data-ttu-id="184ab-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="184ab-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="184ab-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="184ab-125">Request body</span></span>
<span data-ttu-id="184ab-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="184ab-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="184ab-127">响应</span><span class="sxs-lookup"><span data-stu-id="184ab-127">Response</span></span>
<span data-ttu-id="184ab-128">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [bookingBusiness](../resources/bookingbusiness.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="184ab-128">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="184ab-129">示例</span><span class="sxs-lookup"><span data-stu-id="184ab-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="184ab-130">请求</span><span class="sxs-lookup"><span data-stu-id="184ab-130">Request</span></span>
<span data-ttu-id="184ab-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="184ab-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="184ab-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="184ab-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
# <a name="c"></a>[<span data-ttu-id="184ab-133">C#</span><span class="sxs-lookup"><span data-stu-id="184ab-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="184ab-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="184ab-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="184ab-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="184ab-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="184ab-136">Java</span><span class="sxs-lookup"><span data-stu-id="184ab-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="184ab-137">响应</span><span class="sxs-lookup"><span data-stu-id="184ab-137">Response</span></span>
<span data-ttu-id="184ab-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="184ab-138">The following is an example of the response.</span></span> <span data-ttu-id="184ab-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="184ab-139">Note: The response object shown here might be shortened for readability.</span></span>
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
