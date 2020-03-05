---
title: 更新 bookingbusiness
description: 更新 bookingBusiness 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b150db37b78bb4c09bbaa1f1b91f569db754b352
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441142"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="b4752-103">更新 bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="b4752-103">Update bookingbusiness</span></span>

<span data-ttu-id="b4752-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b4752-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4752-105">更新[bookingBusiness](../resources/bookingbusiness.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b4752-105">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b4752-106">权限</span><span class="sxs-lookup"><span data-stu-id="b4752-106">Permissions</span></span>
<span data-ttu-id="b4752-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4752-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4752-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4752-109">Permission type</span></span>      | <span data-ttu-id="b4752-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4752-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4752-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4752-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="b4752-112">全部预订. 全部，全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="b4752-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b4752-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4752-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4752-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4752-114">Not supported.</span></span>   |
|<span data-ttu-id="b4752-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4752-115">Application</span></span> | <span data-ttu-id="b4752-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4752-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b4752-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4752-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b4752-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="b4752-118">Optional request headers</span></span>
| <span data-ttu-id="b4752-119">名称</span><span class="sxs-lookup"><span data-stu-id="b4752-119">Name</span></span>       | <span data-ttu-id="b4752-120">说明</span><span class="sxs-lookup"><span data-stu-id="b4752-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b4752-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4752-121">Authorization</span></span>  | <span data-ttu-id="b4752-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b4752-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4752-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4752-123">Request body</span></span>
<span data-ttu-id="b4752-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b4752-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b4752-127">属性</span><span class="sxs-lookup"><span data-stu-id="b4752-127">Property</span></span>     | <span data-ttu-id="b4752-128">类型</span><span class="sxs-lookup"><span data-stu-id="b4752-128">Type</span></span>   |<span data-ttu-id="b4752-129">说明</span><span class="sxs-lookup"><span data-stu-id="b4752-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4752-130">address</span><span class="sxs-lookup"><span data-stu-id="b4752-130">address</span></span>|[<span data-ttu-id="b4752-131">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b4752-131">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="b4752-132">企业的街道地址。</span><span class="sxs-lookup"><span data-stu-id="b4752-132">The street address of the business.</span></span>|
|<span data-ttu-id="b4752-133">businessHours</span><span class="sxs-lookup"><span data-stu-id="b4752-133">businessHours</span></span>|<span data-ttu-id="b4752-134">[bookingWorkHours](../resources/bookingworkhours.md)集合</span><span class="sxs-lookup"><span data-stu-id="b4752-134">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="b4752-135">业务的运行时间。</span><span class="sxs-lookup"><span data-stu-id="b4752-135">The hours of operation for the business.</span></span>|
|<span data-ttu-id="b4752-136">businessType</span><span class="sxs-lookup"><span data-stu-id="b4752-136">businessType</span></span>|<span data-ttu-id="b4752-137">String</span><span class="sxs-lookup"><span data-stu-id="b4752-137">String</span></span>|<span data-ttu-id="b4752-138">企业的类型。</span><span class="sxs-lookup"><span data-stu-id="b4752-138">The type of business.</span></span>|
|<span data-ttu-id="b4752-139">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="b4752-139">defaultCurrencyIso</span></span>|<span data-ttu-id="b4752-140">String</span><span class="sxs-lookup"><span data-stu-id="b4752-140">String</span></span>|<span data-ttu-id="b4752-141">业务在 Microsoft 预订中所运行的货币的代码。</span><span class="sxs-lookup"><span data-stu-id="b4752-141">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="b4752-142">displayName</span><span class="sxs-lookup"><span data-stu-id="b4752-142">displayName</span></span>|<span data-ttu-id="b4752-143">字符串</span><span class="sxs-lookup"><span data-stu-id="b4752-143">String</span></span>|<span data-ttu-id="b4752-144">与客户进行交互的企业的名称。</span><span class="sxs-lookup"><span data-stu-id="b4752-144">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="b4752-145">email</span><span class="sxs-lookup"><span data-stu-id="b4752-145">email</span></span>|<span data-ttu-id="b4752-146">String</span><span class="sxs-lookup"><span data-stu-id="b4752-146">String</span></span>|<span data-ttu-id="b4752-147">企业的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b4752-147">The email address for the business.</span></span>|
|<span data-ttu-id="b4752-148">phone</span><span class="sxs-lookup"><span data-stu-id="b4752-148">phone</span></span>|<span data-ttu-id="b4752-149">String</span><span class="sxs-lookup"><span data-stu-id="b4752-149">String</span></span>|<span data-ttu-id="b4752-150">企业的电话号码。</span><span class="sxs-lookup"><span data-stu-id="b4752-150">The telephone number for the business.</span></span>|
|<span data-ttu-id="b4752-151">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="b4752-151">schedulingPolicy</span></span>|[<span data-ttu-id="b4752-152">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="b4752-152">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="b4752-153">指定如何为此公司创建预订。</span><span class="sxs-lookup"><span data-stu-id="b4752-153">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="b4752-154">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="b4752-154">webSiteUrl</span></span>|<span data-ttu-id="b4752-155">String</span><span class="sxs-lookup"><span data-stu-id="b4752-155">String</span></span>|<span data-ttu-id="b4752-156">业务网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="b4752-156">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="b4752-157">响应</span><span class="sxs-lookup"><span data-stu-id="b4752-157">Response</span></span>
<span data-ttu-id="b4752-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b4752-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b4752-160">示例</span><span class="sxs-lookup"><span data-stu-id="b4752-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4752-161">请求</span><span class="sxs-lookup"><span data-stu-id="b4752-161">Request</span></span>
<span data-ttu-id="b4752-162">下面的示例更新业务电子邮件地址和日程安排策略，将公司默认的预定时间段更改为一个小时，并提前预订30天。</span><span class="sxs-lookup"><span data-stu-id="b4752-162">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>

# <a name="http"></a>[<span data-ttu-id="b4752-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4752-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingbusiness"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
Content-type: application/json

{
  "email": "admin@fabrikam.com",
  "schedulingPolicy": {
      "timeSlotInterval": "PT60M",
      "minimumLeadTime": "P1D",
      "maximumAdvance": "P30D",
      "sendConfirmationsToOwner": true,
      "allowStaffSelection": true
  }
}
```
# <a name="c"></a>[<span data-ttu-id="b4752-164">C#</span><span class="sxs-lookup"><span data-stu-id="b4752-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4752-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4752-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4752-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4752-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b4752-167">响应</span><span class="sxs-lookup"><span data-stu-id="b4752-167">Response</span></span>
<span data-ttu-id="b4752-168">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b4752-168">The following is an example of the response.</span></span> <span data-ttu-id="b4752-169">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b4752-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b4752-170">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4752-170">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
