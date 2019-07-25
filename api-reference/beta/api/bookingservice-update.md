---
title: 更新 bookingservice
description: 更新指定 bookingbusiness 中的 bookingService 对象的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 49a775e542dba518d382b6999def6aa5795861a8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865263"
---
# <a name="update-bookingservice"></a><span data-ttu-id="4537b-103">更新 bookingservice</span><span class="sxs-lookup"><span data-stu-id="4537b-103">Update bookingservice</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4537b-104">更新指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingService](../resources/bookingservice.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4537b-104">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="4537b-105">下面是可以为服务自定义的一些示例:</span><span class="sxs-lookup"><span data-stu-id="4537b-105">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="4537b-106">价格</span><span class="sxs-lookup"><span data-stu-id="4537b-106">Price</span></span>
- <span data-ttu-id="4537b-107">约会的典型长度</span><span class="sxs-lookup"><span data-stu-id="4537b-107">Typical length of an appointment</span></span>
- <span data-ttu-id="4537b-108">提醒</span><span class="sxs-lookup"><span data-stu-id="4537b-108">Reminders</span></span>
- <span data-ttu-id="4537b-109">在服务完成之前或结束前设置的任何时间缓冲</span><span class="sxs-lookup"><span data-stu-id="4537b-109">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="4537b-110">将策略参数 (如 "最低通知")[安排](../resources/bookingschedulingpolicy.md)为 "书籍" 或 "取消", 以及客户是否可以选择约会的特定员工成员。</span><span class="sxs-lookup"><span data-stu-id="4537b-110">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="4537b-111">权限</span><span class="sxs-lookup"><span data-stu-id="4537b-111">Permissions</span></span>
<span data-ttu-id="4537b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4537b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4537b-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="4537b-114">Permission type</span></span>      | <span data-ttu-id="4537b-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4537b-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4537b-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4537b-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="4537b-117">全部预订. 全部, 全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="4537b-117">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4537b-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4537b-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4537b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="4537b-119">Not supported.</span></span>   |
|<span data-ttu-id="4537b-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="4537b-120">Application</span></span> | <span data-ttu-id="4537b-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="4537b-121">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4537b-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4537b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="4537b-123">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="4537b-123">Optional request headers</span></span>
| <span data-ttu-id="4537b-124">名称</span><span class="sxs-lookup"><span data-stu-id="4537b-124">Name</span></span>       | <span data-ttu-id="4537b-125">说明</span><span class="sxs-lookup"><span data-stu-id="4537b-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4537b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="4537b-126">Authorization</span></span>  | <span data-ttu-id="4537b-127">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="4537b-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4537b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4537b-128">Request body</span></span>
<span data-ttu-id="4537b-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4537b-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4537b-132">属性</span><span class="sxs-lookup"><span data-stu-id="4537b-132">Property</span></span>     | <span data-ttu-id="4537b-133">类型</span><span class="sxs-lookup"><span data-stu-id="4537b-133">Type</span></span>   |<span data-ttu-id="4537b-134">说明</span><span class="sxs-lookup"><span data-stu-id="4537b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4537b-135">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="4537b-135">defaultDuration</span></span>|<span data-ttu-id="4537b-136">持续时间</span><span class="sxs-lookup"><span data-stu-id="4537b-136">Duration</span></span>|<span data-ttu-id="4537b-137">服务的默认长度, 以天数、小时数、分钟数和秒数表示。</span><span class="sxs-lookup"><span data-stu-id="4537b-137">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="4537b-138">例如, P11D23H59M 59.999999999999 S。</span><span class="sxs-lookup"><span data-stu-id="4537b-138">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="4537b-139">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="4537b-139">defaultLocation</span></span>|[<span data-ttu-id="4537b-140">location</span><span class="sxs-lookup"><span data-stu-id="4537b-140">location</span></span>](../resources/location.md)|<span data-ttu-id="4537b-141">服务的默认物理位置。</span><span class="sxs-lookup"><span data-stu-id="4537b-141">The default physical location for the service.</span></span>|
|<span data-ttu-id="4537b-142">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="4537b-142">defaultPrice</span></span>|<span data-ttu-id="4537b-143">双精度</span><span class="sxs-lookup"><span data-stu-id="4537b-143">Double</span></span>|<span data-ttu-id="4537b-144">服务的默认货币价格。</span><span class="sxs-lookup"><span data-stu-id="4537b-144">The default monetary price for the service.</span></span>|
|<span data-ttu-id="4537b-145">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="4537b-145">defaultPriceType</span></span>|<span data-ttu-id="4537b-146">string</span><span class="sxs-lookup"><span data-stu-id="4537b-146">string</span></span>|<span data-ttu-id="4537b-147">服务收费的默认方式。</span><span class="sxs-lookup"><span data-stu-id="4537b-147">The default way the service is charged.</span></span> <span data-ttu-id="4537b-148">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="4537b-148">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="4537b-149">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="4537b-149">defaultReminders</span></span>|<span data-ttu-id="4537b-150">[bookingReminder](../resources/bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="4537b-150">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="4537b-151">此服务的约会的默认提醒集。</span><span class="sxs-lookup"><span data-stu-id="4537b-151">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="4537b-152">此属性的值仅在按 ID 读取此**bookingService**时可用。</span><span class="sxs-lookup"><span data-stu-id="4537b-152">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="4537b-153">说明</span><span class="sxs-lookup"><span data-stu-id="4537b-153">description</span></span>|<span data-ttu-id="4537b-154">String</span><span class="sxs-lookup"><span data-stu-id="4537b-154">String</span></span>|<span data-ttu-id="4537b-155">服务的文本说明。</span><span class="sxs-lookup"><span data-stu-id="4537b-155">A text description for the service.</span></span>|
|<span data-ttu-id="4537b-156">displayName</span><span class="sxs-lookup"><span data-stu-id="4537b-156">displayName</span></span>|<span data-ttu-id="4537b-157">字符串</span><span class="sxs-lookup"><span data-stu-id="4537b-157">String</span></span>|<span data-ttu-id="4537b-158">服务名称。</span><span class="sxs-lookup"><span data-stu-id="4537b-158">A service name.</span></span>|
|<span data-ttu-id="4537b-159">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4537b-159">emailAddress</span></span>|<span data-ttu-id="4537b-160">String</span><span class="sxs-lookup"><span data-stu-id="4537b-160">String</span></span>|<span data-ttu-id="4537b-161">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="4537b-161">An email address</span></span>|
|<span data-ttu-id="4537b-162">id</span><span class="sxs-lookup"><span data-stu-id="4537b-162">id</span></span>|<span data-ttu-id="4537b-163">String</span><span class="sxs-lookup"><span data-stu-id="4537b-163">String</span></span>| <span data-ttu-id="4537b-164">只读。</span><span class="sxs-lookup"><span data-stu-id="4537b-164">Read-only.</span></span>|
|<span data-ttu-id="4537b-165">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="4537b-165">isHiddenFromCustomers</span></span>|<span data-ttu-id="4537b-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="4537b-166">Boolean</span></span>|<span data-ttu-id="4537b-167">如果为 True, 则表示此服务不可供客户预订。</span><span class="sxs-lookup"><span data-stu-id="4537b-167">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="4537b-168">notes</span><span class="sxs-lookup"><span data-stu-id="4537b-168">notes</span></span>|<span data-ttu-id="4537b-169">String</span><span class="sxs-lookup"><span data-stu-id="4537b-169">String</span></span>|<span data-ttu-id="4537b-170">有关此服务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="4537b-170">Additional information about this service.</span></span>|
|<span data-ttu-id="4537b-171">postBuffer</span><span class="sxs-lookup"><span data-stu-id="4537b-171">postBuffer</span></span>|<span data-ttu-id="4537b-172">持续时间</span><span class="sxs-lookup"><span data-stu-id="4537b-172">Duration</span></span>|<span data-ttu-id="4537b-173">此服务的约会结束后以及下一个客户约会可以被预订前要缓冲的时间。</span><span class="sxs-lookup"><span data-stu-id="4537b-173">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="4537b-174">preBuffer</span><span class="sxs-lookup"><span data-stu-id="4537b-174">preBuffer</span></span>|<span data-ttu-id="4537b-175">持续时间</span><span class="sxs-lookup"><span data-stu-id="4537b-175">Duration</span></span>|<span data-ttu-id="4537b-176">在此服务的约会开始之前要缓冲的时间。</span><span class="sxs-lookup"><span data-stu-id="4537b-176">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="4537b-177">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="4537b-177">schedulingPolicy</span></span>|[<span data-ttu-id="4537b-178">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="4537b-178">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="4537b-179">确定应如何创建和管理此类服务的约会的一组策略。</span><span class="sxs-lookup"><span data-stu-id="4537b-179">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="4537b-180">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="4537b-180">staffMemberIds</span></span>|<span data-ttu-id="4537b-181">String collection</span><span class="sxs-lookup"><span data-stu-id="4537b-181">String collection</span></span>|<span data-ttu-id="4537b-182">代表提供此服务的[教职员工成员](../resources/bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="4537b-182">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="4537b-183">响应</span><span class="sxs-lookup"><span data-stu-id="4537b-183">Response</span></span>
<span data-ttu-id="4537b-p106">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4537b-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4537b-186">示例</span><span class="sxs-lookup"><span data-stu-id="4537b-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4537b-187">请求</span><span class="sxs-lookup"><span data-stu-id="4537b-187">Request</span></span>
<span data-ttu-id="4537b-188">下面的示例更新指定服务的持续时间。</span><span class="sxs-lookup"><span data-stu-id="4537b-188">The following example updates the duration of the specified service.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4537b-189">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="4537b-189">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="4537b-190">C#</span><span class="sxs-lookup"><span data-stu-id="4537b-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4537b-191">Javascript</span><span class="sxs-lookup"><span data-stu-id="4537b-191">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4537b-192">目标-C</span><span class="sxs-lookup"><span data-stu-id="4537b-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="4537b-193">Java</span><span class="sxs-lookup"><span data-stu-id="4537b-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-bookingservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4537b-194">响应</span><span class="sxs-lookup"><span data-stu-id="4537b-194">Response</span></span>
<span data-ttu-id="4537b-195">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4537b-195">The following is an example of the response.</span></span>
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
  ]
}
-->
