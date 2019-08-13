---
title: 获取 bookingStaffMember
description: 获取指定 bookingbusiness 中的 bookingStaffMember 的属性和关系。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: a45236dcd154b1e377a975bdd488a74b4433de94
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318096"
---
# <a name="get-bookingstaffmember"></a><span data-ttu-id="bb0de-103">获取 bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="bb0de-103">Get bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb0de-104">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingStaffMember](../resources/bookingstaffmember.md)的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb0de-104">Get the properties and relationships of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="bb0de-105">权限</span><span class="sxs-lookup"><span data-stu-id="bb0de-105">Permissions</span></span>
<span data-ttu-id="bb0de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb0de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb0de-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bb0de-108">Permission type</span></span>      | <span data-ttu-id="bb0de-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bb0de-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb0de-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bb0de-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="bb0de-111">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="bb0de-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="bb0de-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bb0de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb0de-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb0de-113">Not supported.</span></span>   |
|<span data-ttu-id="bb0de-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bb0de-114">Application</span></span> | <span data-ttu-id="bb0de-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bb0de-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="bb0de-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb0de-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb0de-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bb0de-117">Optional query parameters</span></span>
<span data-ttu-id="bb0de-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bb0de-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb0de-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb0de-119">Request headers</span></span>
| <span data-ttu-id="bb0de-120">名称</span><span class="sxs-lookup"><span data-stu-id="bb0de-120">Name</span></span>      |<span data-ttu-id="bb0de-121">说明</span><span class="sxs-lookup"><span data-stu-id="bb0de-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bb0de-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb0de-122">Authorization</span></span>  | <span data-ttu-id="bb0de-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bb0de-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb0de-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb0de-124">Request body</span></span>
<span data-ttu-id="bb0de-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb0de-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bb0de-126">响应</span><span class="sxs-lookup"><span data-stu-id="bb0de-126">Response</span></span>
<span data-ttu-id="bb0de-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[bookingStaffMember](../resources/bookingstaffmember.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bb0de-127">If successful, this method returns a `200 OK` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb0de-128">示例</span><span class="sxs-lookup"><span data-stu-id="bb0de-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb0de-129">请求</span><span class="sxs-lookup"><span data-stu-id="bb0de-129">Request</span></span>
<span data-ttu-id="bb0de-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bb0de-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bb0de-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bb0de-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingstaffmember"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bb0de-132">C#</span><span class="sxs-lookup"><span data-stu-id="bb0de-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bb0de-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb0de-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bb0de-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="bb0de-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bb0de-135">Java</span><span class="sxs-lookup"><span data-stu-id="bb0de-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingstaffmember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bb0de-136">响应</span><span class="sxs-lookup"><span data-stu-id="bb0de-136">Response</span></span>
<span data-ttu-id="bb0de-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bb0de-137">The following is an example of the response.</span></span> <span data-ttu-id="bb0de-138">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="bb0de-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bb0de-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb0de-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers/$entity",
    "id": "71d64d0e-7225-49b6-b0b1-070d476cda51",
    "displayName": "Samantha Booth",
    "emailAddress": "samanthab@M365B489948.OnMicrosoft.com",
    "availabilityIsAffectedByPersonalCalendar": true,
    "colorIndex": 0,
    "role": "administrator",
    "useBusinessHours": true,
    "workingHours": [
        {
            "day": "monday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "tuesday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "wednesday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "thursday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "friday",
            "timeSlots": [
                {
                    "start": "08:00:00.0000000",
                    "end": "17:00:00.0000000"
                }
            ]
        },
        {
            "day": "saturday",
            "timeSlots": []
        },
        {
            "day": "sunday",
            "timeSlots": []
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
