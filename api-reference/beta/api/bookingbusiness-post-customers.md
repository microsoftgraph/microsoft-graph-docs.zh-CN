---
title: 创建 bookingCustomer
description: 创建新的 bookingCustomer 对象。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 49bdec773488d8c8f88116544e7351d34295ddd2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636084"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="67c62-103">创建 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="67c62-103">Create bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67c62-104">创建新的[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="67c62-104">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="67c62-105">权限</span><span class="sxs-lookup"><span data-stu-id="67c62-105">Permissions</span></span>
<span data-ttu-id="67c62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67c62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67c62-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="67c62-108">Permission type</span></span>      | <span data-ttu-id="67c62-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67c62-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67c62-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67c62-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="67c62-111">BookingsAppointment, 全部, 全部登记, 全部, 预订。 All</span><span class="sxs-lookup"><span data-stu-id="67c62-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="67c62-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67c62-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67c62-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="67c62-113">Not supported.</span></span>   |
|<span data-ttu-id="67c62-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="67c62-114">Application</span></span> | <span data-ttu-id="67c62-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="67c62-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="67c62-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67c62-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="67c62-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="67c62-117">Request headers</span></span>
| <span data-ttu-id="67c62-118">名称</span><span class="sxs-lookup"><span data-stu-id="67c62-118">Name</span></span>       | <span data-ttu-id="67c62-119">说明</span><span class="sxs-lookup"><span data-stu-id="67c62-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="67c62-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="67c62-120">Authorization</span></span>  | <span data-ttu-id="67c62-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="67c62-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="67c62-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="67c62-122">Request body</span></span>
<span data-ttu-id="67c62-123">在请求正文中, 提供[bookingCustomer](../resources/bookingcustomer.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67c62-123">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="67c62-124">响应</span><span class="sxs-lookup"><span data-stu-id="67c62-124">Response</span></span>
<span data-ttu-id="67c62-125">如果成功, 此方法在`201, Created`响应正文中返回响应代码和[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="67c62-125">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67c62-126">示例</span><span class="sxs-lookup"><span data-stu-id="67c62-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67c62-127">请求</span><span class="sxs-lookup"><span data-stu-id="67c62-127">Request</span></span>
<span data-ttu-id="67c62-128">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="67c62-128">The following is an example of the request.</span></span>
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
<span data-ttu-id="67c62-129">在请求正文中, 提供[bookingCustomer](../resources/bookingcustomer.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67c62-129">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="67c62-130">响应</span><span class="sxs-lookup"><span data-stu-id="67c62-130">Response</span></span>
<span data-ttu-id="67c62-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="67c62-131">The following is an example of the response.</span></span> <span data-ttu-id="67c62-132">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="67c62-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="67c62-133">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67c62-133">All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="67c62-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="67c62-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="67c62-135">语言</span><span class="sxs-lookup"><span data-stu-id="67c62-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_bookingcustomer_from_bookingbusiness-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="67c62-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="67c62-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_bookingcustomer_from_bookingbusiness-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingbusiness-post-customers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
