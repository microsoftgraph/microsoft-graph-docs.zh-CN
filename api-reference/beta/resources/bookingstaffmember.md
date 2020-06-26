---
title: bookingStaffMember 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: c8676ce2e43e88ce53e4c79e13b9151a0eca2b58
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895711"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="06d6b-104">bookingStaffMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="06d6b-104">bookingStaffMember resource type</span></span>

<span data-ttu-id="06d6b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06d6b-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="06d6b-106">表示在[bookingBusiness](bookingbusiness.md)中提供服务的教职员工成员。</span><span class="sxs-lookup"><span data-stu-id="06d6b-106">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="06d6b-107">教职员工成员可以是配置了预订业务的 Microsoft 365 租户的一部分，也可以使用来自其他电子邮件提供商的电子邮件服务。</span><span class="sxs-lookup"><span data-stu-id="06d6b-107">Staff members can be part of the Microsoft 365 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="06d6b-108">预订约会时，预订 API 会考虑以下设置以确定教职员工成员的可用性：</span><span class="sxs-lookup"><span data-stu-id="06d6b-108">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="06d6b-109">默认情况下，业务的运营时间（ [bookingBusiness](bookingbusiness.md)实体的**businessHours**属性）表示教职员工成员的正式可用性。</span><span class="sxs-lookup"><span data-stu-id="06d6b-109">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="06d6b-110">如果**useBusinessHours**为 false，则教职员工成员的特定工作时间（ **BookingStaffmember**实体的**workingHours**属性）表示该成员的常规可用性。</span><span class="sxs-lookup"><span data-stu-id="06d6b-110">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="06d6b-111">如果**availabilityIsAffectedByPersonalCalendar**为 true，则预订 API 将首先查看教职员工成员的一般可用小时数（由 #1 或 #2 决定），并在进行预定前在教职员工成员的个人日历中验证这些小时内的可用性。</span><span class="sxs-lookup"><span data-stu-id="06d6b-111">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="06d6b-112">方法</span><span class="sxs-lookup"><span data-stu-id="06d6b-112">Methods</span></span>

