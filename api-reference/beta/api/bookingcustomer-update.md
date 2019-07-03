---
title: 更新 bookingcustomer
description: 更新 bookingCustomer 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 56d0b4bf1c4ef7dbfc8a6878833afc4c9ebba5da
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439047"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="94239-103">更新 bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="94239-103">Update bookingcustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94239-104">更新[bookingCustomer](../resources/bookingcustomer.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94239-104">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="94239-105">权限</span><span class="sxs-lookup"><span data-stu-id="94239-105">Permissions</span></span>
<span data-ttu-id="94239-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94239-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="94239-108">Permission type</span></span>      | <span data-ttu-id="94239-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94239-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94239-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94239-110">Delegated (work or school account)</span></span> | <span data-ttu-id="94239-111">BookingsAppointment, 全部, 全部登记, 全部, 预订。 All</span><span class="sxs-lookup"><span data-stu-id="94239-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="94239-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94239-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94239-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="94239-113">Not supported.</span></span>   |
|<span data-ttu-id="94239-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="94239-114">Application</span></span> | <span data-ttu-id="94239-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94239-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="94239-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94239-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="94239-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="94239-117">Optional request headers</span></span>
| <span data-ttu-id="94239-118">名称</span><span class="sxs-lookup"><span data-stu-id="94239-118">Name</span></span>       | <span data-ttu-id="94239-119">说明</span><span class="sxs-lookup"><span data-stu-id="94239-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="94239-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="94239-120">Authorization</span></span>  | <span data-ttu-id="94239-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="94239-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="94239-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="94239-122">Request body</span></span>
<span data-ttu-id="94239-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="94239-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94239-126">属性</span><span class="sxs-lookup"><span data-stu-id="94239-126">Property</span></span>     | <span data-ttu-id="94239-127">类型</span><span class="sxs-lookup"><span data-stu-id="94239-127">Type</span></span>   |<span data-ttu-id="94239-128">说明</span><span class="sxs-lookup"><span data-stu-id="94239-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94239-129">displayName</span><span class="sxs-lookup"><span data-stu-id="94239-129">displayName</span></span>|<span data-ttu-id="94239-130">String</span><span class="sxs-lookup"><span data-stu-id="94239-130">String</span></span>|<span data-ttu-id="94239-131">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="94239-131">The name of the customer.</span></span>|
|<span data-ttu-id="94239-132">emailAddress</span><span class="sxs-lookup"><span data-stu-id="94239-132">emailAddress</span></span>|<span data-ttu-id="94239-133">String</span><span class="sxs-lookup"><span data-stu-id="94239-133">String</span></span>|<span data-ttu-id="94239-134">客户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="94239-134">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="94239-135">响应</span><span class="sxs-lookup"><span data-stu-id="94239-135">Response</span></span>
<span data-ttu-id="94239-136">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="94239-136">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="94239-137">示例</span><span class="sxs-lookup"><span data-stu-id="94239-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94239-138">请求</span><span class="sxs-lookup"><span data-stu-id="94239-138">Request</span></span>
<span data-ttu-id="94239-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="94239-139">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="94239-140">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="94239-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="94239-141">C#</span><span class="sxs-lookup"><span data-stu-id="94239-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingcustomer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="94239-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="94239-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingcustomer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="94239-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="94239-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingcustomer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="94239-144">响应</span><span class="sxs-lookup"><span data-stu-id="94239-144">Response</span></span>
<span data-ttu-id="94239-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="94239-145">The following is an example of the response.</span></span> <span data-ttu-id="94239-146">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="94239-146">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="94239-147">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="94239-147">All of the properties will be returned from an actual call.</span></span>
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
