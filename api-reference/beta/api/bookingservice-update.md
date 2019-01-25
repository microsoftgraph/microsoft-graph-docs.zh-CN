---
title: 更新 bookingservice
description: 更新中指定 bookingbusiness bookingService 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6049fe68eaa45597246bef1c1b11952e3c4a5d42
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519715"
---
# <a name="update-bookingservice"></a><span data-ttu-id="fa5c4-103">更新 bookingservice</span><span class="sxs-lookup"><span data-stu-id="fa5c4-103">Update bookingservice</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa5c4-104">更新中指定[bookingbusiness](../resources/bookingbusiness.md) [bookingService](../resources/bookingservice.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-104">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="fa5c4-105">以下是您可以将自定义服务的一些示例：</span><span class="sxs-lookup"><span data-stu-id="fa5c4-105">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="fa5c4-106">价格</span><span class="sxs-lookup"><span data-stu-id="fa5c4-106">Price</span></span>
- <span data-ttu-id="fa5c4-107">约会的典型长度</span><span class="sxs-lookup"><span data-stu-id="fa5c4-107">Typical length of an appointment</span></span>
- <span data-ttu-id="fa5c4-108">Reminders</span><span class="sxs-lookup"><span data-stu-id="fa5c4-108">Reminders</span></span>
- <span data-ttu-id="fa5c4-109">任何时候，只要缓冲区之前设置或完成维修之后</span><span class="sxs-lookup"><span data-stu-id="fa5c4-109">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="fa5c4-110">[计划策略](../resources/bookingschedulingpolicy.md)参数，如最低通知书籍或取消，以及是否客户可以选择的约会的特定人员成员。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-110">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa5c4-111">权限</span><span class="sxs-lookup"><span data-stu-id="fa5c4-111">Permissions</span></span>
<span data-ttu-id="fa5c4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa5c4-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa5c4-114">Permission type</span></span>      | <span data-ttu-id="fa5c4-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa5c4-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa5c4-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa5c4-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="fa5c4-117">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="fa5c4-117">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="fa5c4-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa5c4-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa5c4-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-119">Not supported.</span></span>   |
|<span data-ttu-id="fa5c4-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa5c4-120">Application</span></span> | <span data-ttu-id="fa5c4-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fa5c4-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa5c4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="fa5c4-123">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="fa5c4-123">Optional request headers</span></span>
| <span data-ttu-id="fa5c4-124">名称</span><span class="sxs-lookup"><span data-stu-id="fa5c4-124">Name</span></span>       | <span data-ttu-id="fa5c4-125">说明</span><span class="sxs-lookup"><span data-stu-id="fa5c4-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fa5c4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa5c4-126">Authorization</span></span>  | <span data-ttu-id="fa5c4-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fa5c4-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa5c4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa5c4-128">Request body</span></span>
<span data-ttu-id="fa5c4-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fa5c4-132">属性</span><span class="sxs-lookup"><span data-stu-id="fa5c4-132">Property</span></span>     | <span data-ttu-id="fa5c4-133">类型</span><span class="sxs-lookup"><span data-stu-id="fa5c4-133">Type</span></span>   |<span data-ttu-id="fa5c4-134">说明</span><span class="sxs-lookup"><span data-stu-id="fa5c4-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa5c4-135">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="fa5c4-135">defaultDuration</span></span>|<span data-ttu-id="fa5c4-136">持续时间</span><span class="sxs-lookup"><span data-stu-id="fa5c4-136">Duration</span></span>|<span data-ttu-id="fa5c4-137">默认服务中的天、 小时、 分钟和秒数字表示的长度。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-137">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="fa5c4-138">例如，P11D23H59M59.999999999999S。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-138">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="fa5c4-139">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="fa5c4-139">defaultLocation</span></span>|[<span data-ttu-id="fa5c4-140">location</span><span class="sxs-lookup"><span data-stu-id="fa5c4-140">location</span></span>](../resources/location.md)|<span data-ttu-id="fa5c4-141">服务的默认物理位置。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-141">The default physical location for the service.</span></span>|
|<span data-ttu-id="fa5c4-142">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="fa5c4-142">defaultPrice</span></span>|<span data-ttu-id="fa5c4-143">双精度</span><span class="sxs-lookup"><span data-stu-id="fa5c4-143">Double</span></span>|<span data-ttu-id="fa5c4-144">该服务默认货币价格。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-144">The default monetary price for the service.</span></span>|
|<span data-ttu-id="fa5c4-145">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="fa5c4-145">defaultPriceType</span></span>|<span data-ttu-id="fa5c4-146">string</span><span class="sxs-lookup"><span data-stu-id="fa5c4-146">string</span></span>|<span data-ttu-id="fa5c4-147">负责服务的默认方式。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-147">The default way the service is charged.</span></span> <span data-ttu-id="fa5c4-148">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-148">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="fa5c4-149">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="fa5c4-149">defaultReminders</span></span>|<span data-ttu-id="fa5c4-150">[bookingReminder](../resources/bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="fa5c4-150">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="fa5c4-151">默认设置的该服务的约会的提醒。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-151">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="fa5c4-152">此属性的值时，可仅读取此**bookingService**由其 id。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-152">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="fa5c4-153">说明</span><span class="sxs-lookup"><span data-stu-id="fa5c4-153">description</span></span>|<span data-ttu-id="fa5c4-154">字符串</span><span class="sxs-lookup"><span data-stu-id="fa5c4-154">String</span></span>|<span data-ttu-id="fa5c4-155">服务的文本说明。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-155">A text description for the service.</span></span>|
|<span data-ttu-id="fa5c4-156">displayName</span><span class="sxs-lookup"><span data-stu-id="fa5c4-156">displayName</span></span>|<span data-ttu-id="fa5c4-157">String</span><span class="sxs-lookup"><span data-stu-id="fa5c4-157">String</span></span>|<span data-ttu-id="fa5c4-158">服务名称。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-158">A service name.</span></span>|
|<span data-ttu-id="fa5c4-159">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fa5c4-159">emailAddress</span></span>|<span data-ttu-id="fa5c4-160">String</span><span class="sxs-lookup"><span data-stu-id="fa5c4-160">String</span></span>|<span data-ttu-id="fa5c4-161">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="fa5c4-161">An email address</span></span>|
|<span data-ttu-id="fa5c4-162">id</span><span class="sxs-lookup"><span data-stu-id="fa5c4-162">id</span></span>|<span data-ttu-id="fa5c4-163">String</span><span class="sxs-lookup"><span data-stu-id="fa5c4-163">String</span></span>| <span data-ttu-id="fa5c4-164">只读。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-164">Read-only.</span></span>|
|<span data-ttu-id="fa5c4-165">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="fa5c4-165">isHiddenFromCustomers</span></span>|<span data-ttu-id="fa5c4-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="fa5c4-166">Boolean</span></span>|<span data-ttu-id="fa5c4-167">True 表示该服务不是预定的客户。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-167">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="fa5c4-168">notes</span><span class="sxs-lookup"><span data-stu-id="fa5c4-168">notes</span></span>|<span data-ttu-id="fa5c4-169">String</span><span class="sxs-lookup"><span data-stu-id="fa5c4-169">String</span></span>|<span data-ttu-id="fa5c4-170">有关此服务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-170">Additional information about this service.</span></span>|
|<span data-ttu-id="fa5c4-171">后</span><span class="sxs-lookup"><span data-stu-id="fa5c4-171">postBuffer</span></span>|<span data-ttu-id="fa5c4-172">持续时间</span><span class="sxs-lookup"><span data-stu-id="fa5c4-172">Duration</span></span>|<span data-ttu-id="fa5c4-173">此服务的时间为缓冲区之后为约会结束，且在下一步之前客户约会可以为预约。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-173">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="fa5c4-174">缓冲区</span><span class="sxs-lookup"><span data-stu-id="fa5c4-174">preBuffer</span></span>|<span data-ttu-id="fa5c4-175">持续时间</span><span class="sxs-lookup"><span data-stu-id="fa5c4-175">Duration</span></span>|<span data-ttu-id="fa5c4-176">缓冲区之前可以启动此服务的约会的时间。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-176">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="fa5c4-177">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="fa5c4-177">schedulingPolicy</span></span>|[<span data-ttu-id="fa5c4-178">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="fa5c4-178">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="fa5c4-179">确定如何创建和管理服务此类型的约会的策略集。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-179">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="fa5c4-180">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="fa5c4-180">staffMemberIds</span></span>|<span data-ttu-id="fa5c4-181">String 集合</span><span class="sxs-lookup"><span data-stu-id="fa5c4-181">String collection</span></span>|<span data-ttu-id="fa5c4-182">表示这些[员工](../resources/bookingstaffmember.md)提供此服务。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-182">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="fa5c4-183">响应</span><span class="sxs-lookup"><span data-stu-id="fa5c4-183">Response</span></span>
<span data-ttu-id="fa5c4-p106">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fa5c4-186">示例</span><span class="sxs-lookup"><span data-stu-id="fa5c4-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa5c4-187">请求</span><span class="sxs-lookup"><span data-stu-id="fa5c4-187">Request</span></span>
<span data-ttu-id="fa5c4-188">下面的示例将更新指定的服务的持续时间。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-188">The following example updates the duration of the specified service.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingservice"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT30M"
}
```
##### <a name="response"></a><span data-ttu-id="fa5c4-189">响应</span><span class="sxs-lookup"><span data-stu-id="fa5c4-189">Response</span></span>
<span data-ttu-id="fa5c4-190">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fa5c4-190">The following is an example of the response.</span></span>
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
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
