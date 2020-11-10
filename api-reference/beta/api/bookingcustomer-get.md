---
title: 获取 bookingCustomer
description: 获取 bookingCustomer 对象的属性和关系。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 3e4c6474669bb8d7b7163672e9310bec22b98980
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960480"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="5ea71-103">获取 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="5ea71-103">Get bookingCustomer</span></span>

<span data-ttu-id="5ea71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ea71-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ea71-105">获取 [bookingCustomer](../resources/bookingcustomer.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5ea71-105">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5ea71-106">权限</span><span class="sxs-lookup"><span data-stu-id="5ea71-106">Permissions</span></span>
<span data-ttu-id="5ea71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ea71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ea71-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ea71-109">Permission type</span></span>      | <span data-ttu-id="5ea71-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ea71-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ea71-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ea71-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="5ea71-112">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="5ea71-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5ea71-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ea71-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ea71-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ea71-114">Not supported.</span></span>   |
|<span data-ttu-id="5ea71-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ea71-115">Application</span></span> | <span data-ttu-id="5ea71-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ea71-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5ea71-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ea71-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5ea71-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5ea71-118">Optional query parameters</span></span>
<span data-ttu-id="5ea71-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5ea71-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ea71-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ea71-120">Request headers</span></span>
| <span data-ttu-id="5ea71-121">名称</span><span class="sxs-lookup"><span data-stu-id="5ea71-121">Name</span></span>      |<span data-ttu-id="5ea71-122">说明</span><span class="sxs-lookup"><span data-stu-id="5ea71-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ea71-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ea71-123">Authorization</span></span>  | <span data-ttu-id="5ea71-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5ea71-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ea71-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ea71-125">Request body</span></span>
<span data-ttu-id="5ea71-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ea71-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5ea71-127">响应</span><span class="sxs-lookup"><span data-stu-id="5ea71-127">Response</span></span>
<span data-ttu-id="5ea71-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [bookingCustomer](../resources/bookingcustomer.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5ea71-128">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5ea71-129">示例</span><span class="sxs-lookup"><span data-stu-id="5ea71-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ea71-130">请求</span><span class="sxs-lookup"><span data-stu-id="5ea71-130">Request</span></span>
<span data-ttu-id="5ea71-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5ea71-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ea71-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ea71-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
# <a name="c"></a>[<span data-ttu-id="5ea71-133">C#</span><span class="sxs-lookup"><span data-stu-id="5ea71-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ea71-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ea71-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ea71-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ea71-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5ea71-136">Java</span><span class="sxs-lookup"><span data-stu-id="5ea71-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ea71-137">响应</span><span class="sxs-lookup"><span data-stu-id="5ea71-137">Response</span></span>
<span data-ttu-id="5ea71-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5ea71-138">The following is an example of the response.</span></span> <span data-ttu-id="5ea71-139">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5ea71-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5ea71-140">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5ea71-140">All of the properties will be returned from an actual call.</span></span>
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
