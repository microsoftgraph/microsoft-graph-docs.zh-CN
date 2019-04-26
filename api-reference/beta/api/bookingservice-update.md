---
title: 更新 bookingservice
description: 更新指定 bookingbusiness 中的 bookingService 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 41bcc4b31735cefb162a03a8c5a3dfd82cc6364e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322464"
---
# <a name="update-bookingservice"></a><span data-ttu-id="b4105-103">更新 bookingservice</span><span class="sxs-lookup"><span data-stu-id="b4105-103">Update bookingservice</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4105-104">更新指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingService](../resources/bookingservice.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b4105-104">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="b4105-105">下面是可以为服务自定义的一些示例:</span><span class="sxs-lookup"><span data-stu-id="b4105-105">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="b4105-106">价格</span><span class="sxs-lookup"><span data-stu-id="b4105-106">Price</span></span>
- <span data-ttu-id="b4105-107">约会的典型长度</span><span class="sxs-lookup"><span data-stu-id="b4105-107">Typical length of an appointment</span></span>
- <span data-ttu-id="b4105-108">提醒</span><span class="sxs-lookup"><span data-stu-id="b4105-108">Reminders</span></span>
- <span data-ttu-id="b4105-109">在服务完成之前或结束前设置的任何时间缓冲</span><span class="sxs-lookup"><span data-stu-id="b4105-109">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="b4105-110">将策略参数 (如 "最低通知")[安排](../resources/bookingschedulingpolicy.md)为 "书籍" 或 "取消", 以及客户是否可以选择约会的特定员工成员。</span><span class="sxs-lookup"><span data-stu-id="b4105-110">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4105-111">权限</span><span class="sxs-lookup"><span data-stu-id="b4105-111">Permissions</span></span>
<span data-ttu-id="b4105-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4105-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4105-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4105-114">Permission type</span></span>      | <span data-ttu-id="b4105-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4105-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4105-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4105-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="b4105-117">全部预订. 全部, 全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="b4105-117">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b4105-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4105-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4105-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4105-119">Not supported.</span></span>   |
|<span data-ttu-id="b4105-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4105-120">Application</span></span> | <span data-ttu-id="b4105-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4105-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b4105-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4105-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="b4105-123">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="b4105-123">Optional request headers</span></span>
| <span data-ttu-id="b4105-124">名称</span><span class="sxs-lookup"><span data-stu-id="b4105-124">Name</span></span>       | <span data-ttu-id="b4105-125">说明</span><span class="sxs-lookup"><span data-stu-id="b4105-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b4105-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4105-126">Authorization</span></span>  | <span data-ttu-id="b4105-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b4105-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4105-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4105-128">Request body</span></span>
<span data-ttu-id="b4105-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b4105-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b4105-132">属性</span><span class="sxs-lookup"><span data-stu-id="b4105-132">Property</span></span>     | <span data-ttu-id="b4105-133">类型</span><span class="sxs-lookup"><span data-stu-id="b4105-133">Type</span></span>   |<span data-ttu-id="b4105-134">说明</span><span class="sxs-lookup"><span data-stu-id="b4105-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4105-135">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="b4105-135">defaultDuration</span></span>|<span data-ttu-id="b4105-136">持续时间</span><span class="sxs-lookup"><span data-stu-id="b4105-136">Duration</span></span>|<span data-ttu-id="b4105-137">服务的默认长度, 以天数、小时数、分钟数和秒数表示。</span><span class="sxs-lookup"><span data-stu-id="b4105-137">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="b4105-138">例如, p11d23h59m 59.999999999999 s。</span><span class="sxs-lookup"><span data-stu-id="b4105-138">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="b4105-139">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="b4105-139">defaultLocation</span></span>|[<span data-ttu-id="b4105-140">location</span><span class="sxs-lookup"><span data-stu-id="b4105-140">location</span></span>](../resources/location.md)|<span data-ttu-id="b4105-141">服务的默认物理位置。</span><span class="sxs-lookup"><span data-stu-id="b4105-141">The default physical location for the service.</span></span>|
|<span data-ttu-id="b4105-142">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="b4105-142">defaultPrice</span></span>|<span data-ttu-id="b4105-143">双精度</span><span class="sxs-lookup"><span data-stu-id="b4105-143">Double</span></span>|<span data-ttu-id="b4105-144">服务的默认货币价格。</span><span class="sxs-lookup"><span data-stu-id="b4105-144">The default monetary price for the service.</span></span>|
|<span data-ttu-id="b4105-145">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="b4105-145">defaultPriceType</span></span>|<span data-ttu-id="b4105-146">string</span><span class="sxs-lookup"><span data-stu-id="b4105-146">string</span></span>|<span data-ttu-id="b4105-147">服务收费的默认方式。</span><span class="sxs-lookup"><span data-stu-id="b4105-147">The default way the service is charged.</span></span> <span data-ttu-id="b4105-148">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="b4105-148">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="b4105-149">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="b4105-149">defaultReminders</span></span>|<span data-ttu-id="b4105-150">[bookingReminder](../resources/bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="b4105-150">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="b4105-151">此服务的约会的默认提醒集。</span><span class="sxs-lookup"><span data-stu-id="b4105-151">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="b4105-152">此属性的值仅在按 ID 读取此**bookingService**时可用。</span><span class="sxs-lookup"><span data-stu-id="b4105-152">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="b4105-153">说明</span><span class="sxs-lookup"><span data-stu-id="b4105-153">description</span></span>|<span data-ttu-id="b4105-154">String</span><span class="sxs-lookup"><span data-stu-id="b4105-154">String</span></span>|<span data-ttu-id="b4105-155">服务的文本说明。</span><span class="sxs-lookup"><span data-stu-id="b4105-155">A text description for the service.</span></span>|
|<span data-ttu-id="b4105-156">displayName</span><span class="sxs-lookup"><span data-stu-id="b4105-156">displayName</span></span>|<span data-ttu-id="b4105-157">字符串</span><span class="sxs-lookup"><span data-stu-id="b4105-157">String</span></span>|<span data-ttu-id="b4105-158">服务名称。</span><span class="sxs-lookup"><span data-stu-id="b4105-158">A service name.</span></span>|
|<span data-ttu-id="b4105-159">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b4105-159">emailAddress</span></span>|<span data-ttu-id="b4105-160">String</span><span class="sxs-lookup"><span data-stu-id="b4105-160">String</span></span>|<span data-ttu-id="b4105-161">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="b4105-161">An email address</span></span>|
|<span data-ttu-id="b4105-162">id</span><span class="sxs-lookup"><span data-stu-id="b4105-162">id</span></span>|<span data-ttu-id="b4105-163">String</span><span class="sxs-lookup"><span data-stu-id="b4105-163">String</span></span>| <span data-ttu-id="b4105-164">只读。</span><span class="sxs-lookup"><span data-stu-id="b4105-164">Read-only.</span></span>|
|<span data-ttu-id="b4105-165">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="b4105-165">isHiddenFromCustomers</span></span>|<span data-ttu-id="b4105-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4105-166">Boolean</span></span>|<span data-ttu-id="b4105-167">如果为 True, 则表示此服务不可供客户预订。</span><span class="sxs-lookup"><span data-stu-id="b4105-167">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="b4105-168">notes</span><span class="sxs-lookup"><span data-stu-id="b4105-168">notes</span></span>|<span data-ttu-id="b4105-169">String</span><span class="sxs-lookup"><span data-stu-id="b4105-169">String</span></span>|<span data-ttu-id="b4105-170">有关此服务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="b4105-170">Additional information about this service.</span></span>|
|<span data-ttu-id="b4105-171">postBuffer</span><span class="sxs-lookup"><span data-stu-id="b4105-171">postBuffer</span></span>|<span data-ttu-id="b4105-172">持续时间</span><span class="sxs-lookup"><span data-stu-id="b4105-172">Duration</span></span>|<span data-ttu-id="b4105-173">此服务的约会结束后以及下一个客户约会可以被预订前要缓冲的时间。</span><span class="sxs-lookup"><span data-stu-id="b4105-173">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="b4105-174">preBuffer</span><span class="sxs-lookup"><span data-stu-id="b4105-174">preBuffer</span></span>|<span data-ttu-id="b4105-175">持续时间</span><span class="sxs-lookup"><span data-stu-id="b4105-175">Duration</span></span>|<span data-ttu-id="b4105-176">在此服务的约会开始之前要缓冲的时间。</span><span class="sxs-lookup"><span data-stu-id="b4105-176">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="b4105-177">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="b4105-177">schedulingPolicy</span></span>|[<span data-ttu-id="b4105-178">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="b4105-178">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="b4105-179">确定应如何创建和管理此类服务的约会的一组策略。</span><span class="sxs-lookup"><span data-stu-id="b4105-179">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="b4105-180">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="b4105-180">staffMemberIds</span></span>|<span data-ttu-id="b4105-181">String 集合</span><span class="sxs-lookup"><span data-stu-id="b4105-181">String collection</span></span>|<span data-ttu-id="b4105-182">代表提供此服务的[教职员工成员](../resources/bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="b4105-182">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="b4105-183">响应</span><span class="sxs-lookup"><span data-stu-id="b4105-183">Response</span></span>
<span data-ttu-id="b4105-p106">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b4105-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b4105-186">示例</span><span class="sxs-lookup"><span data-stu-id="b4105-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4105-187">请求</span><span class="sxs-lookup"><span data-stu-id="b4105-187">Request</span></span>
<span data-ttu-id="b4105-188">下面的示例更新指定服务的持续时间。</span><span class="sxs-lookup"><span data-stu-id="b4105-188">The following example updates the duration of the specified service.</span></span>
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
##### <a name="response"></a><span data-ttu-id="b4105-189">响应</span><span class="sxs-lookup"><span data-stu-id="b4105-189">Response</span></span>
<span data-ttu-id="b4105-190">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b4105-190">The following is an example of the response.</span></span>
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
  "suppressions": []
}
-->
