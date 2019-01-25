---
title: 更新 bookingstaffmember
description: 更新在指定 bookingbusiness bookingStaffMember 的属性。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 608580a16d796a4ee1b296c0a19caea110326cff
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514556"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="fc014-103">更新 bookingstaffmember</span><span class="sxs-lookup"><span data-stu-id="fc014-103">Update bookingstaffmember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc014-104">更新在指定[bookingbusiness](../resources/bookingbusiness.md) [bookingStaffMember](../resources/bookingstaffmember.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="fc014-104">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="fc014-105">权限</span><span class="sxs-lookup"><span data-stu-id="fc014-105">Permissions</span></span>
<span data-ttu-id="fc014-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc014-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc014-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc014-108">Permission type</span></span>      | <span data-ttu-id="fc014-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc014-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc014-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc014-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="fc014-111">Bookings.ReadWrite.All Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="fc014-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="fc014-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc014-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc014-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc014-113">Not supported.</span></span>   |
|<span data-ttu-id="fc014-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc014-114">Application</span></span> | <span data-ttu-id="fc014-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc014-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fc014-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc014-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="fc014-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="fc014-117">Optional request headers</span></span>
| <span data-ttu-id="fc014-118">名称</span><span class="sxs-lookup"><span data-stu-id="fc014-118">Name</span></span>       | <span data-ttu-id="fc014-119">说明</span><span class="sxs-lookup"><span data-stu-id="fc014-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="fc014-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc014-120">Authorization</span></span>  | <span data-ttu-id="fc014-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="fc014-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc014-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc014-122">Request body</span></span>
<span data-ttu-id="fc014-p102">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="fc014-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fc014-126">属性</span><span class="sxs-lookup"><span data-stu-id="fc014-126">Property</span></span>     | <span data-ttu-id="fc014-127">类型</span><span class="sxs-lookup"><span data-stu-id="fc014-127">Type</span></span>   |<span data-ttu-id="fc014-128">说明</span><span class="sxs-lookup"><span data-stu-id="fc014-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc014-129">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="fc014-129">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="fc014-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc014-130">Boolean</span></span>|<span data-ttu-id="fc014-131">True 表示，如果该人员成员是 Office 365 用户，预订 API 使用 Office 365，以及**workingHours**属性的员工成员的个人日历来确定可用性。</span><span class="sxs-lookup"><span data-stu-id="fc014-131">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="fc014-132">ColorIndex</span><span class="sxs-lookup"><span data-stu-id="fc014-132">colorIndex</span></span>|<span data-ttu-id="fc014-133">Int32</span><span class="sxs-lookup"><span data-stu-id="fc014-133">Int32</span></span>|<span data-ttu-id="fc014-134">标识要表示员工成员的颜色。</span><span class="sxs-lookup"><span data-stu-id="fc014-134">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="fc014-135">颜色对应于预订应用程序中的**人员详细信息**页面中的调色板。</span><span class="sxs-lookup"><span data-stu-id="fc014-135">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="fc014-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fc014-136">displayName</span></span>|<span data-ttu-id="fc014-137">字符串</span><span class="sxs-lookup"><span data-stu-id="fc014-137">String</span></span>|<span data-ttu-id="fc014-138">员工成员，显示给客户的名称。</span><span class="sxs-lookup"><span data-stu-id="fc014-138">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="fc014-139">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fc014-139">emailAddress</span></span>|<span data-ttu-id="fc014-140">String</span><span class="sxs-lookup"><span data-stu-id="fc014-140">String</span></span>|<span data-ttu-id="fc014-141">员工成员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="fc014-141">The email address of the staff member.</span></span> <span data-ttu-id="fc014-142">这可以随着业务，相同的 Office 365 租户中或不同的电子邮件域中。</span><span class="sxs-lookup"><span data-stu-id="fc014-142">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="fc014-143">如果**sendConfirmationsToOwner**属性设置为使用此电子邮件地址的企业计划策略中，则返回 true。</span><span class="sxs-lookup"><span data-stu-id="fc014-143">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="fc014-144">role</span><span class="sxs-lookup"><span data-stu-id="fc014-144">role</span></span>|<span data-ttu-id="fc014-145">string</span><span class="sxs-lookup"><span data-stu-id="fc014-145">string</span></span>| <span data-ttu-id="fc014-146">企业中的人员成员角色。</span><span class="sxs-lookup"><span data-stu-id="fc014-146">The role of the staff member in the business.</span></span> <span data-ttu-id="fc014-147">可取值为：`guest`、`administrator`、`viewer`、`externalGuest`。</span><span class="sxs-lookup"><span data-stu-id="fc014-147">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="fc014-148">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="fc014-148">useBusinessHours</span></span>|<span data-ttu-id="fc014-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc014-149">Boolean</span></span>|<span data-ttu-id="fc014-150">True 表示由业务的**工作时间**属性来确定员工成员的可用性。</span><span class="sxs-lookup"><span data-stu-id="fc014-150">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="fc014-151">False，则意味着可用性由员工成员的**workingHouse**属性设置。</span><span class="sxs-lookup"><span data-stu-id="fc014-151">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="fc014-152">workingHours</span><span class="sxs-lookup"><span data-stu-id="fc014-152">workingHours</span></span>|<span data-ttu-id="fc014-153">[bookingWorkHours](../resources/bookingworkhours.md)集合</span><span class="sxs-lookup"><span data-stu-id="fc014-153">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="fc014-154">员工成员了可供预定的一周中每一天时间范围。</span><span class="sxs-lookup"><span data-stu-id="fc014-154">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="fc014-155">响应</span><span class="sxs-lookup"><span data-stu-id="fc014-155">Response</span></span>
<span data-ttu-id="fc014-p107">如果成功，此方法返回 `204 No content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="fc014-p107">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fc014-158">示例</span><span class="sxs-lookup"><span data-stu-id="fc014-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc014-159">请求</span><span class="sxs-lookup"><span data-stu-id="fc014-159">Request</span></span>
<span data-ttu-id="fc014-160">以下示例更改员工成员的计划已的工作。</span><span class="sxs-lookup"><span data-stu-id="fc014-160">The following example changes the staff member's schedule to have Mondays off.</span></span>
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
##### <a name="response"></a><span data-ttu-id="fc014-161">响应</span><span class="sxs-lookup"><span data-stu-id="fc014-161">Response</span></span>
<span data-ttu-id="fc014-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fc014-162">The following is an example of the response.</span></span>
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
    "Error: /api-reference/beta/api/bookingstaffmember-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
