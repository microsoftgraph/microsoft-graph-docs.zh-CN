---
title: 更新 bookingservice
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 6830ebc8fc101c4c9ce60f6157ed6bfdab82748c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937038"
---
# <a name="update-bookingservice"></a><span data-ttu-id="56347-104">更新 bookingservice</span><span class="sxs-lookup"><span data-stu-id="56347-104">Update bookingservice</span></span>

 > <span data-ttu-id="56347-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="56347-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56347-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="56347-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="56347-107">更新中指定[bookingbusiness](../resources/bookingbusiness.md) [bookingService](../resources/bookingservice.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="56347-107">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="56347-108">以下是您可以将自定义服务的一些示例：</span><span class="sxs-lookup"><span data-stu-id="56347-108">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="56347-109">Price</span><span class="sxs-lookup"><span data-stu-id="56347-109">Price</span></span>
- <span data-ttu-id="56347-110">约会的典型长度</span><span class="sxs-lookup"><span data-stu-id="56347-110">Typical length of an appointment</span></span>
- <span data-ttu-id="56347-111">Reminders</span><span class="sxs-lookup"><span data-stu-id="56347-111">Reminders</span></span>
- <span data-ttu-id="56347-112">任何时候，只要缓冲区之前设置或完成维修之后</span><span class="sxs-lookup"><span data-stu-id="56347-112">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="56347-113">[计划策略](../resources/bookingschedulingpolicy.md)参数，如最低通知书籍或取消，以及是否客户可以选择的约会的特定人员成员。</span><span class="sxs-lookup"><span data-stu-id="56347-113">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="56347-114">权限</span><span class="sxs-lookup"><span data-stu-id="56347-114">Permissions</span></span>
<span data-ttu-id="56347-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56347-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56347-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="56347-117">Permission type</span></span>      | <span data-ttu-id="56347-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56347-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56347-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56347-119">Delegated (work or school account)</span></span> |  <span data-ttu-id="56347-120">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="56347-120">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="56347-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56347-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56347-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="56347-122">Not supported.</span></span>   |
|<span data-ttu-id="56347-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="56347-123">Application</span></span> | <span data-ttu-id="56347-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="56347-124">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="56347-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56347-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="56347-126">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="56347-126">Optional request headers</span></span>
| <span data-ttu-id="56347-127">名称</span><span class="sxs-lookup"><span data-stu-id="56347-127">Name</span></span>       | <span data-ttu-id="56347-128">说明</span><span class="sxs-lookup"><span data-stu-id="56347-128">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="56347-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="56347-129">Authorization</span></span>  | <span data-ttu-id="56347-130">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="56347-130">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="56347-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="56347-131">Request body</span></span>
<span data-ttu-id="56347-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="56347-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="56347-135">属性</span><span class="sxs-lookup"><span data-stu-id="56347-135">Property</span></span>     | <span data-ttu-id="56347-136">类型</span><span class="sxs-lookup"><span data-stu-id="56347-136">Type</span></span>   |<span data-ttu-id="56347-137">说明</span><span class="sxs-lookup"><span data-stu-id="56347-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56347-138">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="56347-138">defaultDuration</span></span>|<span data-ttu-id="56347-139">Duration</span><span class="sxs-lookup"><span data-stu-id="56347-139">Duration</span></span>|<span data-ttu-id="56347-140">默认服务中的天、 小时、 分钟和秒数字表示的长度。</span><span class="sxs-lookup"><span data-stu-id="56347-140">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="56347-141">例如，P11D23H59M59.999999999999S。</span><span class="sxs-lookup"><span data-stu-id="56347-141">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="56347-142">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="56347-142">defaultLocation</span></span>|[<span data-ttu-id="56347-143">location</span><span class="sxs-lookup"><span data-stu-id="56347-143">location</span></span>](../resources/location.md)|<span data-ttu-id="56347-144">服务的默认物理位置。</span><span class="sxs-lookup"><span data-stu-id="56347-144">The default physical location for the service.</span></span>|
|<span data-ttu-id="56347-145">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="56347-145">defaultPrice</span></span>|<span data-ttu-id="56347-146">Double</span><span class="sxs-lookup"><span data-stu-id="56347-146">Double</span></span>|<span data-ttu-id="56347-147">该服务默认货币价格。</span><span class="sxs-lookup"><span data-stu-id="56347-147">The default monetary price for the service.</span></span>|
|<span data-ttu-id="56347-148">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="56347-148">defaultPriceType</span></span>|<span data-ttu-id="56347-149">string</span><span class="sxs-lookup"><span data-stu-id="56347-149">string</span></span>|<span data-ttu-id="56347-150">负责服务的默认方式。</span><span class="sxs-lookup"><span data-stu-id="56347-150">The default way the service is charged.</span></span> <span data-ttu-id="56347-151">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="56347-151">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="56347-152">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="56347-152">defaultReminders</span></span>|<span data-ttu-id="56347-153">[bookingReminder](../resources/bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="56347-153">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="56347-154">默认设置的该服务的约会的提醒。</span><span class="sxs-lookup"><span data-stu-id="56347-154">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="56347-155">此属性的值时，可仅读取此**bookingService**由其 id。</span><span class="sxs-lookup"><span data-stu-id="56347-155">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="56347-156">说明</span><span class="sxs-lookup"><span data-stu-id="56347-156">description</span></span>|<span data-ttu-id="56347-157">字符串</span><span class="sxs-lookup"><span data-stu-id="56347-157">String</span></span>|<span data-ttu-id="56347-158">服务的文本说明。</span><span class="sxs-lookup"><span data-stu-id="56347-158">A text description for the service.</span></span>|
|<span data-ttu-id="56347-159">displayName</span><span class="sxs-lookup"><span data-stu-id="56347-159">displayName</span></span>|<span data-ttu-id="56347-160">字符串</span><span class="sxs-lookup"><span data-stu-id="56347-160">String</span></span>|<span data-ttu-id="56347-161">服务名称。</span><span class="sxs-lookup"><span data-stu-id="56347-161">A service name.</span></span>|
|<span data-ttu-id="56347-162">emailAddress</span><span class="sxs-lookup"><span data-stu-id="56347-162">emailAddress</span></span>|<span data-ttu-id="56347-163">String</span><span class="sxs-lookup"><span data-stu-id="56347-163">String</span></span>|<span data-ttu-id="56347-164">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="56347-164">An email address</span></span>|
|<span data-ttu-id="56347-165">id</span><span class="sxs-lookup"><span data-stu-id="56347-165">id</span></span>|<span data-ttu-id="56347-166">String</span><span class="sxs-lookup"><span data-stu-id="56347-166">String</span></span>| <span data-ttu-id="56347-167">只读。</span><span class="sxs-lookup"><span data-stu-id="56347-167">Read-only.</span></span>|
|<span data-ttu-id="56347-168">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="56347-168">isHiddenFromCustomers</span></span>|<span data-ttu-id="56347-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="56347-169">Boolean</span></span>|<span data-ttu-id="56347-170">True 表示该服务不是预定的客户。</span><span class="sxs-lookup"><span data-stu-id="56347-170">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="56347-171">notes</span><span class="sxs-lookup"><span data-stu-id="56347-171">notes</span></span>|<span data-ttu-id="56347-172">String</span><span class="sxs-lookup"><span data-stu-id="56347-172">String</span></span>|<span data-ttu-id="56347-173">有关此服务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="56347-173">Additional information about this service.</span></span>|
|<span data-ttu-id="56347-174">后</span><span class="sxs-lookup"><span data-stu-id="56347-174">postBuffer</span></span>|<span data-ttu-id="56347-175">Duration</span><span class="sxs-lookup"><span data-stu-id="56347-175">Duration</span></span>|<span data-ttu-id="56347-176">此服务的时间为缓冲区之后为约会结束，且在下一步之前客户约会可以为预约。</span><span class="sxs-lookup"><span data-stu-id="56347-176">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="56347-177">缓冲区</span><span class="sxs-lookup"><span data-stu-id="56347-177">preBuffer</span></span>|<span data-ttu-id="56347-178">Duration</span><span class="sxs-lookup"><span data-stu-id="56347-178">Duration</span></span>|<span data-ttu-id="56347-179">缓冲区之前可以启动此服务的约会的时间。</span><span class="sxs-lookup"><span data-stu-id="56347-179">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="56347-180">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="56347-180">schedulingPolicy</span></span>|[<span data-ttu-id="56347-181">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="56347-181">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="56347-182">确定如何创建和管理服务此类型的约会的策略集。</span><span class="sxs-lookup"><span data-stu-id="56347-182">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="56347-183">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="56347-183">staffMemberIds</span></span>|<span data-ttu-id="56347-184">String 集合</span><span class="sxs-lookup"><span data-stu-id="56347-184">String collection</span></span>|<span data-ttu-id="56347-185">表示这些[员工](../resources/bookingstaffmember.md)提供此服务。</span><span class="sxs-lookup"><span data-stu-id="56347-185">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="56347-186">响应</span><span class="sxs-lookup"><span data-stu-id="56347-186">Response</span></span>
<span data-ttu-id="56347-p108">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="56347-p108">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56347-189">示例</span><span class="sxs-lookup"><span data-stu-id="56347-189">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56347-190">请求</span><span class="sxs-lookup"><span data-stu-id="56347-190">Request</span></span>
<span data-ttu-id="56347-191">下面的示例将更新指定的服务的持续时间。</span><span class="sxs-lookup"><span data-stu-id="56347-191">The following example updates the duration of the specified service.</span></span>
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
##### <a name="response"></a><span data-ttu-id="56347-192">响应</span><span class="sxs-lookup"><span data-stu-id="56347-192">Response</span></span>
<span data-ttu-id="56347-193">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="56347-193">The following is an example of the response.</span></span> 
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
  "description": "Update bookingservice",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
