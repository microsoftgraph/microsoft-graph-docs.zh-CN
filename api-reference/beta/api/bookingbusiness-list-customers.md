---
title: 列出的客户
description: 获取 bookingCustomer 对象的列表。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: ac91295cc6ac0edf96980d20e97153cd7cac0a29
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524938"
---
# <a name="list-customers"></a><span data-ttu-id="5d74e-103">列出的客户</span><span class="sxs-lookup"><span data-stu-id="5d74e-103">List customers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d74e-104">获取[bookingCustomer](../resources/bookingcustomer.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5d74e-104">Get a list of [bookingCustomer](../resources/bookingcustomer.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="5d74e-105">权限</span><span class="sxs-lookup"><span data-stu-id="5d74e-105">Permissions</span></span>
<span data-ttu-id="5d74e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d74e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d74e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d74e-108">Permission type</span></span>      | <span data-ttu-id="5d74e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d74e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5d74e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d74e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="5d74e-111">Bookings.Read.All，BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="5d74e-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5d74e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d74e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d74e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d74e-113">Not supported.</span></span>   |
|<span data-ttu-id="5d74e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d74e-114">Application</span></span> | <span data-ttu-id="5d74e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d74e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5d74e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d74e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/customers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5d74e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5d74e-117">Optional query parameters</span></span>
<span data-ttu-id="5d74e-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5d74e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5d74e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d74e-119">Request headers</span></span>
| <span data-ttu-id="5d74e-120">名称</span><span class="sxs-lookup"><span data-stu-id="5d74e-120">Name</span></span>      |<span data-ttu-id="5d74e-121">说明</span><span class="sxs-lookup"><span data-stu-id="5d74e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5d74e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d74e-122">Authorization</span></span>  | <span data-ttu-id="5d74e-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5d74e-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d74e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d74e-124">Request body</span></span>
<span data-ttu-id="5d74e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5d74e-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5d74e-126">响应</span><span class="sxs-lookup"><span data-stu-id="5d74e-126">Response</span></span>
<span data-ttu-id="5d74e-127">如果成功，此方法返回`200 OK`响应代码和响应正文中的[bookingCustomer](../resources/bookingcustomer.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="5d74e-127">If successful, this method returns a `200 OK` response code and collection of [bookingCustomer](../resources/bookingcustomer.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5d74e-128">示例</span><span class="sxs-lookup"><span data-stu-id="5d74e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5d74e-129">请求</span><span class="sxs-lookup"><span data-stu-id="5d74e-129">Request</span></span>
<span data-ttu-id="5d74e-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5d74e-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_customers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
```
##### <a name="response"></a><span data-ttu-id="5d74e-131">响应</span><span class="sxs-lookup"><span data-stu-id="5d74e-131">Response</span></span>
<span data-ttu-id="5d74e-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5d74e-132">The following is an example of the response.</span></span> <span data-ttu-id="5d74e-133">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5d74e-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5d74e-134">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5d74e-134">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-list-customers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
