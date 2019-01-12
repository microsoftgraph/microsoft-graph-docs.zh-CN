---
title: 列出的客户
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: de40a68981c7cf158b9082e93124f119d44d3ca0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946915"
---
# <a name="list-customers"></a><span data-ttu-id="c45c0-104">列出的客户</span><span class="sxs-lookup"><span data-stu-id="c45c0-104">List customers</span></span>

 > <span data-ttu-id="c45c0-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c45c0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c45c0-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c45c0-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="c45c0-107">获取[bookingCustomer](../resources/bookingcustomer.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c45c0-107">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="c45c0-108">权限</span><span class="sxs-lookup"><span data-stu-id="c45c0-108">Permissions</span></span>
<span data-ttu-id="c45c0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c45c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c45c0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c45c0-111">Permission type</span></span>      | <span data-ttu-id="c45c0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c45c0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c45c0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c45c0-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c45c0-114">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="c45c0-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c45c0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c45c0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c45c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c45c0-116">Not supported.</span></span>   |
|<span data-ttu-id="c45c0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c45c0-117">Application</span></span> | <span data-ttu-id="c45c0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c45c0-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="c45c0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c45c0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c45c0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c45c0-120">Optional query parameters</span></span>
<span data-ttu-id="c45c0-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c45c0-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c45c0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c45c0-122">Request headers</span></span>
| <span data-ttu-id="c45c0-123">名称</span><span class="sxs-lookup"><span data-stu-id="c45c0-123">Name</span></span>      |<span data-ttu-id="c45c0-124">说明</span><span class="sxs-lookup"><span data-stu-id="c45c0-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c45c0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c45c0-125">Authorization</span></span>  | <span data-ttu-id="c45c0-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c45c0-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c45c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c45c0-127">Request body</span></span>
<span data-ttu-id="c45c0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c45c0-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c45c0-129">响应</span><span class="sxs-lookup"><span data-stu-id="c45c0-129">Response</span></span>
<span data-ttu-id="c45c0-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[bookingCustomer](../resources/bookingcustomer.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="c45c0-130">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c45c0-131">示例</span><span class="sxs-lookup"><span data-stu-id="c45c0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c45c0-132">请求</span><span class="sxs-lookup"><span data-stu-id="c45c0-132">Request</span></span>
<span data-ttu-id="c45c0-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c45c0-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
##### <a name="response"></a><span data-ttu-id="c45c0-134">响应</span><span class="sxs-lookup"><span data-stu-id="c45c0-134">Response</span></span>
<span data-ttu-id="c45c0-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c45c0-135">The following is an example of the response.</span></span> <span data-ttu-id="c45c0-136">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c45c0-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c45c0-137">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c45c0-137">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List customers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
