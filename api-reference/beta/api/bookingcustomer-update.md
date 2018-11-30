---
title: 更新 bookingcustomer
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: d28a2a30da1c626c65c65a1dc3cab000a06580d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043019"
---
# <a name="update-bookingcustomer"></a><span data-ttu-id="dc974-104">更新 bookingcustomer</span><span class="sxs-lookup"><span data-stu-id="dc974-104">Update bookingcustomer</span></span>

 > <span data-ttu-id="dc974-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dc974-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc974-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dc974-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="dc974-107">更新[bookingCustomer](../resources/bookingcustomer.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dc974-107">Update the properties of a [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc974-108">权限</span><span class="sxs-lookup"><span data-stu-id="dc974-108">Permissions</span></span>
<span data-ttu-id="dc974-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc974-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc974-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc974-111">Permission type</span></span>      | <span data-ttu-id="dc974-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc974-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc974-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc974-113">Delegated (work or school account)</span></span> | <span data-ttu-id="dc974-114">BookingsAppointment.ReadWrite.All，Bookings.ReadWrite.All，Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="dc974-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="dc974-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc974-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc974-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc974-116">Not supported.</span></span>   |
|<span data-ttu-id="dc974-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc974-117">Application</span></span> | <span data-ttu-id="dc974-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc974-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="dc974-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc974-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/customers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="dc974-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="dc974-120">Optional request headers</span></span>
| <span data-ttu-id="dc974-121">名称</span><span class="sxs-lookup"><span data-stu-id="dc974-121">Name</span></span>       | <span data-ttu-id="dc974-122">说明</span><span class="sxs-lookup"><span data-stu-id="dc974-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="dc974-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc974-123">Authorization</span></span>  | <span data-ttu-id="dc974-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="dc974-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc974-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc974-125">Request body</span></span>
<span data-ttu-id="dc974-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="dc974-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="dc974-129">属性</span><span class="sxs-lookup"><span data-stu-id="dc974-129">Property</span></span>     | <span data-ttu-id="dc974-130">类型</span><span class="sxs-lookup"><span data-stu-id="dc974-130">Type</span></span>   |<span data-ttu-id="dc974-131">说明</span><span class="sxs-lookup"><span data-stu-id="dc974-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc974-132">displayName</span><span class="sxs-lookup"><span data-stu-id="dc974-132">displayName</span></span>|<span data-ttu-id="dc974-133">字符串</span><span class="sxs-lookup"><span data-stu-id="dc974-133">String</span></span>|<span data-ttu-id="dc974-134">客户的名称。</span><span class="sxs-lookup"><span data-stu-id="dc974-134">The name of the customer.</span></span>|
|<span data-ttu-id="dc974-135">emailAddress</span><span class="sxs-lookup"><span data-stu-id="dc974-135">emailAddress</span></span>|<span data-ttu-id="dc974-136">String</span><span class="sxs-lookup"><span data-stu-id="dc974-136">String</span></span>|<span data-ttu-id="dc974-137">客户的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="dc974-137">The SMTP address of the customer.</span></span>|

## <a name="response"></a><span data-ttu-id="dc974-138">响应</span><span class="sxs-lookup"><span data-stu-id="dc974-138">Response</span></span>
<span data-ttu-id="dc974-139">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[bookingCustomer](../resources/bookingcustomer.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dc974-139">If successful, this method returns a `200 OK` response code and updated [bookingCustomer](../resources/bookingcustomer.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dc974-140">示例</span><span class="sxs-lookup"><span data-stu-id="dc974-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc974-141">请求</span><span class="sxs-lookup"><span data-stu-id="dc974-141">Request</span></span>
<span data-ttu-id="dc974-142">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dc974-142">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="dc974-143">响应</span><span class="sxs-lookup"><span data-stu-id="dc974-143">Response</span></span>
<span data-ttu-id="dc974-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dc974-144">The following is an example of the response.</span></span> <span data-ttu-id="dc974-145">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dc974-145">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dc974-146">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dc974-146">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingcustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->