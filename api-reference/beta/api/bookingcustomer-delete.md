---
title: 删除 bookingCustomer
description: 删除指定的 bookingCustomer 对象。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: f519783c6178a8bf0d26adc33c96dd96bc9681f8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987890"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="c6be4-103">删除 bookingCustomer</span><span class="sxs-lookup"><span data-stu-id="c6be4-103">Delete bookingCustomer</span></span>

<span data-ttu-id="c6be4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6be4-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6be4-105">删除指定的 [bookingCustomer](../resources/bookingcustomer.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6be4-105">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6be4-106">权限</span><span class="sxs-lookup"><span data-stu-id="c6be4-106">Permissions</span></span>
<span data-ttu-id="c6be4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6be4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6be4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6be4-109">Permission type</span></span>      | <span data-ttu-id="c6be4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6be4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6be4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6be4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c6be4-112">BookingsAppointment，全部，全部登记，全部，预订。 All</span><span class="sxs-lookup"><span data-stu-id="c6be4-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c6be4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6be4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6be4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6be4-114">Not supported.</span></span>   |
|<span data-ttu-id="c6be4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6be4-115">Application</span></span> | <span data-ttu-id="c6be4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6be4-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c6be4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6be4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="c6be4-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6be4-118">Request headers</span></span>
| <span data-ttu-id="c6be4-119">名称</span><span class="sxs-lookup"><span data-stu-id="c6be4-119">Name</span></span>       | <span data-ttu-id="c6be4-120">说明</span><span class="sxs-lookup"><span data-stu-id="c6be4-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c6be4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6be4-121">Authorization</span></span>  | <span data-ttu-id="c6be4-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c6be4-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6be4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6be4-123">Request body</span></span>
<span data-ttu-id="c6be4-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c6be4-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c6be4-125">响应</span><span class="sxs-lookup"><span data-stu-id="c6be4-125">Response</span></span>
<span data-ttu-id="c6be4-p102">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c6be4-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6be4-128">示例</span><span class="sxs-lookup"><span data-stu-id="c6be4-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6be4-129">请求</span><span class="sxs-lookup"><span data-stu-id="c6be4-129">Request</span></span>
<span data-ttu-id="c6be4-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c6be4-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c6be4-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6be4-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
# <a name="c"></a>[<span data-ttu-id="c6be4-132">C#</span><span class="sxs-lookup"><span data-stu-id="c6be4-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6be4-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6be4-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6be4-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6be4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c6be4-135">响应</span><span class="sxs-lookup"><span data-stu-id="c6be4-135">Response</span></span>
<span data-ttu-id="c6be4-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c6be4-136">The following is an example of the response.</span></span> <span data-ttu-id="c6be4-137">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c6be4-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c6be4-138">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c6be4-138">All of the properties will be returned from an actual call.</span></span>
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


