---
title: 更新 bookingservice
description: 更新指定 bookingbusiness 中的 bookingService 对象的属性。
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 9c64dc057963bdaed34ecab70792fdd5df526406
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43376354"
---
# <a name="update-bookingservice"></a><span data-ttu-id="0b882-103">更新 bookingservice</span><span class="sxs-lookup"><span data-stu-id="0b882-103">Update bookingservice</span></span>

<span data-ttu-id="0b882-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b882-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b882-105">更新指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingService](../resources/bookingservice.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0b882-105">Update the properties of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="0b882-106">下面是可以为服务自定义的一些示例：</span><span class="sxs-lookup"><span data-stu-id="0b882-106">The following are some examples you can customize for a service:</span></span>
- <span data-ttu-id="0b882-107">价格</span><span class="sxs-lookup"><span data-stu-id="0b882-107">Price</span></span>
- <span data-ttu-id="0b882-108">约会的典型长度</span><span class="sxs-lookup"><span data-stu-id="0b882-108">Typical length of an appointment</span></span>
- <span data-ttu-id="0b882-109">提醒</span><span class="sxs-lookup"><span data-stu-id="0b882-109">Reminders</span></span>
- <span data-ttu-id="0b882-110">在服务完成之前或结束前设置的任何时间缓冲</span><span class="sxs-lookup"><span data-stu-id="0b882-110">Any time buffer to set up before or finish up after the service</span></span>
- <span data-ttu-id="0b882-111">将策略参数（如 "最低通知"）[安排](../resources/bookingschedulingpolicy.md)为 "书籍" 或 "取消"，以及客户是否可以选择约会的特定员工成员。</span><span class="sxs-lookup"><span data-stu-id="0b882-111">[Scheduling policy](../resources/bookingschedulingpolicy.md) parameters such as minimum notice to book or cancel, and whether customers can select specific staff members for an appointment.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b882-112">权限</span><span class="sxs-lookup"><span data-stu-id="0b882-112">Permissions</span></span>
<span data-ttu-id="0b882-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b882-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b882-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b882-115">Permission type</span></span>      | <span data-ttu-id="0b882-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b882-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0b882-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b882-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="0b882-118">全部预订. 全部，全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="0b882-118">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0b882-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b882-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b882-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b882-120">Not supported.</span></span>   |
|<span data-ttu-id="0b882-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b882-121">Application</span></span> | <span data-ttu-id="0b882-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b882-122">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0b882-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b882-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="0b882-124">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="0b882-124">Optional request headers</span></span>
| <span data-ttu-id="0b882-125">名称</span><span class="sxs-lookup"><span data-stu-id="0b882-125">Name</span></span>       | <span data-ttu-id="0b882-126">说明</span><span class="sxs-lookup"><span data-stu-id="0b882-126">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="0b882-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b882-127">Authorization</span></span>  | <span data-ttu-id="0b882-128">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0b882-128">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b882-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b882-129">Request body</span></span>
<span data-ttu-id="0b882-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0b882-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0b882-133">属性</span><span class="sxs-lookup"><span data-stu-id="0b882-133">Property</span></span>     | <span data-ttu-id="0b882-134">类型</span><span class="sxs-lookup"><span data-stu-id="0b882-134">Type</span></span>   |<span data-ttu-id="0b882-135">说明</span><span class="sxs-lookup"><span data-stu-id="0b882-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b882-136">defaultDuration</span><span class="sxs-lookup"><span data-stu-id="0b882-136">defaultDuration</span></span>|<span data-ttu-id="0b882-137">持续时间</span><span class="sxs-lookup"><span data-stu-id="0b882-137">Duration</span></span>|<span data-ttu-id="0b882-138">服务的默认长度，以天数、小时数、分钟数和秒数表示。</span><span class="sxs-lookup"><span data-stu-id="0b882-138">The default length of the service, represented in numbers of days, hours, minutes, and seconds.</span></span> <span data-ttu-id="0b882-139">例如，P11D23H59M 59.999999999999 S。</span><span class="sxs-lookup"><span data-stu-id="0b882-139">For example, P11D23H59M59.999999999999S.</span></span> |
|<span data-ttu-id="0b882-140">defaultLocation</span><span class="sxs-lookup"><span data-stu-id="0b882-140">defaultLocation</span></span>|[<span data-ttu-id="0b882-141">位置</span><span class="sxs-lookup"><span data-stu-id="0b882-141">location</span></span>](../resources/location.md)|<span data-ttu-id="0b882-142">服务的默认物理位置。</span><span class="sxs-lookup"><span data-stu-id="0b882-142">The default physical location for the service.</span></span>|
|<span data-ttu-id="0b882-143">defaultPrice</span><span class="sxs-lookup"><span data-stu-id="0b882-143">defaultPrice</span></span>|<span data-ttu-id="0b882-144">双精度</span><span class="sxs-lookup"><span data-stu-id="0b882-144">Double</span></span>|<span data-ttu-id="0b882-145">服务的默认货币价格。</span><span class="sxs-lookup"><span data-stu-id="0b882-145">The default monetary price for the service.</span></span>|
|<span data-ttu-id="0b882-146">defaultPriceType</span><span class="sxs-lookup"><span data-stu-id="0b882-146">defaultPriceType</span></span>|<span data-ttu-id="0b882-147">string</span><span class="sxs-lookup"><span data-stu-id="0b882-147">string</span></span>|<span data-ttu-id="0b882-148">服务收费的默认方式。</span><span class="sxs-lookup"><span data-stu-id="0b882-148">The default way the service is charged.</span></span> <span data-ttu-id="0b882-149">可取值为：`undefined`、`fixedPrice`、`startingAt`、`hourly`、`free`、`priceVaries`、`callUs`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="0b882-149">Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.</span></span>|
|<span data-ttu-id="0b882-150">defaultReminders</span><span class="sxs-lookup"><span data-stu-id="0b882-150">defaultReminders</span></span>|<span data-ttu-id="0b882-151">[bookingReminder](../resources/bookingreminder.md)集合</span><span class="sxs-lookup"><span data-stu-id="0b882-151">[bookingReminder](../resources/bookingreminder.md) collection</span></span>|<span data-ttu-id="0b882-152">此服务的约会的默认提醒集。</span><span class="sxs-lookup"><span data-stu-id="0b882-152">The default set of reminders for an appointment of this service.</span></span> <span data-ttu-id="0b882-153">此属性的值仅在按 ID 读取此**bookingService**时可用。</span><span class="sxs-lookup"><span data-stu-id="0b882-153">The value of this property is available only when reading this **bookingService** by its ID.</span></span>|
|<span data-ttu-id="0b882-154">description</span><span class="sxs-lookup"><span data-stu-id="0b882-154">description</span></span>|<span data-ttu-id="0b882-155">String</span><span class="sxs-lookup"><span data-stu-id="0b882-155">String</span></span>|<span data-ttu-id="0b882-156">服务的文本说明。</span><span class="sxs-lookup"><span data-stu-id="0b882-156">A text description for the service.</span></span>|
|<span data-ttu-id="0b882-157">displayName</span><span class="sxs-lookup"><span data-stu-id="0b882-157">displayName</span></span>|<span data-ttu-id="0b882-158">字符串</span><span class="sxs-lookup"><span data-stu-id="0b882-158">String</span></span>|<span data-ttu-id="0b882-159">服务名称。</span><span class="sxs-lookup"><span data-stu-id="0b882-159">A service name.</span></span>|
|<span data-ttu-id="0b882-160">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0b882-160">emailAddress</span></span>|<span data-ttu-id="0b882-161">String</span><span class="sxs-lookup"><span data-stu-id="0b882-161">String</span></span>|<span data-ttu-id="0b882-162">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="0b882-162">An email address</span></span>|
|<span data-ttu-id="0b882-163">id</span><span class="sxs-lookup"><span data-stu-id="0b882-163">id</span></span>|<span data-ttu-id="0b882-164">字符串</span><span class="sxs-lookup"><span data-stu-id="0b882-164">String</span></span>| <span data-ttu-id="0b882-165">只读。</span><span class="sxs-lookup"><span data-stu-id="0b882-165">Read-only.</span></span>|
|<span data-ttu-id="0b882-166">isHiddenFromCustomers</span><span class="sxs-lookup"><span data-stu-id="0b882-166">isHiddenFromCustomers</span></span>|<span data-ttu-id="0b882-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b882-167">Boolean</span></span>|<span data-ttu-id="0b882-168">如果为 True，则表示此服务不可供客户预订。</span><span class="sxs-lookup"><span data-stu-id="0b882-168">True means this service is not available to customers for booking.</span></span>|
|<span data-ttu-id="0b882-169">notes</span><span class="sxs-lookup"><span data-stu-id="0b882-169">notes</span></span>|<span data-ttu-id="0b882-170">字符串</span><span class="sxs-lookup"><span data-stu-id="0b882-170">String</span></span>|<span data-ttu-id="0b882-171">有关此服务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="0b882-171">Additional information about this service.</span></span>|
|<span data-ttu-id="0b882-172">postBuffer</span><span class="sxs-lookup"><span data-stu-id="0b882-172">postBuffer</span></span>|<span data-ttu-id="0b882-173">持续时间</span><span class="sxs-lookup"><span data-stu-id="0b882-173">Duration</span></span>|<span data-ttu-id="0b882-174">此服务的约会结束后以及下一个客户约会可以被预订前要缓冲的时间。</span><span class="sxs-lookup"><span data-stu-id="0b882-174">The time to buffer after an appointment for this service ends, and before the next customer appointment can be booked.</span></span>|
|<span data-ttu-id="0b882-175">preBuffer</span><span class="sxs-lookup"><span data-stu-id="0b882-175">preBuffer</span></span>|<span data-ttu-id="0b882-176">持续时间</span><span class="sxs-lookup"><span data-stu-id="0b882-176">Duration</span></span>|<span data-ttu-id="0b882-177">在此服务的约会开始之前要缓冲的时间。</span><span class="sxs-lookup"><span data-stu-id="0b882-177">The time to buffer before an appointment for this service can start.</span></span>|
|<span data-ttu-id="0b882-178">schedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="0b882-178">schedulingPolicy</span></span>|[<span data-ttu-id="0b882-179">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="0b882-179">bookingSchedulingPolicy</span></span>](../resources/bookingschedulingpolicy.md)|<span data-ttu-id="0b882-180">确定应如何创建和管理此类服务的约会的一组策略。</span><span class="sxs-lookup"><span data-stu-id="0b882-180">The set of policies that determine how appointments for this type of service should be created and managed.</span></span>|
|<span data-ttu-id="0b882-181">staffMemberIds</span><span class="sxs-lookup"><span data-stu-id="0b882-181">staffMemberIds</span></span>|<span data-ttu-id="0b882-182">String 集合</span><span class="sxs-lookup"><span data-stu-id="0b882-182">String collection</span></span>|<span data-ttu-id="0b882-183">代表提供此服务的[教职员工成员](../resources/bookingstaffmember.md)。</span><span class="sxs-lookup"><span data-stu-id="0b882-183">Represents those [staff members](../resources/bookingstaffmember.md) who provide this service.</span></span> |

## <a name="response"></a><span data-ttu-id="0b882-184">响应</span><span class="sxs-lookup"><span data-stu-id="0b882-184">Response</span></span>
<span data-ttu-id="0b882-p106">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="0b882-p106">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0b882-187">示例</span><span class="sxs-lookup"><span data-stu-id="0b882-187">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0b882-188">请求</span><span class="sxs-lookup"><span data-stu-id="0b882-188">Request</span></span>
<span data-ttu-id="0b882-189">下面的示例更新指定服务的持续时间。</span><span class="sxs-lookup"><span data-stu-id="0b882-189">The following example updates the duration of the specified service.</span></span>

# <a name="http"></a>[<span data-ttu-id="0b882-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b882-190">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0b882-191">C#</span><span class="sxs-lookup"><span data-stu-id="0b882-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b882-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b882-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b882-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b882-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0b882-194">响应</span><span class="sxs-lookup"><span data-stu-id="0b882-194">Response</span></span>
<span data-ttu-id="0b882-195">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b882-195">The following is an example of the response.</span></span>
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
