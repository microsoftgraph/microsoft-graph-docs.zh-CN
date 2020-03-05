---
title: 更新 bookingstaffmember
description: 更新指定 bookingbusiness 中的 bookingStaffMember 的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: e710d98ffd287e2c763608d899f74ddf2e6ce82c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441065"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="5e1cf-103">更新 bookingstaffmember</span><span class="sxs-lookup"><span data-stu-id="5e1cf-103">Update bookingstaffmember</span></span>

<span data-ttu-id="5e1cf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5e1cf-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e1cf-105">更新指定[bookingbusiness](../resources/bookingbusiness.md)中的[bookingStaffMember](../resources/bookingstaffmember.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-105">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5e1cf-106">权限</span><span class="sxs-lookup"><span data-stu-id="5e1cf-106">Permissions</span></span>
<span data-ttu-id="5e1cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e1cf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e1cf-109">Permission type</span></span>      | <span data-ttu-id="5e1cf-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e1cf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e1cf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e1cf-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="5e1cf-112">全部预订. 全部，全部预订. 全部</span><span class="sxs-lookup"><span data-stu-id="5e1cf-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5e1cf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e1cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e1cf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-114">Not supported.</span></span>   |
|<span data-ttu-id="5e1cf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e1cf-115">Application</span></span> | <span data-ttu-id="5e1cf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5e1cf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e1cf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="5e1cf-118">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="5e1cf-118">Optional request headers</span></span>
| <span data-ttu-id="5e1cf-119">名称</span><span class="sxs-lookup"><span data-stu-id="5e1cf-119">Name</span></span>       | <span data-ttu-id="5e1cf-120">说明</span><span class="sxs-lookup"><span data-stu-id="5e1cf-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5e1cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e1cf-121">Authorization</span></span>  | <span data-ttu-id="5e1cf-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5e1cf-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e1cf-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e1cf-123">Request body</span></span>
<span data-ttu-id="5e1cf-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5e1cf-127">属性</span><span class="sxs-lookup"><span data-stu-id="5e1cf-127">Property</span></span>     | <span data-ttu-id="5e1cf-128">类型</span><span class="sxs-lookup"><span data-stu-id="5e1cf-128">Type</span></span>   |<span data-ttu-id="5e1cf-129">说明</span><span class="sxs-lookup"><span data-stu-id="5e1cf-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e1cf-130">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="5e1cf-130">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="5e1cf-131">布尔</span><span class="sxs-lookup"><span data-stu-id="5e1cf-131">Boolean</span></span>|<span data-ttu-id="5e1cf-132">如果为 True，则表示如果教职员工成员是 Office 365 用户，则预订 API 将使用 Office 365 中的教职员工成员的个人日历以及**workingHours**属性来确定可用性。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-132">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="5e1cf-133">colorIndex</span><span class="sxs-lookup"><span data-stu-id="5e1cf-133">colorIndex</span></span>|<span data-ttu-id="5e1cf-134">Int32</span><span class="sxs-lookup"><span data-stu-id="5e1cf-134">Int32</span></span>|<span data-ttu-id="5e1cf-135">标识代表教职员工成员的颜色。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-135">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="5e1cf-136">该颜色对应于预订应用中的 "**员工详细信息**" 页上的调色板。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-136">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="5e1cf-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5e1cf-137">displayName</span></span>|<span data-ttu-id="5e1cf-138">String</span><span class="sxs-lookup"><span data-stu-id="5e1cf-138">String</span></span>|<span data-ttu-id="5e1cf-139">向客户显示的教职员工成员的姓名。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-139">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="5e1cf-140">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5e1cf-140">emailAddress</span></span>|<span data-ttu-id="5e1cf-141">String</span><span class="sxs-lookup"><span data-stu-id="5e1cf-141">String</span></span>|<span data-ttu-id="5e1cf-142">教职员工成员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-142">The email address of the staff member.</span></span> <span data-ttu-id="5e1cf-143">这可以位于与企业相同的 Office 365 租户中，也可以位于不同的电子邮件域中。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-143">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="5e1cf-144">如果在企业的计划策略中将**sendConfirmationsToOwner**属性设置为 true，则使用此电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-144">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="5e1cf-145">role</span><span class="sxs-lookup"><span data-stu-id="5e1cf-145">role</span></span>|<span data-ttu-id="5e1cf-146">string</span><span class="sxs-lookup"><span data-stu-id="5e1cf-146">string</span></span>| <span data-ttu-id="5e1cf-147">企业中教职员工成员的角色。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-147">The role of the staff member in the business.</span></span> <span data-ttu-id="5e1cf-148">可取值为：`guest`、`administrator`、`viewer`、`externalGuest`。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-148">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="5e1cf-149">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="5e1cf-149">useBusinessHours</span></span>|<span data-ttu-id="5e1cf-150">布尔</span><span class="sxs-lookup"><span data-stu-id="5e1cf-150">Boolean</span></span>|<span data-ttu-id="5e1cf-151">如果为 True，则表示教职员工成员的可用性取决于企业的**businessHours**属性。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-151">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="5e1cf-152">False 表示可用性由教职员工成员的**workingHouse**属性设置决定。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-152">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="5e1cf-153">workingHours</span><span class="sxs-lookup"><span data-stu-id="5e1cf-153">workingHours</span></span>|<span data-ttu-id="5e1cf-154">[bookingWorkHours](../resources/bookingworkhours.md)集合</span><span class="sxs-lookup"><span data-stu-id="5e1cf-154">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="5e1cf-155">教职员工成员可用于预订的一周中每一天的小时数。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-155">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="5e1cf-156">响应</span><span class="sxs-lookup"><span data-stu-id="5e1cf-156">Response</span></span>
<span data-ttu-id="5e1cf-p107">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-p107">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5e1cf-159">示例</span><span class="sxs-lookup"><span data-stu-id="5e1cf-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e1cf-160">请求</span><span class="sxs-lookup"><span data-stu-id="5e1cf-160">Request</span></span>
<span data-ttu-id="5e1cf-161">以下示例将教职员工成员的日程安排更改为 "星期一关"。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-161">The following example changes the staff member's schedule to have Mondays off.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e1cf-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e1cf-162">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_bookingstaffmember"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148
Content-type: application/json

{
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[

            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"tuesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"wednesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"thursday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"friday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="5e1cf-163">C#</span><span class="sxs-lookup"><span data-stu-id="5e1cf-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e1cf-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e1cf-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e1cf-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e1cf-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5e1cf-166">响应</span><span class="sxs-lookup"><span data-stu-id="5e1cf-166">Response</span></span>
<span data-ttu-id="5e1cf-167">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5e1cf-167">The following is an example of the response.</span></span>
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
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
