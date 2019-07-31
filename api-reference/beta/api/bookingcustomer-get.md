---
title: 获取 bookingCustomer
description: 获取 bookingCustomer 对象的属性和关系。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: ca93e963fa1ac77128f38449eb67582a11abd736
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944960"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="94a22-103">获取 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="94a22-103">Get bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94a22-104">获取[bookingCustomer](../resources/bookingcustomer.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94a22-104">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="94a22-105">权限</span><span class="sxs-lookup"><span data-stu-id="94a22-105">Permissions</span></span>
<span data-ttu-id="94a22-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94a22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94a22-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="94a22-108">Permission type</span></span>      | <span data-ttu-id="94a22-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94a22-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a22-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94a22-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="94a22-111">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="94a22-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="94a22-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94a22-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a22-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="94a22-113">Not supported.</span></span>   |
|<span data-ttu-id="94a22-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="94a22-114">Application</span></span> | <span data-ttu-id="94a22-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94a22-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="94a22-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94a22-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="94a22-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="94a22-117">Optional query parameters</span></span>
<span data-ttu-id="94a22-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="94a22-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94a22-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="94a22-119">Request headers</span></span>
| <span data-ttu-id="94a22-120">名称</span><span class="sxs-lookup"><span data-stu-id="94a22-120">Name</span></span>      |<span data-ttu-id="94a22-121">说明</span><span class="sxs-lookup"><span data-stu-id="94a22-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="94a22-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="94a22-122">Authorization</span></span>  | <span data-ttu-id="94a22-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="94a22-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="94a22-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="94a22-124">Request body</span></span>
<span data-ttu-id="94a22-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="94a22-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="94a22-126">响应</span><span class="sxs-lookup"><span data-stu-id="94a22-126">Response</span></span>
<span data-ttu-id="94a22-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94a22-127">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94a22-128">示例</span><span class="sxs-lookup"><span data-stu-id="94a22-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94a22-129">请求</span><span class="sxs-lookup"><span data-stu-id="94a22-129">Request</span></span>
<span data-ttu-id="94a22-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="94a22-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="94a22-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="94a22-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="94a22-132">C#</span><span class="sxs-lookup"><span data-stu-id="94a22-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94a22-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="94a22-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94a22-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="94a22-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="94a22-135">Java</span><span class="sxs-lookup"><span data-stu-id="94a22-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="94a22-136">响应</span><span class="sxs-lookup"><span data-stu-id="94a22-136">Response</span></span>
<span data-ttu-id="94a22-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="94a22-137">The following is an example of the response.</span></span> <span data-ttu-id="94a22-138">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="94a22-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="94a22-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94a22-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
    "displayName": "Adele Vance",
    "emailAddress": "adelev@proseware.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