| <span data-ttu-id="06d6b-113">方法</span><span class="sxs-lookup"><span data-stu-id="06d6b-113">Method</span></span>           | <span data-ttu-id="06d6b-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="06d6b-114">Return Type</span></span>    |<span data-ttu-id="06d6b-115">说明</span><span class="sxs-lookup"><span data-stu-id="06d6b-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="06d6b-116">列出教职员工成员</span><span class="sxs-lookup"><span data-stu-id="06d6b-116">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="06d6b-117">[bookingStaffMember](bookingstaffmember.md)集合</span><span class="sxs-lookup"><span data-stu-id="06d6b-117">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="06d6b-118">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingStaffMember**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="06d6b-118">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="06d6b-119">创建 bookingStaff</span><span class="sxs-lookup"><span data-stu-id="06d6b-119">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="06d6b-120">[bookingStaffMember](bookingstaffmember.md)集合</span><span class="sxs-lookup"><span data-stu-id="06d6b-120">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="06d6b-121">在指定的[bookingbusiness](../resources/bookingbusiness.md)中创建新的**bookingStaffMember** 。</span><span class="sxs-lookup"><span data-stu-id="06d6b-121">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="06d6b-122">获取 bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="06d6b-122">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="06d6b-123">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="06d6b-123">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="06d6b-124">获取指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingStaffMember**的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06d6b-124">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="06d6b-125">更新</span><span class="sxs-lookup"><span data-stu-id="06d6b-125">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="06d6b-126">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="06d6b-126">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="06d6b-127">更新指定[bookingbusiness](../resources/bookingbusiness.md)中的**bookingStaffMember**的属性。</span><span class="sxs-lookup"><span data-stu-id="06d6b-127">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="06d6b-128">删除</span><span class="sxs-lookup"><span data-stu-id="06d6b-128">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="06d6b-129">无</span><span class="sxs-lookup"><span data-stu-id="06d6b-129">None</span></span> |<span data-ttu-id="06d6b-130">删除指定[bookingbusiness](../resources/bookingbusiness.md)中的教职员工成员。</span><span class="sxs-lookup"><span data-stu-id="06d6b-130">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="06d6b-131">属性</span><span class="sxs-lookup"><span data-stu-id="06d6b-131">Properties</span></span>
| <span data-ttu-id="06d6b-132">属性</span><span class="sxs-lookup"><span data-stu-id="06d6b-132">Property</span></span>     | <span data-ttu-id="06d6b-133">类型</span><span class="sxs-lookup"><span data-stu-id="06d6b-133">Type</span></span>   |<span data-ttu-id="06d6b-134">说明</span><span class="sxs-lookup"><span data-stu-id="06d6b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06d6b-135">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="06d6b-135">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="06d6b-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="06d6b-136">Boolean</span></span>|<span data-ttu-id="06d6b-137">如果为 True，则表示如果教职员工成员是 Microsoft 365 用户，则预订 API 将在进行预订前验证员工在 Microsoft 365 的个人日历中的可用性。</span><span class="sxs-lookup"><span data-stu-id="06d6b-137">True means that if the staff member is a Microsoft 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Microsoft 365, before making a booking.</span></span> |
|<span data-ttu-id="06d6b-138">colorIndex</span><span class="sxs-lookup"><span data-stu-id="06d6b-138">colorIndex</span></span>|<span data-ttu-id="06d6b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="06d6b-139">Int32</span></span>|<span data-ttu-id="06d6b-140">标识代表教职员工成员的颜色。</span><span class="sxs-lookup"><span data-stu-id="06d6b-140">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="06d6b-141">该颜色对应于预订应用中的 "**员工详细信息**" 页上的调色板。</span><span class="sxs-lookup"><span data-stu-id="06d6b-141">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="06d6b-142">displayName</span><span class="sxs-lookup"><span data-stu-id="06d6b-142">displayName</span></span>|<span data-ttu-id="06d6b-143">字符串</span><span class="sxs-lookup"><span data-stu-id="06d6b-143">String</span></span>|<span data-ttu-id="06d6b-144">向客户显示的教职员工成员的姓名。</span><span class="sxs-lookup"><span data-stu-id="06d6b-144">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="06d6b-145">必填。</span><span class="sxs-lookup"><span data-stu-id="06d6b-145">Required.</span></span>|
|<span data-ttu-id="06d6b-146">emailAddress</span><span class="sxs-lookup"><span data-stu-id="06d6b-146">emailAddress</span></span>|<span data-ttu-id="06d6b-147">String</span><span class="sxs-lookup"><span data-stu-id="06d6b-147">String</span></span>|<span data-ttu-id="06d6b-148">教职员工成员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="06d6b-148">The email address of the staff member.</span></span> <span data-ttu-id="06d6b-149">这可以与公司在同一 Microsoft 365 租户中，也可以位于不同的电子邮件域中。</span><span class="sxs-lookup"><span data-stu-id="06d6b-149">This can be in the same Microsoft 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="06d6b-150">如果在企业的计划策略中将**sendConfirmationsToOwner**属性设置为 true，则可以使用此电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="06d6b-150">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="06d6b-151">必需。</span><span class="sxs-lookup"><span data-stu-id="06d6b-151">Required.</span></span>|
|<span data-ttu-id="06d6b-152">id</span><span class="sxs-lookup"><span data-stu-id="06d6b-152">id</span></span>|<span data-ttu-id="06d6b-153">String</span><span class="sxs-lookup"><span data-stu-id="06d6b-153">String</span></span>| <span data-ttu-id="06d6b-154">以 GUID 格式的教职员工成员的 ID。</span><span class="sxs-lookup"><span data-stu-id="06d6b-154">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="06d6b-155">只读。</span><span class="sxs-lookup"><span data-stu-id="06d6b-155">Read-only.</span></span>|
|<span data-ttu-id="06d6b-156">role</span><span class="sxs-lookup"><span data-stu-id="06d6b-156">role</span></span>|<span data-ttu-id="06d6b-157">string</span><span class="sxs-lookup"><span data-stu-id="06d6b-157">string</span></span>| <span data-ttu-id="06d6b-158">企业中教职员工成员的角色。</span><span class="sxs-lookup"><span data-stu-id="06d6b-158">The role of the staff member in the business.</span></span> <span data-ttu-id="06d6b-159">可取值为：`guest`、`administrator`、`viewer`、`externalGuest`。</span><span class="sxs-lookup"><span data-stu-id="06d6b-159">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="06d6b-160">必填。</span><span class="sxs-lookup"><span data-stu-id="06d6b-160">Required.</span></span>|
|<span data-ttu-id="06d6b-161">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="06d6b-161">useBusinessHours</span></span>|<span data-ttu-id="06d6b-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="06d6b-162">Boolean</span></span>|<span data-ttu-id="06d6b-163">如果为 True，则表示教职员工成员的可用性是在企业的**businessHours**属性中指定的。</span><span class="sxs-lookup"><span data-stu-id="06d6b-163">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="06d6b-164">False 表示可用性由教职员工成员的**workingHours**属性设置决定。</span><span class="sxs-lookup"><span data-stu-id="06d6b-164">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="06d6b-165">workingHours</span><span class="sxs-lookup"><span data-stu-id="06d6b-165">workingHours</span></span>|<span data-ttu-id="06d6b-166">[bookingWorkHours](bookingworkhours.md)集合</span><span class="sxs-lookup"><span data-stu-id="06d6b-166">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="06d6b-167">教职员工成员可用于预订的一周中每一天的小时数。</span><span class="sxs-lookup"><span data-stu-id="06d6b-167">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="06d6b-168">默认情况下，它们被初始化为与企业的**businessHours**属性相同。</span><span class="sxs-lookup"><span data-stu-id="06d6b-168">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06d6b-169">关系</span><span class="sxs-lookup"><span data-stu-id="06d6b-169">Relationships</span></span>
<span data-ttu-id="06d6b-170">无</span><span class="sxs-lookup"><span data-stu-id="06d6b-170">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="06d6b-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06d6b-171">JSON representation</span></span>

<span data-ttu-id="06d6b-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06d6b-172">The following is a JSON representation of the resource.</span></span>

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
