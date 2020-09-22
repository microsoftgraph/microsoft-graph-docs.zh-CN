---
title: 创建 bookingCustomer
description: 创建新的 bookingCustomer 对象。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 69187e27949e66606c26012e0ea10dc2742eeb0f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996597"
---
# <a name="create-bookingcustomer"></a><span data-ttu-id="4578c-103">创建 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="4578c-103">Create bookingCustomer</span></span>

<span data-ttu-id="4578c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4578c-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4578c-105">创建新的 [bookingCustomer](../resources/bookingcustomer.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4578c-105">Create a new [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4578c-106">权限</span><span class="sxs-lookup"><span data-stu-id="4578c-106">Permissions</span></span>
<span data-ttu-id="4578c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4578c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4578c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4578c-109">Permission type</span></span>      | <span data-ttu-id="4578c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4578c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4578c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4578c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="4578c-112">BookingsAppointment，全部，全部登记，全部，预订。 All</span><span class="sxs-lookup"><span data-stu-id="4578c-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4578c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4578c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4578c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4578c-114">Not supported.</span></span>   |
|<span data-ttu-id="4578c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4578c-115">Application</span></span> | <span data-ttu-id="4578c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4578c-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4578c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4578c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/customers

```
## <a name="request-headers"></a><span data-ttu-id="4578c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4578c-118">Request headers</span></span>
| <span data-ttu-id="4578c-119">名称</span><span class="sxs-lookup"><span data-stu-id="4578c-119">Name</span></span>       | <span data-ttu-id="4578c-120">说明</span><span class="sxs-lookup"><span data-stu-id="4578c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4578c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4578c-121">Authorization</span></span>  | <span data-ttu-id="4578c-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4578c-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4578c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="4578c-123">Request body</span></span>
<span data-ttu-id="4578c-124">在请求正文中，提供 [bookingCustomer](../resources/bookingcustomer.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4578c-124">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="4578c-125">响应</span><span class="sxs-lookup"><span data-stu-id="4578c-125">Response</span></span>
<span data-ttu-id="4578c-126">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和 [bookingCustomer](../resources/bookingcustomer.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4578c-126">If successful, this method returns `201, Created` response code and [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4578c-127">示例</span><span class="sxs-lookup"><span data-stu-id="4578c-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4578c-128">请求</span><span class="sxs-lookup"><span data-stu-id="4578c-128">Request</span></span>
<span data-ttu-id="4578c-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4578c-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4578c-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="4578c-130">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4578c-131">C#</span><span class="sxs-lookup"><span data-stu-id="4578c-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingcustomer-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4578c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4578c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingcustomer-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4578c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4578c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingcustomer-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4578c-134">在请求正文中，提供 [bookingCustomer](../resources/bookingcustomer.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4578c-134">In the request body, supply a JSON representation of [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4578c-135">响应</span><span class="sxs-lookup"><span data-stu-id="4578c-135">Response</span></span>
<span data-ttu-id="4578c-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4578c-136">The following is an example of the response.</span></span> <span data-ttu-id="4578c-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4578c-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4578c-138">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4578c-138">All of the properties will be returned from an actual call.</span></span>
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


