---
title: 更新 bookingcustomer
description: 更新 bookingCustomer 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: c1af0dc924c923b9a9c0c2fa6093120ccbfa3cf7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441107"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="8a1d6-103">更新 bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="8a1d6-103">Update bookingcustomer</span></span>

<span data-ttu-id="8a1d6-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8a1d6-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a1d6-105">更新[bookingCustomer](../resources/bookingcustomer.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8a1d6-105">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8a1d6-106">权限</span><span class="sxs-lookup"><span data-stu-id="8a1d6-106">Permissions</span></span>
<span data-ttu-id="8a1d6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8a1d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a1d6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8a1d6-109">Permission type</span></span>      | <span data-ttu-id="8a1d6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8a1d6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a1d6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8a1d6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8a1d6-112">BookingsAppointment，全部，全部登记，全部，预订。 All</span><span class="sxs-lookup"><span data-stu-id="8a1d6-112">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8a1d6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8a1d6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a1d6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a1d6-114">Not supported.</span></span>   |
|<span data-ttu-id="8a1d6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8a1d6-115">Application</span></span> | <span data-ttu-id="8a1d6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8a1d6-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8a1d6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8a1d6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="8a1d6-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="8a1d6-118">Optional request headers</span></span>
| <span data-ttu-id="8a1d6-119">名称</span><span class="sxs-lookup"><span data-stu-id="8a1d6-119">Name</span></span>       | <span data-ttu-id="8a1d6-120">说明</span><span class="sxs-lookup"><span data-stu-id="8a1d6-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8a1d6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a1d6-121">Authorization</span></span>  | <span data-ttu-id="8a1d6-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="8a1d6-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a1d6-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8a1d6-123">Request body</span></span>
<span data-ttu-id="8a1d6-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="8a1d6-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8a1d6-127">属性</span><span class="sxs-lookup"><span data-stu-id="8a1d6-127">Property</span></span>     | <span data-ttu-id="8a1d6-128">类型</span><span class="sxs-lookup"><span data-stu-id="8a1d6-128">Type</span></span>   |<span data-ttu-id="8a1d6-129">说明</span><span class="sxs-lookup"><span data-stu-id="8a1d6-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a1d6-130">displayName</span><span class="sxs-lookup"><span data-stu-id="8a1d6-130">displayName</span></span>|<span data-ttu-id="8a1d6-131">String</span><span class="sxs-lookup"><span data-stu-id="8a1d6-131">String</span></span>|<span data-ttu-id="8a1d6-132">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="8a1d6-132">The name of the customer.</span></span>|
|<span data-ttu-id="8a1d6-133">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8a1d6-133">emailAddress</span></span>|<span data-ttu-id="8a1d6-134">String</span><span class="sxs-lookup"><span data-stu-id="8a1d6-134">String</span></span>|<span data-ttu-id="8a1d6-135">客户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="8a1d6-135">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="8a1d6-136">响应</span><span class="sxs-lookup"><span data-stu-id="8a1d6-136">Response</span></span>
<span data-ttu-id="8a1d6-137">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8a1d6-137">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8a1d6-138">示例</span><span class="sxs-lookup"><span data-stu-id="8a1d6-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8a1d6-139">请求</span><span class="sxs-lookup"><span data-stu-id="8a1d6-139">Request</span></span>
<span data-ttu-id="8a1d6-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8a1d6-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8a1d6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8a1d6-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingcustomer"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/8bb19078-0f45-4efb-b2c5-da78b860f73a
Content-type: application/json

{
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```
# <a name="c"></a>[<span data-ttu-id="8a1d6-142">C#</span><span class="sxs-lookup"><span data-stu-id="8a1d6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8a1d6-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8a1d6-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8a1d6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8a1d6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8a1d6-145">响应</span><span class="sxs-lookup"><span data-stu-id="8a1d6-145">Response</span></span>
<span data-ttu-id="8a1d6-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="8a1d6-146">The following is an example of the response.</span></span> <span data-ttu-id="8a1d6-147">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8a1d6-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8a1d6-148">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8a1d6-148">All of the properties will be returned from an actual call.</span></span>
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
    "displayName": "Adele",
    "emailAddress": "adele@relecloud.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
