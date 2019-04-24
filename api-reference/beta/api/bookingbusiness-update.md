---
title: 更新 bookingbusiness
description: 更新 bookingBusiness 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: dba24dafef030ae53fc83fb06d1cc7b99ed71e81
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461624"
---
# <a name="update-bookingbusiness"></a><span data-ttu-id="f0426-103">更新 bookingbusiness</span><span class="sxs-lookup"><span data-stu-id="f0426-103">Update bookingbusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0426-104">更新[bookingBusiness](../resources/bookingbusiness.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f0426-104">Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f0426-105">权限</span><span class="sxs-lookup"><span data-stu-id="f0426-105">Permissions</span></span>
<span data-ttu-id="f0426-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0426-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0426-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0426-108">Permission type</span></span>      | <span data-ttu-id="f0426-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0426-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0426-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0426-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f0426-111">全部预订. 全部, 全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="f0426-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f0426-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0426-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0426-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0426-113">Not supported.</span></span>   |
|<span data-ttu-id="f0426-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0426-114">Application</span></span> | <span data-ttu-id="f0426-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0426-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f0426-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0426-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/<id>
```
## <a name="optional-request-headers"></a><span data-ttu-id="f0426-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="f0426-117">Optional request headers</span></span>
| <span data-ttu-id="f0426-118">名称</span><span class="sxs-lookup"><span data-stu-id="f0426-118">Name</span></span>       | <span data-ttu-id="f0426-119">说明</span><span class="sxs-lookup"><span data-stu-id="f0426-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f0426-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0426-120">Authorization</span></span>  | <span data-ttu-id="f0426-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f0426-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0426-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0426-122">Request body</span></span>
<span data-ttu-id="f0426-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="f0426-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f0426-126">属性</span><span class="sxs-lookup"><span data-stu-id="f0426-126">Property</span></span>     | <span data-ttu-id="f0426-127">类型</span><span class="sxs-lookup"><span data-stu-id="f0426-127">Type</span></span>   |<span data-ttu-id="f0426-128">说明</span><span class="sxs-lookup"><span data-stu-id="f0426-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0426-129">address</span><span class="sxs-lookup"><span data-stu-id="f0426-129">address</span></span>|[<span data-ttu-id="f0426-130">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="f0426-130">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="f0426-131">企业的街道地址。</span><span class="sxs-lookup"><span data-stu-id="f0426-131">The street address of the business.</span></span>|
|<span data-ttu-id="f0426-132">businessHours</span><span class="sxs-lookup"><span data-stu-id="f0426-132">businessHours</span></span>|<span data-ttu-id="f0426-133">[bookingWorkHours](../resources/bookingworkhours.md)集合</span><span class="sxs-lookup"><span data-stu-id="f0426-133">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="f0426-134">业务的运行时间。</span><span class="sxs-lookup"><span data-stu-id="f0426-134">The hours of operation for the business.</span></span>|
|<span data-ttu-id="f0426-135">businessType</span><span class="sxs-lookup"><span data-stu-id="f0426-135">businessType</span></span>|<span data-ttu-id="f0426-136">字符串</span><span class="sxs-lookup"><span data-stu-id="f0426-136">String</span></span>|<span data-ttu-id="f0426-137">企业的类型。</span><span class="sxs-lookup"><span data-stu-id="f0426-137">The type of business.</span></span>|
|<span data-ttu-id="f0426-138">defaultCurrencyIso</span><span class="sxs-lookup"><span data-stu-id="f0426-138">defaultCurrencyIso</span></span>|<span data-ttu-id="f0426-139">字符串</span><span class="sxs-lookup"><span data-stu-id="f0426-139">String</span></span>|<span data-ttu-id="f0426-140">业务在 Microsoft 预订中所运行的货币的代码。</span><span class="sxs-lookup"><span data-stu-id="f0426-140">The code for the currency that the business operates in on Microsoft Bookings.</span></span>|
|<span data-ttu-id="f0426-141">displayName</span><span class="sxs-lookup"><span data-stu-id="f0426-141">displayName</span></span>|<span data-ttu-id="f0426-142">String</span><span class="sxs-lookup"><span data-stu-id="f0426-142">String</span></span>|<span data-ttu-id="f0426-143">与客户进行交互的企业的名称。</span><span class="sxs-lookup"><span data-stu-id="f0426-143">A name for the business that interfaces with customers.</span></span>|
|<span data-ttu-id="f0426-144">email</span><span class="sxs-lookup"><span data-stu-id="f0426-144">email</span></span>|<span data-ttu-id="f0426-145">字符串</span><span class="sxs-lookup"><span data-stu-id="f0426-145">String</span></span>|<span data-ttu-id="f0426-146">企业的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f0426-146">The email address for the business.</span></span>|
|<span data-ttu-id="f0426-147">phone</span><span class="sxs-lookup"><span data-stu-id="f0426-147">phone</span></span>|<span data-ttu-id="f0426-148">String</span><span class="sxs-lookup"><span data-stu-id="f0426-148">String</span></span>|<span data-ttu-id="f0426-149">企业的电话号码。</span><span class="sxs-lookup"><span data-stu-id="f0426-149">The telephone number for the business.</span></span>|
|<span data-ttu-id="f0426-150">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="f0426-150">schedulingPolicy</span></span>|[<span data-ttu-id="f0426-151">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="f0426-151">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="f0426-152">指定如何为此公司创建预订。</span><span class="sxs-lookup"><span data-stu-id="f0426-152">Specifies how bookings can be created for this business.</span></span>|
|<span data-ttu-id="f0426-153">webSiteUrl</span><span class="sxs-lookup"><span data-stu-id="f0426-153">webSiteUrl</span></span>|<span data-ttu-id="f0426-154">字符串</span><span class="sxs-lookup"><span data-stu-id="f0426-154">String</span></span>|<span data-ttu-id="f0426-155">业务网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="f0426-155">The URL of the business web site.</span></span>|

## <a name="response"></a><span data-ttu-id="f0426-156">响应</span><span class="sxs-lookup"><span data-stu-id="f0426-156">Response</span></span>
<span data-ttu-id="f0426-p103">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f0426-p103">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f0426-159">示例</span><span class="sxs-lookup"><span data-stu-id="f0426-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0426-160">请求</span><span class="sxs-lookup"><span data-stu-id="f0426-160">Request</span></span>
<span data-ttu-id="f0426-161">下面的示例更新业务电子邮件地址和日程安排策略, 将公司默认的预定时间段更改为一个小时, 并提前预订30天。</span><span class="sxs-lookup"><span data-stu-id="f0426-161">The following example updates the business email address and scheduling policy, to change the business default booking time slot to an hour, and advance booking up to 30 days.</span></span>
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
##### <a name="response"></a><span data-ttu-id="f0426-162">响应</span><span class="sxs-lookup"><span data-stu-id="f0426-162">Response</span></span>
<span data-ttu-id="f0426-163">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f0426-163">The following is an example of the response.</span></span> <span data-ttu-id="f0426-164">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f0426-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f0426-165">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f0426-165">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
