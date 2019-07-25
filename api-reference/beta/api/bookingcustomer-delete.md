---
title: 删除 bookingCustomer
description: 删除指定的 bookingCustomer 对象。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 045f6eaf21ef400338ad2159c0a036d13bfb1c07
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865387"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="56689-103">删除 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="56689-103">Delete bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56689-104">删除指定的[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="56689-104">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="56689-105">权限</span><span class="sxs-lookup"><span data-stu-id="56689-105">Permissions</span></span>
<span data-ttu-id="56689-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56689-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56689-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="56689-108">Permission type</span></span>      | <span data-ttu-id="56689-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56689-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56689-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56689-110">Delegated (work or school account)</span></span> | <span data-ttu-id="56689-111">BookingsAppointment, 全部, 全部登记, 全部, 预订。 All</span><span class="sxs-lookup"><span data-stu-id="56689-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="56689-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56689-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56689-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="56689-113">Not supported.</span></span>   |
|<span data-ttu-id="56689-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="56689-114">Application</span></span> | <span data-ttu-id="56689-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="56689-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="56689-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56689-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="56689-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="56689-117">Request headers</span></span>
| <span data-ttu-id="56689-118">名称</span><span class="sxs-lookup"><span data-stu-id="56689-118">Name</span></span>       | <span data-ttu-id="56689-119">说明</span><span class="sxs-lookup"><span data-stu-id="56689-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="56689-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="56689-120">Authorization</span></span>  | <span data-ttu-id="56689-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="56689-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="56689-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="56689-122">Request body</span></span>
<span data-ttu-id="56689-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56689-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="56689-124">响应</span><span class="sxs-lookup"><span data-stu-id="56689-124">Response</span></span>
<span data-ttu-id="56689-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="56689-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56689-127">示例</span><span class="sxs-lookup"><span data-stu-id="56689-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56689-128">请求</span><span class="sxs-lookup"><span data-stu-id="56689-128">Request</span></span>
<span data-ttu-id="56689-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="56689-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="56689-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="56689-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="56689-131">C#</span><span class="sxs-lookup"><span data-stu-id="56689-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56689-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="56689-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="56689-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="56689-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="56689-134">Java</span><span class="sxs-lookup"><span data-stu-id="56689-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bookingcustomer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="56689-135">响应</span><span class="sxs-lookup"><span data-stu-id="56689-135">Response</span></span>
<span data-ttu-id="56689-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="56689-136">The following is an example of the response.</span></span> <span data-ttu-id="56689-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="56689-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="56689-138">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56689-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
