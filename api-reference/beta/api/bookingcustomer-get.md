---
title: 获取 bookingCustomer
description: 获取 bookingCustomer 对象的属性和关系。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 4ed191250a6858aa94b3428b1d01dd4de112c2b1
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313161"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="49bd7-103">获取 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="49bd7-103">Get bookingCustomer</span></span>

<span data-ttu-id="49bd7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49bd7-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49bd7-105">获取 [bookingCustomer](../resources/bookingcustomer.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="49bd7-105">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="49bd7-106">权限</span><span class="sxs-lookup"><span data-stu-id="49bd7-106">Permissions</span></span>
<span data-ttu-id="49bd7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49bd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49bd7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="49bd7-109">Permission type</span></span>      | <span data-ttu-id="49bd7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49bd7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49bd7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49bd7-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="49bd7-112">BookingsAppointment、全部、预订、全部、登记、全部、预订。所有</span><span class="sxs-lookup"><span data-stu-id="49bd7-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="49bd7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49bd7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49bd7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="49bd7-114">Not supported.</span></span>   |
|<span data-ttu-id="49bd7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="49bd7-115">Application</span></span> | <span data-ttu-id="49bd7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="49bd7-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="49bd7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49bd7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="49bd7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="49bd7-118">Optional query parameters</span></span>
<span data-ttu-id="49bd7-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="49bd7-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49bd7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="49bd7-120">Request headers</span></span>
| <span data-ttu-id="49bd7-121">名称</span><span class="sxs-lookup"><span data-stu-id="49bd7-121">Name</span></span>      |<span data-ttu-id="49bd7-122">说明</span><span class="sxs-lookup"><span data-stu-id="49bd7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49bd7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="49bd7-123">Authorization</span></span>  | <span data-ttu-id="49bd7-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="49bd7-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="49bd7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="49bd7-125">Request body</span></span>
<span data-ttu-id="49bd7-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="49bd7-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="49bd7-127">响应</span><span class="sxs-lookup"><span data-stu-id="49bd7-127">Response</span></span>
<span data-ttu-id="49bd7-128">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [bookingCustomer](../resources/bookingcustomer.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="49bd7-128">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49bd7-129">示例</span><span class="sxs-lookup"><span data-stu-id="49bd7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49bd7-130">请求</span><span class="sxs-lookup"><span data-stu-id="49bd7-130">Request</span></span>
<span data-ttu-id="49bd7-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="49bd7-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49bd7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="49bd7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
# <a name="c"></a>[<span data-ttu-id="49bd7-133">C#</span><span class="sxs-lookup"><span data-stu-id="49bd7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49bd7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49bd7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49bd7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49bd7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="49bd7-136">响应</span><span class="sxs-lookup"><span data-stu-id="49bd7-136">Response</span></span>
<span data-ttu-id="49bd7-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="49bd7-137">The following is an example of the response.</span></span> <span data-ttu-id="49bd7-138">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="49bd7-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="49bd7-139">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49bd7-139">All of the properties will be returned from an actual call.</span></span>
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