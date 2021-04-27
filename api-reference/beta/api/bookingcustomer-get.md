---
title: 获取 bookingCustomer
description: 获取 bookingCustomer 对象的属性和关系。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 77e2a1a44a973581524dd652a33f7e9a449512a4
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047824"
---
# <a name="get-bookingcustomer"></a><span data-ttu-id="5675a-103">获取 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="5675a-103">Get bookingCustomer</span></span>

<span data-ttu-id="5675a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5675a-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5675a-105">获取 [bookingCustomer](../resources/bookingcustomer.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5675a-105">Get the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5675a-106">权限</span><span class="sxs-lookup"><span data-stu-id="5675a-106">Permissions</span></span>
<span data-ttu-id="5675a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5675a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5675a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5675a-109">Permission type</span></span>      | <span data-ttu-id="5675a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5675a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5675a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5675a-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="5675a-112">Bookings.Read.All、BookingsAppointment.ReadWrite.All、Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="5675a-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5675a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5675a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5675a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5675a-114">Not supported.</span></span>   |
|<span data-ttu-id="5675a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5675a-115">Application</span></span> | <span data-ttu-id="5675a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5675a-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5675a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5675a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5675a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5675a-118">Optional query parameters</span></span>
<span data-ttu-id="5675a-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5675a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5675a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5675a-120">Request headers</span></span>
| <span data-ttu-id="5675a-121">名称</span><span class="sxs-lookup"><span data-stu-id="5675a-121">Name</span></span>      |<span data-ttu-id="5675a-122">说明</span><span class="sxs-lookup"><span data-stu-id="5675a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5675a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5675a-123">Authorization</span></span>  | <span data-ttu-id="5675a-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5675a-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5675a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5675a-125">Request body</span></span>
<span data-ttu-id="5675a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5675a-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5675a-127">响应</span><span class="sxs-lookup"><span data-stu-id="5675a-127">Response</span></span>
<span data-ttu-id="5675a-128">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [bookingCustomer](../resources/bookingcustomer.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5675a-128">If successful, this method returns a `200 OK` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5675a-129">示例</span><span class="sxs-lookup"><span data-stu-id="5675a-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5675a-130">请求</span><span class="sxs-lookup"><span data-stu-id="5675a-130">Request</span></span>
<span data-ttu-id="5675a-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5675a-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5675a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5675a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingcustomer"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
```
# <a name="c"></a>[<span data-ttu-id="5675a-133">C#</span><span class="sxs-lookup"><span data-stu-id="5675a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5675a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5675a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5675a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5675a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5675a-136">Java</span><span class="sxs-lookup"><span data-stu-id="5675a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5675a-137">响应</span><span class="sxs-lookup"><span data-stu-id="5675a-137">Response</span></span>
<span data-ttu-id="5675a-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5675a-138">The following is an example of the response.</span></span> <span data-ttu-id="5675a-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5675a-139">Note: The response object shown here might be shortened for readability.</span></span>
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
