---
title: 更新 bookingservice
description: 更新指定 bookingbusiness 中的 bookingService 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 98bade824541db13810071bc2a256c3daf06a887
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262564"
---
# <a name="update-bookingservice"></a><span data-ttu-id="c5986-103">更新 bookingservice</span><span class="sxs-lookup"><span data-stu-id="c5986-103">Update bookingservice</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5986-104">更新指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingService](../resources/bookingservice.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c5986-104">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="c5986-105">下面是可以为服务自定义的一些示例:</span><span class="sxs-lookup"><span data-stu-id="c5986-105">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="c5986-106">价格</span><span class="sxs-lookup"><span data-stu-id="c5986-106">Price</span></span>
- <span data-ttu-id="c5986-107">约会的典型长度</span><span class="sxs-lookup"><span data-stu-id="c5986-107">Typical length of an appointment</span></span>
- <span data-ttu-id="c5986-108">提醒</span><span class="sxs-lookup"><span data-stu-id="c5986-108">Reminders</span></span>
- <span data-ttu-id="c5986-109">在服务完成之前或结束前设置的任何时间缓冲</span><span class="sxs-lookup"><span data-stu-id="c5986-109">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="c5986-110">将策略参数 (如 "最低通知")[安排](../resources/bookingschedulingpolicy.md)为 "书籍" 或 "取消", 以及客户是否可以选择约会的特定员工成员。</span><span class="sxs-lookup"><span data-stu-id="c5986-110">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5986-111">权限</span><span class="sxs-lookup"><span data-stu-id="c5986-111">Permissions</span></span>
<span data-ttu-id="c5986-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5986-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5986-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5986-114">Permission type</span></span>      | <span data-ttu-id="c5986-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5986-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5986-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5986-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="c5986-117">全部预订. 全部, 全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="c5986-117">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c5986-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5986-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5986-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5986-119">Not supported.</span></span>   |
|<span data-ttu-id="c5986-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5986-120">Application</span></span> | <span data-ttu-id="c5986-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5986-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c5986-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5986-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="c5986-123">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="c5986-123">Optional request headers</span></span>
| <span data-ttu-id="c5986-124">名称</span><span class="sxs-lookup"><span data-stu-id="c5986-124">Name</span></span>       | <span data-ttu-id="c5986-125">说明</span><span class="sxs-lookup"><span data-stu-id="c5986-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c5986-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5986-126">Authorization</span></span>  | <span data-ttu-id="c5986-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c5986-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5986-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5986-128">Request body</span></span>
<span data-ttu-id="c5986-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c5986-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c5986-132">属性</span><span class="sxs-lookup"><span data-stu-id="c5986-132">Property</span></span>     | <span data-ttu-id="c5986-133">类型</span><span class="sxs-lookup"><span data-stu-id="c5986-133">Type</span></span>   |<span data-ttu-id="c5986-134">说明</span><span class="sxs-lookup"><span data-stu-id="c5986-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5986-135">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="c5986-135">defaultDuration</span></span>|<span data-ttu-id="c5986-136">持续时间</span><span class="sxs-lookup"><span data-stu-id="c5986-136">Duration</span></span>|<span data-ttu-id="c5986-137">服务的默认长度, 以天数、小时数、分钟数和秒数表示。</span><span class="sxs-lookup"><span data-stu-id="c5986-137">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="c5986-138">例如, P11D23H59M 59.999999999999 S。</span><span class="sxs-lookup"><span data-stu-id="c5986-138">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="c5986-139">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="c5986-139">defaultLocation</span></span>|[<span data-ttu-id="c5986-140">location</span><span class="sxs-lookup"><span data-stu-id="c5986-140">location</span></span>](../resources/location.md)|<span data-ttu-id="c5986-141">服务的默认物理位置。</span><span class="sxs-lookup"><span data-stu-id="c5986-141">The default physical location for the service.</span></span>|
|<span data-ttu-id="c5986-142">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="c5986-142">defaultPrice</span></span>|<span data-ttu-id="c5986-143">双精度</span><span class="sxs-lookup"><span data-stu-id="c5986-143">Double</span></span>|<span data-ttu-id="c5986-144">服务的默认货币价格。</span><span class="sxs-lookup"><span data-stu-id="c5986-144">The default monetary price for the service.</span></span>|
|<span data-ttu-id="c5986-145">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="c5986-145">defaultPriceType</span></span>|<span data-ttu-id="c5986-146">string</span><span class="sxs-lookup"><span data-stu-id="c5986-146">string</span></span>|<span data-ttu-id="c5986-147">服务收费的默认方式。</span><span class="sxs-lookup"><span data-stu-id="c5986-147">The default way the service is charged.</span></span> <span data-ttu-id="c5986-148">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="c5986-148">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="c5986-149">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="c5986-149">defaultReminders</span></span>|<span data-ttu-id="c5986-150">[bookingReminder](../resources/bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="c5986-150">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="c5986-151">此服务的约会的默认提醒集。</span><span class="sxs-lookup"><span data-stu-id="c5986-151">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="c5986-152">此属性的值仅在按 ID 读取此**bookingService**时可用。</span><span class="sxs-lookup"><span data-stu-id="c5986-152">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="c5986-153">说明</span><span class="sxs-lookup"><span data-stu-id="c5986-153">description</span></span>|<span data-ttu-id="c5986-154">String</span><span class="sxs-lookup"><span data-stu-id="c5986-154">String</span></span>|<span data-ttu-id="c5986-155">服务的文本说明。</span><span class="sxs-lookup"><span data-stu-id="c5986-155">A text description for the service.</span></span>|
|<span data-ttu-id="c5986-156">displayName</span><span class="sxs-lookup"><span data-stu-id="c5986-156">displayName</span></span>|<span data-ttu-id="c5986-157">字符串</span><span class="sxs-lookup"><span data-stu-id="c5986-157">String</span></span>|<span data-ttu-id="c5986-158">服务名称。</span><span class="sxs-lookup"><span data-stu-id="c5986-158">A service name.</span></span>|
|<span data-ttu-id="c5986-159">emailAddress</span><span class="sxs-lookup"><span data-stu-id="c5986-159">emailAddress</span></span>|<span data-ttu-id="c5986-160">String</span><span class="sxs-lookup"><span data-stu-id="c5986-160">String</span></span>|<span data-ttu-id="c5986-161">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="c5986-161">An email address</span></span>|
|<span data-ttu-id="c5986-162">id</span><span class="sxs-lookup"><span data-stu-id="c5986-162">id</span></span>|<span data-ttu-id="c5986-163">String</span><span class="sxs-lookup"><span data-stu-id="c5986-163">String</span></span>| <span data-ttu-id="c5986-164">只读。</span><span class="sxs-lookup"><span data-stu-id="c5986-164">Read-only.</span></span>|
|<span data-ttu-id="c5986-165">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="c5986-165">isHiddenFromCustomers</span></span>|<span data-ttu-id="c5986-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5986-166">Boolean</span></span>|<span data-ttu-id="c5986-167">如果为 True, 则表示此服务不可供客户预订。</span><span class="sxs-lookup"><span data-stu-id="c5986-167">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="c5986-168">notes</span><span class="sxs-lookup"><span data-stu-id="c5986-168">notes</span></span>|<span data-ttu-id="c5986-169">String</span><span class="sxs-lookup"><span data-stu-id="c5986-169">String</span></span>|<span data-ttu-id="c5986-170">有关此服务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="c5986-170">Additional information about this service.</span></span>|
|<span data-ttu-id="c5986-171">postBuffer</span><span class="sxs-lookup"><span data-stu-id="c5986-171">postBuffer</span></span>|<span data-ttu-id="c5986-172">持续时间</span><span class="sxs-lookup"><span data-stu-id="c5986-172">Duration</span></span>|<span data-ttu-id="c5986-173">此服务的约会结束后以及下一个客户约会可以被预订前要缓冲的时间。</span><span class="sxs-lookup"><span data-stu-id="c5986-173">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="c5986-174">preBuffer</span><span class="sxs-lookup"><span data-stu-id="c5986-174">preBuffer</span></span>|<span data-ttu-id="c5986-175">持续时间</span><span class="sxs-lookup"><span data-stu-id="c5986-175">Duration</span></span>|<span data-ttu-id="c5986-176">在此服务的约会开始之前要缓冲的时间。</span><span class="sxs-lookup"><span data-stu-id="c5986-176">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="c5986-177">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="c5986-177">schedulingPolicy</span></span>|[<span data-ttu-id="c5986-178">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="c5986-178">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="c5986-179">确定应如何创建和管理此类服务的约会的一组策略。</span><span class="sxs-lookup"><span data-stu-id="c5986-179">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="c5986-180">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="c5986-180">staffMemberIds</span></span>|<span data-ttu-id="c5986-181">String collection</span><span class="sxs-lookup"><span data-stu-id="c5986-181">String collection</span></span>|<span data-ttu-id="c5986-182">代表提供此服务的[教职员工成员](../resources/bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="c5986-182">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="c5986-183">响应</span><span class="sxs-lookup"><span data-stu-id="c5986-183">Response</span></span>
<span data-ttu-id="c5986-p106">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c5986-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5986-186">示例</span><span class="sxs-lookup"><span data-stu-id="c5986-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5986-187">请求</span><span class="sxs-lookup"><span data-stu-id="c5986-187">Request</span></span>
<span data-ttu-id="c5986-188">下面的示例更新指定服务的持续时间。</span><span class="sxs-lookup"><span data-stu-id="c5986-188">The following example updates the duration of the specified service.</span></span>
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
##### <a name="response"></a><span data-ttu-id="c5986-189">响应</span><span class="sxs-lookup"><span data-stu-id="c5986-189">Response</span></span>
<span data-ttu-id="c5986-190">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c5986-190">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c5986-191">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c5986-191">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c5986-192">C#</span><span class="sxs-lookup"><span data-stu-id="c5986-192">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_bookingservice-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5986-193">Javascript</span><span class="sxs-lookup"><span data-stu-id="c5986-193">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_bookingservice-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c5986-194">目标-C</span><span class="sxs-lookup"><span data-stu-id="c5986-194">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_bookingservice-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingservice-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
