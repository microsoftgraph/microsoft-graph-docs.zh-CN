---
title: 更新 bookingstaffmember
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
ms.openlocfilehash: 99501f31ccd2b810d6a0c7f836d5b70bb98f223b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042455"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="5800f-104">更新 bookingstaffmember</span><span class="sxs-lookup"><span data-stu-id="5800f-104">Update bookingstaffmember</span></span>

 > <span data-ttu-id="5800f-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5800f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5800f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5800f-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="5800f-107">更新在指定[bookingbusiness](../resources/bookingbusiness.md) [bookingStaffMember](../resources/bookingstaffmember.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="5800f-107">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5800f-108">权限</span><span class="sxs-lookup"><span data-stu-id="5800f-108">Permissions</span></span>
<span data-ttu-id="5800f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5800f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5800f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5800f-111">Permission type</span></span>      | <span data-ttu-id="5800f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5800f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5800f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5800f-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="5800f-114">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="5800f-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5800f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5800f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5800f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5800f-116">Not supported.</span></span>   |
|<span data-ttu-id="5800f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5800f-117">Application</span></span> | <span data-ttu-id="5800f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5800f-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="5800f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5800f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="5800f-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="5800f-120">Optional request headers</span></span>
| <span data-ttu-id="5800f-121">名称</span><span class="sxs-lookup"><span data-stu-id="5800f-121">Name</span></span>       | <span data-ttu-id="5800f-122">说明</span><span class="sxs-lookup"><span data-stu-id="5800f-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5800f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5800f-123">Authorization</span></span>  | <span data-ttu-id="5800f-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="5800f-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5800f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5800f-125">Request body</span></span>
<span data-ttu-id="5800f-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5800f-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5800f-129">属性</span><span class="sxs-lookup"><span data-stu-id="5800f-129">Property</span></span>     | <span data-ttu-id="5800f-130">类型</span><span class="sxs-lookup"><span data-stu-id="5800f-130">Type</span></span>   |<span data-ttu-id="5800f-131">说明</span><span class="sxs-lookup"><span data-stu-id="5800f-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5800f-132">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="5800f-132">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="5800f-133">布尔</span><span class="sxs-lookup"><span data-stu-id="5800f-133">Boolean</span></span>|<span data-ttu-id="5800f-134">True 表示，如果该人员成员是 Office 365 用户，预订 API 使用 Office 365，以及**workingHours**属性的员工成员的个人日历来确定可用性。</span><span class="sxs-lookup"><span data-stu-id="5800f-134">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="5800f-135">colorIndex</span><span class="sxs-lookup"><span data-stu-id="5800f-135">colorIndex</span></span>|<span data-ttu-id="5800f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="5800f-136">Int32</span></span>|<span data-ttu-id="5800f-137">标识要表示员工成员的颜色。</span><span class="sxs-lookup"><span data-stu-id="5800f-137">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="5800f-138">颜色对应于预订应用程序中的**人员详细信息**页面中的调色板。</span><span class="sxs-lookup"><span data-stu-id="5800f-138">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="5800f-139">displayName</span><span class="sxs-lookup"><span data-stu-id="5800f-139">displayName</span></span>|<span data-ttu-id="5800f-140">字符串</span><span class="sxs-lookup"><span data-stu-id="5800f-140">String</span></span>|<span data-ttu-id="5800f-141">员工成员，显示给客户的名称。</span><span class="sxs-lookup"><span data-stu-id="5800f-141">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="5800f-142">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5800f-142">emailAddress</span></span>|<span data-ttu-id="5800f-143">String</span><span class="sxs-lookup"><span data-stu-id="5800f-143">String</span></span>|<span data-ttu-id="5800f-144">员工成员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5800f-144">The email address of the staff member.</span></span> <span data-ttu-id="5800f-145">这可以随着业务，相同的 Office 365 租户中或不同的电子邮件域中。</span><span class="sxs-lookup"><span data-stu-id="5800f-145">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="5800f-146">如果**sendConfirmationsToOwner**属性设置为使用此电子邮件地址的企业计划策略中，则返回 true。</span><span class="sxs-lookup"><span data-stu-id="5800f-146">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="5800f-147">role</span><span class="sxs-lookup"><span data-stu-id="5800f-147">role</span></span>|<span data-ttu-id="5800f-148">string</span><span class="sxs-lookup"><span data-stu-id="5800f-148">string</span></span>| <span data-ttu-id="5800f-149">企业中的人员成员角色。</span><span class="sxs-lookup"><span data-stu-id="5800f-149">The role of the staff member in the business.</span></span> <span data-ttu-id="5800f-150">可取值为：`guest`、`administrator`、`viewer`、`externalGuest`。</span><span class="sxs-lookup"><span data-stu-id="5800f-150">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="5800f-151">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="5800f-151">useBusinessHours</span></span>|<span data-ttu-id="5800f-152">布尔</span><span class="sxs-lookup"><span data-stu-id="5800f-152">Boolean</span></span>|<span data-ttu-id="5800f-153">True 表示由业务的**工作时间**属性来确定员工成员的可用性。</span><span class="sxs-lookup"><span data-stu-id="5800f-153">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="5800f-154">False，则意味着可用性由员工成员的**workingHouse**属性设置。</span><span class="sxs-lookup"><span data-stu-id="5800f-154">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="5800f-155">workingHours</span><span class="sxs-lookup"><span data-stu-id="5800f-155">workingHours</span></span>|<span data-ttu-id="5800f-156">[bookingWorkHours](../resources/bookingworkhours.md)集合</span><span class="sxs-lookup"><span data-stu-id="5800f-156">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="5800f-157">员工成员了可供预定的一周中每一天时间范围。</span><span class="sxs-lookup"><span data-stu-id="5800f-157">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="5800f-158">响应</span><span class="sxs-lookup"><span data-stu-id="5800f-158">Response</span></span>
<span data-ttu-id="5800f-p109">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5800f-p109">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5800f-161">示例</span><span class="sxs-lookup"><span data-stu-id="5800f-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5800f-162">请求</span><span class="sxs-lookup"><span data-stu-id="5800f-162">Request</span></span>
<span data-ttu-id="5800f-163">以下示例更改员工成员的计划已的工作。</span><span class="sxs-lookup"><span data-stu-id="5800f-163">The following example changes the staff member's schedule to have Mondays off.</span></span>
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
##### <a name="response"></a><span data-ttu-id="5800f-164">响应</span><span class="sxs-lookup"><span data-stu-id="5800f-164">Response</span></span>
<span data-ttu-id="5800f-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5800f-165">The following is an example of the response.</span></span> 
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
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->