---
title: 更新 bookingbusiness
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: c0d92e0ddf792e28cb488cf466a1462272086c8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043372"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="4645f-104">更新 bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="4645f-104">Update bookingbusiness</span></span>

 > <span data-ttu-id="4645f-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4645f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4645f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4645f-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="4645f-107">更新[bookingBusiness](../resources/bookingbusiness.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4645f-107">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4645f-108">权限</span><span class="sxs-lookup"><span data-stu-id="4645f-108">Permissions</span></span>
<span data-ttu-id="4645f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4645f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4645f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4645f-111">Permission type</span></span>      | <span data-ttu-id="4645f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4645f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4645f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4645f-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="4645f-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="4645f-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4645f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4645f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4645f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4645f-116">Not supported.</span></span>   |
|<span data-ttu-id="4645f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4645f-117">Application</span></span> | <span data-ttu-id="4645f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4645f-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="4645f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4645f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="4645f-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="4645f-120">Optional request headers</span></span>
| <span data-ttu-id="4645f-121">名称</span><span class="sxs-lookup"><span data-stu-id="4645f-121">Name</span></span>       | <span data-ttu-id="4645f-122">说明</span><span class="sxs-lookup"><span data-stu-id="4645f-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4645f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4645f-123">Authorization</span></span>  | <span data-ttu-id="4645f-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4645f-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4645f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4645f-125">Request body</span></span>
<span data-ttu-id="4645f-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4645f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4645f-129">属性</span><span class="sxs-lookup"><span data-stu-id="4645f-129">Property</span></span>     | <span data-ttu-id="4645f-130">类型</span><span class="sxs-lookup"><span data-stu-id="4645f-130">Type</span></span>   |<span data-ttu-id="4645f-131">说明</span><span class="sxs-lookup"><span data-stu-id="4645f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4645f-132">address</span><span class="sxs-lookup"><span data-stu-id="4645f-132">address</span></span>|[<span data-ttu-id="4645f-133">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="4645f-133">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="4645f-134">业务街道地址。</span><span class="sxs-lookup"><span data-stu-id="4645f-134">The street address of the business.</span></span>|
|<span data-ttu-id="4645f-135">工作时间</span><span class="sxs-lookup"><span data-stu-id="4645f-135">businessHours</span></span>|<span data-ttu-id="4645f-136">[bookingWorkHours](../resources/bookingworkhours.md)集合</span><span class="sxs-lookup"><span data-stu-id="4645f-136">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="4645f-137">业务操作的时间点。</span><span class="sxs-lookup"><span data-stu-id="4645f-137">The hours of operation for the business.</span></span>|
|<span data-ttu-id="4645f-138">businessType</span><span class="sxs-lookup"><span data-stu-id="4645f-138">businessType</span></span>|<span data-ttu-id="4645f-139">字符串</span><span class="sxs-lookup"><span data-stu-id="4645f-139">String</span></span>|<span data-ttu-id="4645f-140">业务类型。</span><span class="sxs-lookup"><span data-stu-id="4645f-140">The type of business.</span></span>|
|<span data-ttu-id="4645f-141">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="4645f-141">defaultCurrencyIso</span></span>|<span data-ttu-id="4645f-142">字符串</span><span class="sxs-lookup"><span data-stu-id="4645f-142">String</span></span>|<span data-ttu-id="4645f-143">企业中运行 Microsoft 预订的货币代码。</span><span class="sxs-lookup"><span data-stu-id="4645f-143">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="4645f-144">displayName</span><span class="sxs-lookup"><span data-stu-id="4645f-144">displayName</span></span>|<span data-ttu-id="4645f-145">字符串</span><span class="sxs-lookup"><span data-stu-id="4645f-145">String</span></span>|<span data-ttu-id="4645f-146">接口与客户的业务名称。</span><span class="sxs-lookup"><span data-stu-id="4645f-146">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="4645f-147">email</span><span class="sxs-lookup"><span data-stu-id="4645f-147">email</span></span>|<span data-ttu-id="4645f-148">字符串</span><span class="sxs-lookup"><span data-stu-id="4645f-148">String</span></span>|<span data-ttu-id="4645f-149">业务电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="4645f-149">The email address for the business.</span></span>|
|<span data-ttu-id="4645f-150">phone</span><span class="sxs-lookup"><span data-stu-id="4645f-150">phone</span></span>|<span data-ttu-id="4645f-151">String</span><span class="sxs-lookup"><span data-stu-id="4645f-151">String</span></span>|<span data-ttu-id="4645f-152">业务电话号码。</span><span class="sxs-lookup"><span data-stu-id="4645f-152">The telephone number for the business.</span></span>|
|<span data-ttu-id="4645f-153">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="4645f-153">schedulingPolicy</span></span>|[<span data-ttu-id="4645f-154">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="4645f-154">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="4645f-155">指定如何创建此业务预订。</span><span class="sxs-lookup"><span data-stu-id="4645f-155">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="4645f-156">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="4645f-156">webSiteUrl</span></span>|<span data-ttu-id="4645f-157">字符串</span><span class="sxs-lookup"><span data-stu-id="4645f-157">String</span></span>|<span data-ttu-id="4645f-158">业务网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="4645f-158">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="4645f-159">响应</span><span class="sxs-lookup"><span data-stu-id="4645f-159">Response</span></span>
<span data-ttu-id="4645f-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4645f-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4645f-162">示例</span><span class="sxs-lookup"><span data-stu-id="4645f-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4645f-163">请求</span><span class="sxs-lookup"><span data-stu-id="4645f-163">Request</span></span>
<span data-ttu-id="4645f-164">下面的示例将更新的业务电子邮件地址和日程安排策略，更改为一个小时、 业务默认预定时间段和换预订最多 30 天。</span><span class="sxs-lookup"><span data-stu-id="4645f-164">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
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
##### <a name="response"></a><span data-ttu-id="4645f-165">响应</span><span class="sxs-lookup"><span data-stu-id="4645f-165">Response</span></span>
<span data-ttu-id="4645f-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4645f-166">The following is an example of the response.</span></span> <span data-ttu-id="4645f-167">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4645f-167">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4645f-168">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4645f-168">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingbusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->