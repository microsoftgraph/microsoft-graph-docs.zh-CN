---
title: bookingStaffMember 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: b7369ad3662bf86aaca14bc78ea52a1ebddcb4df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985947"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="69897-104">bookingStaffMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="69897-104">bookingStaffMember resource type</span></span>

 > <span data-ttu-id="69897-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="69897-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69897-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="69897-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="69897-107">代表一个人员成员提供[bookingBusiness](bookingbusiness.md)中的服务。</span><span class="sxs-lookup"><span data-stu-id="69897-107">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="69897-108">员工可以是其中配置预订业务，或者他们可使用其他电子邮件提供程序的电子邮件服务的 Office 355 租户的一部分。</span><span class="sxs-lookup"><span data-stu-id="69897-108">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="69897-109">当预订约会，预订 API 考虑以下设置来确定名员工的可用性：</span><span class="sxs-lookup"><span data-stu-id="69897-109">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="69897-110">默认情况下，业务 （ [bookingBusiness](bookingbusiness.md)实体的**工作时间**属性） 的营业时间表示员工成员的常规可用性。</span><span class="sxs-lookup"><span data-stu-id="69897-110">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="69897-111">如果**useBusinessHours**为 false，则员工成员的特定工作小时 （ **bookingStaffmember**实体**workingHours**属性） 表示该成员的常规可用性。</span><span class="sxs-lookup"><span data-stu-id="69897-111">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="69897-112">如果**availabilityIsAffectedByPersonalCalendar**为 true，然后预订 API 将首先查看员工成员的通常可用时间 （作为由 #1 或 #2），并验证可用性中员工成员的个人这些时间在进行预订之前的日历。</span><span class="sxs-lookup"><span data-stu-id="69897-112">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="69897-113">方法</span><span class="sxs-lookup"><span data-stu-id="69897-113">Methods</span></span>

