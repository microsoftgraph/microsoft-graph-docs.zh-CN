---
title: 更新 bookingbusiness
description: 更新 bookingBusiness 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a9713231b8d0556ff27ee872039a40f1eadcc0cd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865443"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="b50c9-103">更新 bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="b50c9-103">Update bookingbusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b50c9-104">更新[bookingBusiness](../resources/bookingbusiness.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b50c9-104">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="b50c9-105">权限</span><span class="sxs-lookup"><span data-stu-id="b50c9-105">Permissions</span></span>
<span data-ttu-id="b50c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b50c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b50c9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b50c9-108">Permission type</span></span>      | <span data-ttu-id="b50c9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b50c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b50c9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b50c9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b50c9-111">全部预订. 全部, 全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="b50c9-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b50c9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b50c9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b50c9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b50c9-113">Not supported.</span></span>   |
|<span data-ttu-id="b50c9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b50c9-114">Application</span></span> | <span data-ttu-id="b50c9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b50c9-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b50c9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b50c9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="b50c9-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="b50c9-117">Optional request headers</span></span>
| <span data-ttu-id="b50c9-118">名称</span><span class="sxs-lookup"><span data-stu-id="b50c9-118">Name</span></span>       | <span data-ttu-id="b50c9-119">说明</span><span class="sxs-lookup"><span data-stu-id="b50c9-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b50c9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b50c9-120">Authorization</span></span>  | <span data-ttu-id="b50c9-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b50c9-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b50c9-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="b50c9-122">Request body</span></span>
<span data-ttu-id="b50c9-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b50c9-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b50c9-126">属性</span><span class="sxs-lookup"><span data-stu-id="b50c9-126">Property</span></span>     | <span data-ttu-id="b50c9-127">类型</span><span class="sxs-lookup"><span data-stu-id="b50c9-127">Type</span></span>   |<span data-ttu-id="b50c9-128">说明</span><span class="sxs-lookup"><span data-stu-id="b50c9-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b50c9-129">address</span><span class="sxs-lookup"><span data-stu-id="b50c9-129">address</span></span>|[<span data-ttu-id="b50c9-130">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b50c9-130">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="b50c9-131">企业的街道地址。</span><span class="sxs-lookup"><span data-stu-id="b50c9-131">The street address of the business.</span></span>|
|<span data-ttu-id="b50c9-132">businessHours</span><span class="sxs-lookup"><span data-stu-id="b50c9-132">businessHours</span></span>|<span data-ttu-id="b50c9-133">[bookingWorkHours](../resources/bookingworkhours.md)集合</span><span class="sxs-lookup"><span data-stu-id="b50c9-133">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="b50c9-134">业务的运行时间。</span><span class="sxs-lookup"><span data-stu-id="b50c9-134">The hours of operation for the business.</span></span>|
|<span data-ttu-id="b50c9-135">businessType</span><span class="sxs-lookup"><span data-stu-id="b50c9-135">businessType</span></span>|<span data-ttu-id="b50c9-136">String</span><span class="sxs-lookup"><span data-stu-id="b50c9-136">String</span></span>|<span data-ttu-id="b50c9-137">企业的类型。</span><span class="sxs-lookup"><span data-stu-id="b50c9-137">The type of business.</span></span>|
|<span data-ttu-id="b50c9-138">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="b50c9-138">defaultCurrencyIso</span></span>|<span data-ttu-id="b50c9-139">String</span><span class="sxs-lookup"><span data-stu-id="b50c9-139">String</span></span>|<span data-ttu-id="b50c9-140">业务在 Microsoft 预订中所运行的货币的代码。</span><span class="sxs-lookup"><span data-stu-id="b50c9-140">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="b50c9-141">displayName</span><span class="sxs-lookup"><span data-stu-id="b50c9-141">displayName</span></span>|<span data-ttu-id="b50c9-142">字符串</span><span class="sxs-lookup"><span data-stu-id="b50c9-142">String</span></span>|<span data-ttu-id="b50c9-143">与客户进行交互的企业的名称。</span><span class="sxs-lookup"><span data-stu-id="b50c9-143">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="b50c9-144">email</span><span class="sxs-lookup"><span data-stu-id="b50c9-144">email</span></span>|<span data-ttu-id="b50c9-145">String</span><span class="sxs-lookup"><span data-stu-id="b50c9-145">String</span></span>|<span data-ttu-id="b50c9-146">企业的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b50c9-146">The email address for the business.</span></span>|
|<span data-ttu-id="b50c9-147">phone</span><span class="sxs-lookup"><span data-stu-id="b50c9-147">phone</span></span>|<span data-ttu-id="b50c9-148">String</span><span class="sxs-lookup"><span data-stu-id="b50c9-148">String</span></span>|<span data-ttu-id="b50c9-149">企业的电话号码。</span><span class="sxs-lookup"><span data-stu-id="b50c9-149">The telephone number for the business.</span></span>|
|<span data-ttu-id="b50c9-150">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="b50c9-150">schedulingPolicy</span></span>|[<span data-ttu-id="b50c9-151">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="b50c9-151">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="b50c9-152">指定如何为此公司创建预订。</span><span class="sxs-lookup"><span data-stu-id="b50c9-152">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="b50c9-153">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="b50c9-153">webSiteUrl</span></span>|<span data-ttu-id="b50c9-154">String</span><span class="sxs-lookup"><span data-stu-id="b50c9-154">String</span></span>|<span data-ttu-id="b50c9-155">业务网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="b50c9-155">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="b50c9-156">响应</span><span class="sxs-lookup"><span data-stu-id="b50c9-156">Response</span></span>
<span data-ttu-id="b50c9-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b50c9-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b50c9-159">示例</span><span class="sxs-lookup"><span data-stu-id="b50c9-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b50c9-160">请求</span><span class="sxs-lookup"><span data-stu-id="b50c9-160">Request</span></span>
<span data-ttu-id="b50c9-161">下面的示例更新业务电子邮件地址和日程安排策略, 将公司默认的预定时间段更改为一个小时, 并提前预订30天。</span><span class="sxs-lookup"><span data-stu-id="b50c9-161">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b50c9-162">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b50c9-162">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b50c9-163">C#</span><span class="sxs-lookup"><span data-stu-id="b50c9-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b50c9-164">Javascript</span><span class="sxs-lookup"><span data-stu-id="b50c9-164">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b50c9-165">目标-C</span><span class="sxs-lookup"><span data-stu-id="b50c9-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b50c9-166">Java</span><span class="sxs-lookup"><span data-stu-id="b50c9-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b50c9-167">响应</span><span class="sxs-lookup"><span data-stu-id="b50c9-167">Response</span></span>
<span data-ttu-id="b50c9-168">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b50c9-168">The following is an example of the response.</span></span> <span data-ttu-id="b50c9-169">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b50c9-169">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b50c9-170">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b50c9-170">All of the properties will be returned from an actual call.</span></span>
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
