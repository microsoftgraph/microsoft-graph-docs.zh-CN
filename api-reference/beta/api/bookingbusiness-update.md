---
title: 更新 bookingbusiness
description: 更新 bookingBusiness 对象的属性。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 767d4b3a355c74f6941bd9d9d20579e1c0dcda23
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047845"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="57897-103">更新 bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="57897-103">Update bookingbusiness</span></span>

<span data-ttu-id="57897-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57897-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57897-105">更新 [bookingBusiness 对象](../resources/bookingbusiness.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="57897-105">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="57897-106">权限</span><span class="sxs-lookup"><span data-stu-id="57897-106">Permissions</span></span>
<span data-ttu-id="57897-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57897-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57897-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="57897-109">Permission type</span></span>      | <span data-ttu-id="57897-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57897-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="57897-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57897-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="57897-112">Bookings.ReadWrite.All、Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="57897-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="57897-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57897-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57897-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="57897-114">Not supported.</span></span>   |
|<span data-ttu-id="57897-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="57897-115">Application</span></span> | <span data-ttu-id="57897-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="57897-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="57897-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57897-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="57897-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="57897-118">Optional request headers</span></span>
| <span data-ttu-id="57897-119">名称</span><span class="sxs-lookup"><span data-stu-id="57897-119">Name</span></span>       | <span data-ttu-id="57897-120">说明</span><span class="sxs-lookup"><span data-stu-id="57897-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="57897-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="57897-121">Authorization</span></span>  | <span data-ttu-id="57897-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="57897-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="57897-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="57897-123">Request body</span></span>
<span data-ttu-id="57897-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="57897-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="57897-127">属性</span><span class="sxs-lookup"><span data-stu-id="57897-127">Property</span></span>     | <span data-ttu-id="57897-128">类型</span><span class="sxs-lookup"><span data-stu-id="57897-128">Type</span></span>   |<span data-ttu-id="57897-129">说明</span><span class="sxs-lookup"><span data-stu-id="57897-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57897-130">address</span><span class="sxs-lookup"><span data-stu-id="57897-130">address</span></span>|[<span data-ttu-id="57897-131">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="57897-131">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="57897-132">企业街道地址。</span><span class="sxs-lookup"><span data-stu-id="57897-132">The street address of the business.</span></span>|
|<span data-ttu-id="57897-133">businessHours</span><span class="sxs-lookup"><span data-stu-id="57897-133">businessHours</span></span>|<span data-ttu-id="57897-134">[bookingWorkHours](../resources/bookingworkhours.md) 集合</span><span class="sxs-lookup"><span data-stu-id="57897-134">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="57897-135">企业运营的小时数。</span><span class="sxs-lookup"><span data-stu-id="57897-135">The hours of operation for the business.</span></span>|
|<span data-ttu-id="57897-136">businessType</span><span class="sxs-lookup"><span data-stu-id="57897-136">businessType</span></span>|<span data-ttu-id="57897-137">String</span><span class="sxs-lookup"><span data-stu-id="57897-137">String</span></span>|<span data-ttu-id="57897-138">业务类型。</span><span class="sxs-lookup"><span data-stu-id="57897-138">The type of business.</span></span>|
|<span data-ttu-id="57897-139">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="57897-139">defaultCurrencyIso</span></span>|<span data-ttu-id="57897-140">String</span><span class="sxs-lookup"><span data-stu-id="57897-140">String</span></span>|<span data-ttu-id="57897-141">在 Microsoft Bookings 上运营业务的货币代码。</span><span class="sxs-lookup"><span data-stu-id="57897-141">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="57897-142">displayName</span><span class="sxs-lookup"><span data-stu-id="57897-142">displayName</span></span>|<span data-ttu-id="57897-143">String</span><span class="sxs-lookup"><span data-stu-id="57897-143">String</span></span>|<span data-ttu-id="57897-144">与客户交互的企业的名称。</span><span class="sxs-lookup"><span data-stu-id="57897-144">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="57897-145">email</span><span class="sxs-lookup"><span data-stu-id="57897-145">email</span></span>|<span data-ttu-id="57897-146">String</span><span class="sxs-lookup"><span data-stu-id="57897-146">String</span></span>|<span data-ttu-id="57897-147">企业的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="57897-147">The email address for the business.</span></span>|
|<span data-ttu-id="57897-148">phone</span><span class="sxs-lookup"><span data-stu-id="57897-148">phone</span></span>|<span data-ttu-id="57897-149">String</span><span class="sxs-lookup"><span data-stu-id="57897-149">String</span></span>|<span data-ttu-id="57897-150">企业的电话号码。</span><span class="sxs-lookup"><span data-stu-id="57897-150">The telephone number for the business.</span></span>|
|<span data-ttu-id="57897-151">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="57897-151">schedulingPolicy</span></span>|[<span data-ttu-id="57897-152">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="57897-152">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="57897-153">指定如何为此业务创建预订。</span><span class="sxs-lookup"><span data-stu-id="57897-153">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="57897-154">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="57897-154">webSiteUrl</span></span>|<span data-ttu-id="57897-155">String</span><span class="sxs-lookup"><span data-stu-id="57897-155">String</span></span>|<span data-ttu-id="57897-156">业务网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="57897-156">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="57897-157">响应</span><span class="sxs-lookup"><span data-stu-id="57897-157">Response</span></span>
<span data-ttu-id="57897-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="57897-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="57897-160">示例</span><span class="sxs-lookup"><span data-stu-id="57897-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="57897-161">请求</span><span class="sxs-lookup"><span data-stu-id="57897-161">Request</span></span>
<span data-ttu-id="57897-162">以下示例更新了企业电子邮件地址和日程安排策略，将业务默认预订时间段更改为一小时，并提前预定最多 30 天。</span><span class="sxs-lookup"><span data-stu-id="57897-162">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>

# <a name="http"></a>[<span data-ttu-id="57897-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="57897-163">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="57897-164">C#</span><span class="sxs-lookup"><span data-stu-id="57897-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="57897-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57897-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="57897-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="57897-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="57897-167">Java</span><span class="sxs-lookup"><span data-stu-id="57897-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingbusiness-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="57897-168">响应</span><span class="sxs-lookup"><span data-stu-id="57897-168">Response</span></span>
<span data-ttu-id="57897-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="57897-169">The following is an example of the response.</span></span> <span data-ttu-id="57897-170">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="57897-170">Note: The response object shown here might be shortened for readability.</span></span>
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