| <span data-ttu-id="69897-114">方法</span><span class="sxs-lookup"><span data-stu-id="69897-114">Method</span></span>           | <span data-ttu-id="69897-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="69897-115">Return Type</span></span>    |<span data-ttu-id="69897-116">说明</span><span class="sxs-lookup"><span data-stu-id="69897-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69897-117">列表员工成员</span><span class="sxs-lookup"><span data-stu-id="69897-117">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="69897-118">[bookingStaffMember](bookingstaffmember.md)集合</span><span class="sxs-lookup"><span data-stu-id="69897-118">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="69897-119">指定[bookingbusiness](../resources/bookingbusiness.md)中获取**bookingStaffMember**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="69897-119">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="69897-120">创建 bookingStaff</span><span class="sxs-lookup"><span data-stu-id="69897-120">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="69897-121">[bookingStaffMember](bookingstaffmember.md)集合</span><span class="sxs-lookup"><span data-stu-id="69897-121">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="69897-122">在指定[bookingbusiness](../resources/bookingbusiness.md)中创建新**bookingStaffMember** 。</span><span class="sxs-lookup"><span data-stu-id="69897-122">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="69897-123">获取 bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="69897-123">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="69897-124">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="69897-124">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="69897-125">指定[bookingbusiness](../resources/bookingbusiness.md)中获取的属性和**bookingStaffMember**的关系。</span><span class="sxs-lookup"><span data-stu-id="69897-125">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="69897-126">更新</span><span class="sxs-lookup"><span data-stu-id="69897-126">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="69897-127">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="69897-127">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="69897-128">更新在指定[bookingbusiness](../resources/bookingbusiness.md) **bookingStaffMember**的属性。</span><span class="sxs-lookup"><span data-stu-id="69897-128">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="69897-129">删除</span><span class="sxs-lookup"><span data-stu-id="69897-129">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="69897-130">无</span><span class="sxs-lookup"><span data-stu-id="69897-130">None</span></span> |<span data-ttu-id="69897-131">删除指定[bookingbusiness](../resources/bookingbusiness.md)中的人员成员。</span><span class="sxs-lookup"><span data-stu-id="69897-131">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="69897-132">属性</span><span class="sxs-lookup"><span data-stu-id="69897-132">Properties</span></span>
| <span data-ttu-id="69897-133">属性</span><span class="sxs-lookup"><span data-stu-id="69897-133">Property</span></span>     | <span data-ttu-id="69897-134">类型</span><span class="sxs-lookup"><span data-stu-id="69897-134">Type</span></span>   |<span data-ttu-id="69897-135">说明</span><span class="sxs-lookup"><span data-stu-id="69897-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69897-136">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="69897-136">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="69897-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="69897-137">Boolean</span></span>|<span data-ttu-id="69897-138">True 表示，如果该人员成员是 Office 365 用户，预订 API 将验证员工成员的可用性其 Office 365 中的个人日历中之前进行预订。</span><span class="sxs-lookup"><span data-stu-id="69897-138">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="69897-139">colorIndex</span><span class="sxs-lookup"><span data-stu-id="69897-139">colorIndex</span></span>|<span data-ttu-id="69897-140">Int32</span><span class="sxs-lookup"><span data-stu-id="69897-140">Int32</span></span>|<span data-ttu-id="69897-141">标识要表示员工成员的颜色。</span><span class="sxs-lookup"><span data-stu-id="69897-141">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="69897-142">颜色对应于预订应用程序中的**人员详细信息**页面中的调色板。</span><span class="sxs-lookup"><span data-stu-id="69897-142">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="69897-143">displayName</span><span class="sxs-lookup"><span data-stu-id="69897-143">displayName</span></span>|<span data-ttu-id="69897-144">字符串</span><span class="sxs-lookup"><span data-stu-id="69897-144">String</span></span>|<span data-ttu-id="69897-145">员工成员，显示给客户的名称。</span><span class="sxs-lookup"><span data-stu-id="69897-145">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="69897-146">必需。</span><span class="sxs-lookup"><span data-stu-id="69897-146">Required.</span></span>|
|<span data-ttu-id="69897-147">emailAddress</span><span class="sxs-lookup"><span data-stu-id="69897-147">emailAddress</span></span>|<span data-ttu-id="69897-148">String</span><span class="sxs-lookup"><span data-stu-id="69897-148">String</span></span>|<span data-ttu-id="69897-149">员工成员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="69897-149">The email address of the staff member.</span></span> <span data-ttu-id="69897-150">这可以随着业务，相同的 Office 365 租户中或不同的电子邮件域中。</span><span class="sxs-lookup"><span data-stu-id="69897-150">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="69897-151">可使用此电子邮件地址，如果**sendConfirmationsToOwner**属性设置为 true 的企业计划策略。</span><span class="sxs-lookup"><span data-stu-id="69897-151">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="69897-152">必需。</span><span class="sxs-lookup"><span data-stu-id="69897-152">Required.</span></span>|
|<span data-ttu-id="69897-153">id</span><span class="sxs-lookup"><span data-stu-id="69897-153">id</span></span>|<span data-ttu-id="69897-154">字符串</span><span class="sxs-lookup"><span data-stu-id="69897-154">String</span></span>| <span data-ttu-id="69897-155">员工成员，GUID 格式的 ID。</span><span class="sxs-lookup"><span data-stu-id="69897-155">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="69897-156">只读。</span><span class="sxs-lookup"><span data-stu-id="69897-156">Read-only.</span></span>|
|<span data-ttu-id="69897-157">role</span><span class="sxs-lookup"><span data-stu-id="69897-157">role</span></span>|<span data-ttu-id="69897-158">string</span><span class="sxs-lookup"><span data-stu-id="69897-158">string</span></span>| <span data-ttu-id="69897-159">企业中的人员成员角色。</span><span class="sxs-lookup"><span data-stu-id="69897-159">The role of the staff member in the business.</span></span> <span data-ttu-id="69897-160">可取值为：`guest`、`administrator`、`viewer`、`externalGuest`。</span><span class="sxs-lookup"><span data-stu-id="69897-160">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="69897-161">必需。</span><span class="sxs-lookup"><span data-stu-id="69897-161">Required.</span></span>|
|<span data-ttu-id="69897-162">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="69897-162">useBusinessHours</span></span>|<span data-ttu-id="69897-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="69897-163">Boolean</span></span>|<span data-ttu-id="69897-164">True 的表示员工成员的可用性，作为业务**businessHours**属性中指定。</span><span class="sxs-lookup"><span data-stu-id="69897-164">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="69897-165">False，则意味着可用性由员工成员的**workingHours**属性设置。</span><span class="sxs-lookup"><span data-stu-id="69897-165">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="69897-166">workingHours</span><span class="sxs-lookup"><span data-stu-id="69897-166">workingHours</span></span>|<span data-ttu-id="69897-167">[bookingWorkHours](bookingworkhours.md)集合</span><span class="sxs-lookup"><span data-stu-id="69897-167">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="69897-168">员工成员了可供预定的一周中每一天时间范围。</span><span class="sxs-lookup"><span data-stu-id="69897-168">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="69897-169">默认情况下，它们都初始化为业务的**工作时间**属性相同。</span><span class="sxs-lookup"><span data-stu-id="69897-169">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69897-170">Relationships</span><span class="sxs-lookup"><span data-stu-id="69897-170">Relationships</span></span>
<span data-ttu-id="69897-171">无</span><span class="sxs-lookup"><span data-stu-id="69897-171">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="69897-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69897-172">JSON representation</span></span>

<span data-ttu-id="69897-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69897-173">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingStaffMember"
}-->

```json
{
  "availabilityIsAffectedByPersonalCalendar": true,
  "colorIndex": 1024,
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "role": "string",
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
