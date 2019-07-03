---
title: 创建 bookingCustomer
description: 创建新的 bookingCustomer 对象。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 5fa56ce58e148bb0edbb1a6ad9b83b9947cda7d8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439187"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="c695f-103">创建 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="c695f-103">Create bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c695f-104">创建新的[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c695f-104">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c695f-105">权限</span><span class="sxs-lookup"><span data-stu-id="c695f-105">Permissions</span></span>
<span data-ttu-id="c695f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c695f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c695f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c695f-108">Permission type</span></span>      | <span data-ttu-id="c695f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c695f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c695f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c695f-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c695f-111">BookingsAppointment, 全部, 全部登记, 全部, 预订。 All</span><span class="sxs-lookup"><span data-stu-id="c695f-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c695f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c695f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c695f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c695f-113">Not supported.</span></span>   |
|<span data-ttu-id="c695f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c695f-114">Application</span></span> | <span data-ttu-id="c695f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c695f-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c695f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c695f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="c695f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c695f-117">Request headers</span></span>
| <span data-ttu-id="c695f-118">名称</span><span class="sxs-lookup"><span data-stu-id="c695f-118">Name</span></span>       | <span data-ttu-id="c695f-119">说明</span><span class="sxs-lookup"><span data-stu-id="c695f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c695f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c695f-120">Authorization</span></span>  | <span data-ttu-id="c695f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c695f-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c695f-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="c695f-122">Request body</span></span>
<span data-ttu-id="c695f-123">在请求正文中, 提供[bookingCustomer](../resources/bookingcustomer.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c695f-123">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="c695f-124">响应</span><span class="sxs-lookup"><span data-stu-id="c695f-124">Response</span></span>
<span data-ttu-id="c695f-125">如果成功, 此方法在`201, Created`响应正文中返回响应代码和[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c695f-125">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c695f-126">示例</span><span class="sxs-lookup"><span data-stu-id="c695f-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c695f-127">请求</span><span class="sxs-lookup"><span data-stu-id="c695f-127">Request</span></span>
<span data-ttu-id="c695f-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c695f-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c695f-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c695f-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookingcustomer_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers
Content-type: application/json

{
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c695f-130">C#</span><span class="sxs-lookup"><span data-stu-id="c695f-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingcustomer-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c695f-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="c695f-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingcustomer-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c695f-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="c695f-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingcustomer-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c695f-133">在请求正文中, 提供[bookingCustomer](../resources/bookingcustomer.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c695f-133">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c695f-134">响应</span><span class="sxs-lookup"><span data-stu-id="c695f-134">Response</span></span>
<span data-ttu-id="c695f-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c695f-135">The following is an example of the response.</span></span> <span data-ttu-id="c695f-136">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c695f-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c695f-137">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c695f-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingCustomer"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/customers/$entity",
    "id": "36038f36-634e-44e4-9415-d7d59c2347aa",
    "displayName": "Joni Sherman",
    "emailAddress": "jonis@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
