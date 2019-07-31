---
title: bookingStaffMember 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 1de32728aff808975efd3121c9fd99fd0819b06c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013085"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="ca1bf-104">bookingStaffMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca1bf-104">bookingStaffMember resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="ca1bf-105">表示在[bookingBusiness](bookingbusiness.md)中提供服务的教职员工成员。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-105">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="ca1bf-106">教职员工成员可以是在其中配置预订业务的 Office 355 租户的一部分, 也可以使用来自其他电子邮件提供商的电子邮件服务。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-106">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="ca1bf-107">预订约会时, 预订 API 会考虑以下设置以确定教职员工成员的可用性:</span><span class="sxs-lookup"><span data-stu-id="ca1bf-107">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="ca1bf-108">默认情况下, 业务的运营时间 ( [bookingBusiness](bookingbusiness.md)实体的**businessHours**属性) 表示教职员工成员的正式可用性。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-108">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="ca1bf-109">如果**useBusinessHours**为 false, 则教职员工成员的特定工作时间 ( **BookingStaffmember**实体的**workingHours**属性) 表示该成员的常规可用性。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-109">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="ca1bf-110">如果**availabilityIsAffectedByPersonalCalendar**为 true, 则预订 API 将首先查看教职员工成员的可用小时数 (由 #1 或 #2 决定), 并在教职员工成员个人的这些时间内验证可用性。日历, 在进行预定前。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-110">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="ca1bf-111">方法</span><span class="sxs-lookup"><span data-stu-id="ca1bf-111">Methods</span></span>

| <span data-ttu-id="ca1bf-112">方法</span><span class="sxs-lookup"><span data-stu-id="ca1bf-112">Method</span></span>           | <span data-ttu-id="ca1bf-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="ca1bf-113">Return Type</span></span>    |<span data-ttu-id="ca1bf-114">说明</span><span class="sxs-lookup"><span data-stu-id="ca1bf-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ca1bf-115">列出教职员工成员</span><span class="sxs-lookup"><span data-stu-id="ca1bf-115">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="ca1bf-116">[bookingStaffMember](bookingstaffmember.md)集合</span><span class="sxs-lookup"><span data-stu-id="ca1bf-116">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="ca1bf-117">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingStaffMember**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-117">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="ca1bf-118">创建 bookingStaff</span><span class="sxs-lookup"><span data-stu-id="ca1bf-118">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="ca1bf-119">[bookingStaffMember](bookingstaffmember.md)集合</span><span class="sxs-lookup"><span data-stu-id="ca1bf-119">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="ca1bf-120">在指定的[bookingbusiness](../resources/bookingbusiness.md)中创建新的**bookingStaffMember** 。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-120">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="ca1bf-121">获取 bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="ca1bf-121">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="ca1bf-122">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="ca1bf-122">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="ca1bf-123">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingStaffMember**的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-123">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="ca1bf-124">更新</span><span class="sxs-lookup"><span data-stu-id="ca1bf-124">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="ca1bf-125">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="ca1bf-125">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="ca1bf-126">更新指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingStaffMember**的属性。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-126">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="ca1bf-127">删除</span><span class="sxs-lookup"><span data-stu-id="ca1bf-127">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="ca1bf-128">无</span><span class="sxs-lookup"><span data-stu-id="ca1bf-128">None</span></span> |<span data-ttu-id="ca1bf-129">删除指定[bookingbusiness](../resources/bookingbusiness.md)中的教职员工成员。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-129">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="ca1bf-130">属性</span><span class="sxs-lookup"><span data-stu-id="ca1bf-130">Properties</span></span>
| <span data-ttu-id="ca1bf-131">属性</span><span class="sxs-lookup"><span data-stu-id="ca1bf-131">Property</span></span>     | <span data-ttu-id="ca1bf-132">类型</span><span class="sxs-lookup"><span data-stu-id="ca1bf-132">Type</span></span>   |<span data-ttu-id="ca1bf-133">说明</span><span class="sxs-lookup"><span data-stu-id="ca1bf-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca1bf-134">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="ca1bf-134">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="ca1bf-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca1bf-135">Boolean</span></span>|<span data-ttu-id="ca1bf-136">如果为 True, 则表示如果教职员工成员是 Office 365 用户, 则在预定前, 预订 API 将验证教职员工成员在 Office 365 的个人日历中的可用性。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-136">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="ca1bf-137">colorIndex</span><span class="sxs-lookup"><span data-stu-id="ca1bf-137">colorIndex</span></span>|<span data-ttu-id="ca1bf-138">Int32</span><span class="sxs-lookup"><span data-stu-id="ca1bf-138">Int32</span></span>|<span data-ttu-id="ca1bf-139">标识代表教职员工成员的颜色。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-139">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="ca1bf-140">该颜色对应于预订应用中的 "**员工详细信息**" 页上的调色板。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-140">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="ca1bf-141">displayName</span><span class="sxs-lookup"><span data-stu-id="ca1bf-141">displayName</span></span>|<span data-ttu-id="ca1bf-142">字符串</span><span class="sxs-lookup"><span data-stu-id="ca1bf-142">String</span></span>|<span data-ttu-id="ca1bf-143">向客户显示的教职员工成员的姓名。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-143">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="ca1bf-144">必需。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-144">Required.</span></span>|
|<span data-ttu-id="ca1bf-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="ca1bf-145">emailAddress</span></span>|<span data-ttu-id="ca1bf-146">String</span><span class="sxs-lookup"><span data-stu-id="ca1bf-146">String</span></span>|<span data-ttu-id="ca1bf-147">教职员工成员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-147">The email address of the staff member.</span></span> <span data-ttu-id="ca1bf-148">这可以位于与企业相同的 Office 365 租户中, 也可以位于不同的电子邮件域中。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-148">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="ca1bf-149">如果在企业的计划策略中将**sendConfirmationsToOwner**属性设置为 true, 则可以使用此电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-149">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="ca1bf-150">必需。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-150">Required.</span></span>|
|<span data-ttu-id="ca1bf-151">id</span><span class="sxs-lookup"><span data-stu-id="ca1bf-151">id</span></span>|<span data-ttu-id="ca1bf-152">String</span><span class="sxs-lookup"><span data-stu-id="ca1bf-152">String</span></span>| <span data-ttu-id="ca1bf-153">以 GUID 格式的教职员工成员的 ID。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-153">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="ca1bf-154">只读。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-154">Read-only.</span></span>|
|<span data-ttu-id="ca1bf-155">role</span><span class="sxs-lookup"><span data-stu-id="ca1bf-155">role</span></span>|<span data-ttu-id="ca1bf-156">string</span><span class="sxs-lookup"><span data-stu-id="ca1bf-156">string</span></span>| <span data-ttu-id="ca1bf-157">企业中教职员工成员的角色。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-157">The role of the staff member in the business.</span></span> <span data-ttu-id="ca1bf-158">可取值为：`guest`、`administrator`、`viewer`、`externalGuest`。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-158">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="ca1bf-159">必需。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-159">Required.</span></span>|
|<span data-ttu-id="ca1bf-160">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="ca1bf-160">useBusinessHours</span></span>|<span data-ttu-id="ca1bf-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca1bf-161">Boolean</span></span>|<span data-ttu-id="ca1bf-162">如果为 True, 则表示教职员工成员的可用性是在企业的**businessHours**属性中指定的。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-162">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="ca1bf-163">False 表示可用性由教职员工成员的**workingHours**属性设置决定。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-163">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="ca1bf-164">workingHours</span><span class="sxs-lookup"><span data-stu-id="ca1bf-164">workingHours</span></span>|<span data-ttu-id="ca1bf-165">[bookingWorkHours](bookingworkhours.md)集合</span><span class="sxs-lookup"><span data-stu-id="ca1bf-165">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="ca1bf-166">教职员工成员可用于预订的一周中每一天的小时数。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-166">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="ca1bf-167">默认情况下, 它们被初始化为与企业的**businessHours**属性相同。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-167">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca1bf-168">关系</span><span class="sxs-lookup"><span data-stu-id="ca1bf-168">Relationships</span></span>
<span data-ttu-id="ca1bf-169">无</span><span class="sxs-lookup"><span data-stu-id="ca1bf-169">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ca1bf-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca1bf-170">JSON representation</span></span>

<span data-ttu-id="ca1bf-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca1bf-171">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
