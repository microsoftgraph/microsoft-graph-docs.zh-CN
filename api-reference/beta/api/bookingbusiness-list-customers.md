---
title: 列出客户
description: 获取 bookingCustomer 对象的列表。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 8833f11ac3755fb63bc0faf504001efc1353ad6a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439271"
---
# <a name="list-customers"></a><span data-ttu-id="7e91d-103">列出客户</span><span class="sxs-lookup"><span data-stu-id="7e91d-103">List customers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e91d-104">获取[bookingCustomer](../resources/bookingcustomer.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7e91d-104">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="7e91d-105">权限</span><span class="sxs-lookup"><span data-stu-id="7e91d-105">Permissions</span></span>
<span data-ttu-id="7e91d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7e91d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e91d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7e91d-108">Permission type</span></span>      | <span data-ttu-id="7e91d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7e91d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e91d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7e91d-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7e91d-111">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="7e91d-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="7e91d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7e91d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e91d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e91d-113">Not supported.</span></span>   |
|<span data-ttu-id="7e91d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7e91d-114">Application</span></span> | <span data-ttu-id="7e91d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7e91d-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="7e91d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7e91d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7e91d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7e91d-117">Optional query parameters</span></span>
<span data-ttu-id="7e91d-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7e91d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7e91d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7e91d-119">Request headers</span></span>
| <span data-ttu-id="7e91d-120">名称</span><span class="sxs-lookup"><span data-stu-id="7e91d-120">Name</span></span>      |<span data-ttu-id="7e91d-121">说明</span><span class="sxs-lookup"><span data-stu-id="7e91d-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7e91d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e91d-122">Authorization</span></span>  | <span data-ttu-id="7e91d-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7e91d-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e91d-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="7e91d-124">Request body</span></span>
<span data-ttu-id="7e91d-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7e91d-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="7e91d-126">响应</span><span class="sxs-lookup"><span data-stu-id="7e91d-126">Response</span></span>
<span data-ttu-id="7e91d-127">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[bookingCustomer](../resources/bookingcustomer.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="7e91d-127">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e91d-128">示例</span><span class="sxs-lookup"><span data-stu-id="7e91d-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7e91d-129">请求</span><span class="sxs-lookup"><span data-stu-id="7e91d-129">Request</span></span>
<span data-ttu-id="7e91d-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7e91d-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7e91d-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7e91d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7e91d-132">C#</span><span class="sxs-lookup"><span data-stu-id="7e91d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-customers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7e91d-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="7e91d-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-customers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7e91d-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="7e91d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-customers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7e91d-135">响应</span><span class="sxs-lookup"><span data-stu-id="7e91d-135">Response</span></span>
<span data-ttu-id="7e91d-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7e91d-136">The following is an example of the response.</span></span> <span data-ttu-id="7e91d-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7e91d-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="7e91d-138">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7e91d-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers",
    "value": [
        {
            "id": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "8bb19078-0f45-4efb-b2c5-da78b860f73a",
            "displayName": "Adele Vance",
            "emailAddress": "adelev@proseware.com"
        },
        {
            "id": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "displayName": "Bob Kelly",
            "emailAddress": "bobk@tailspintoys.com"
        },
        {
            "id": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
            "displayName": "Jordan Miller",
            "emailAddress": "jordanm@contoso.com"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
