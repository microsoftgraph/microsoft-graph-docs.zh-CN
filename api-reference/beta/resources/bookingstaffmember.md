---
title: bookingStaffMember 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 72130f46dc67d4491f9855706528ee5894b8352f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520275"
---
# <a name="bookingstaffmember-resource-type"></a><span data-ttu-id="84392-104">bookingStaffMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="84392-104">bookingStaffMember resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="84392-105">代表一个人员成员提供[bookingBusiness](bookingbusiness.md)中的服务。</span><span class="sxs-lookup"><span data-stu-id="84392-105">Represents a staff member who provides services in a [bookingBusiness](bookingbusiness.md).</span></span>

<span data-ttu-id="84392-106">员工可以是其中配置预订业务，或者他们可使用其他电子邮件提供程序的电子邮件服务的 Office 355 租户的一部分。</span><span class="sxs-lookup"><span data-stu-id="84392-106">Staff members can be part of the Office 355 tenant where the booking business is configured, or they can use email services from other email providers.</span></span>

<span data-ttu-id="84392-107">当预订约会，预订 API 考虑以下设置来确定名员工的可用性：</span><span class="sxs-lookup"><span data-stu-id="84392-107">When booking appointments, the Bookings API considers the following settings to determine a staff member's availability:</span></span> 

1. <span data-ttu-id="84392-108">默认情况下，业务 （ [bookingBusiness](bookingbusiness.md)实体的**工作时间**属性） 的营业时间表示员工成员的常规可用性。</span><span class="sxs-lookup"><span data-stu-id="84392-108">By default, the hours of operation of the business (the **businessHours** property of the [bookingBusiness](bookingbusiness.md) entity) represents the general availability of the staff member.</span></span>
2. <span data-ttu-id="84392-109">如果**useBusinessHours**为 false，则员工成员的特定工作小时 （ **bookingStaffmember**实体**workingHours**属性） 表示该成员的常规可用性。</span><span class="sxs-lookup"><span data-stu-id="84392-109">If **useBusinessHours** is false, then the staff member's specific work hours (**workingHours** property of the **bookingStaffmember** entity) represents that member's general availability.</span></span>
3. <span data-ttu-id="84392-110">如果**availabilityIsAffectedByPersonalCalendar**为 true，然后预订 API 将首先查看员工成员的通常可用时间 （作为由 #1 或 #2），并验证可用性中员工成员的个人这些时间在进行预订之前的日历。</span><span class="sxs-lookup"><span data-stu-id="84392-110">If **availabilityIsAffectedByPersonalCalendar** is true, then the Bookings API would first look at the staff member's generally available hours (as determined by either #1 or #2), and verify availability during those hours in the staff member's personal calendar, before making a booking.</span></span>

## <a name="methods"></a><span data-ttu-id="84392-111">方法</span><span class="sxs-lookup"><span data-stu-id="84392-111">Methods</span></span>

| <span data-ttu-id="84392-112">方法</span><span class="sxs-lookup"><span data-stu-id="84392-112">Method</span></span>           | <span data-ttu-id="84392-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="84392-113">Return Type</span></span>    |<span data-ttu-id="84392-114">说明</span><span class="sxs-lookup"><span data-stu-id="84392-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="84392-115">列表员工成员</span><span class="sxs-lookup"><span data-stu-id="84392-115">List staff members</span></span>](../api/bookingbusiness-list-staffmembers.md) | <span data-ttu-id="84392-116">[bookingStaffMember](bookingstaffmember.md)集合</span><span class="sxs-lookup"><span data-stu-id="84392-116">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="84392-117">指定[bookingbusiness](../resources/bookingbusiness.md)中获取**bookingStaffMember**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="84392-117">Get a list of **bookingStaffMember** objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="84392-118">创建 bookingStaff</span><span class="sxs-lookup"><span data-stu-id="84392-118">Create bookingStaff</span></span>](../api/bookingbusiness-post-staffmembers.md) | <span data-ttu-id="84392-119">[bookingStaffMember](bookingstaffmember.md)集合</span><span class="sxs-lookup"><span data-stu-id="84392-119">[bookingStaffMember](bookingstaffmember.md) collection</span></span> | <span data-ttu-id="84392-120">在指定[bookingbusiness](../resources/bookingbusiness.md)中创建新**bookingStaffMember** 。</span><span class="sxs-lookup"><span data-stu-id="84392-120">Create a new **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |
|[<span data-ttu-id="84392-121">获取 bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="84392-121">Get bookingStaffMember</span></span>](../api/bookingstaffmember-get.md) | [<span data-ttu-id="84392-122">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="84392-122">bookingStaffMember</span></span>](bookingstaffmember.md) |<span data-ttu-id="84392-123">指定[bookingbusiness](../resources/bookingbusiness.md)中获取的属性和**bookingStaffMember**的关系。</span><span class="sxs-lookup"><span data-stu-id="84392-123">Get the properties and relationships of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="84392-124">Update</span><span class="sxs-lookup"><span data-stu-id="84392-124">Update</span></span>](../api/bookingstaffmember-update.md) | [<span data-ttu-id="84392-125">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="84392-125">bookingStaffMember</span></span>](bookingstaffmember.md)    |<span data-ttu-id="84392-126">更新在指定[bookingbusiness](../resources/bookingbusiness.md) **bookingStaffMember**的属性。</span><span class="sxs-lookup"><span data-stu-id="84392-126">Update the properties of a **bookingStaffMember** in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>|
|[<span data-ttu-id="84392-127">删除</span><span class="sxs-lookup"><span data-stu-id="84392-127">Delete</span></span>](../api/bookingstaffmember-delete.md) | <span data-ttu-id="84392-128">无</span><span class="sxs-lookup"><span data-stu-id="84392-128">None</span></span> |<span data-ttu-id="84392-129">删除指定[bookingbusiness](../resources/bookingbusiness.md)中的人员成员。</span><span class="sxs-lookup"><span data-stu-id="84392-129">Delete a staff member in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="84392-130">属性</span><span class="sxs-lookup"><span data-stu-id="84392-130">Properties</span></span>
| <span data-ttu-id="84392-131">属性</span><span class="sxs-lookup"><span data-stu-id="84392-131">Property</span></span>     | <span data-ttu-id="84392-132">类型</span><span class="sxs-lookup"><span data-stu-id="84392-132">Type</span></span>   |<span data-ttu-id="84392-133">说明</span><span class="sxs-lookup"><span data-stu-id="84392-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="84392-134">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="84392-134">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="84392-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="84392-135">Boolean</span></span>|<span data-ttu-id="84392-136">True 表示，如果该人员成员是 Office 365 用户，预订 API 将验证员工成员的可用性其 Office 365 中的个人日历中之前进行预订。</span><span class="sxs-lookup"><span data-stu-id="84392-136">True means that if the staff member is an Office 365 user, the Bookings API would verify the staff member's availability in their personal calendar in Office 365, before making a booking.</span></span> |
|<span data-ttu-id="84392-137">ColorIndex</span><span class="sxs-lookup"><span data-stu-id="84392-137">colorIndex</span></span>|<span data-ttu-id="84392-138">Int32</span><span class="sxs-lookup"><span data-stu-id="84392-138">Int32</span></span>|<span data-ttu-id="84392-139">标识要表示员工成员的颜色。</span><span class="sxs-lookup"><span data-stu-id="84392-139">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="84392-140">颜色对应于预订应用程序中的**人员详细信息**页面中的调色板。</span><span class="sxs-lookup"><span data-stu-id="84392-140">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="84392-141">displayName</span><span class="sxs-lookup"><span data-stu-id="84392-141">displayName</span></span>|<span data-ttu-id="84392-142">String</span><span class="sxs-lookup"><span data-stu-id="84392-142">String</span></span>|<span data-ttu-id="84392-143">员工成员，显示给客户的名称。</span><span class="sxs-lookup"><span data-stu-id="84392-143">The name of the staff member, as displayed to customers.</span></span> <span data-ttu-id="84392-144">必需。</span><span class="sxs-lookup"><span data-stu-id="84392-144">Required.</span></span>|
|<span data-ttu-id="84392-145">emailAddress</span><span class="sxs-lookup"><span data-stu-id="84392-145">emailAddress</span></span>|<span data-ttu-id="84392-146">String</span><span class="sxs-lookup"><span data-stu-id="84392-146">String</span></span>|<span data-ttu-id="84392-147">员工成员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="84392-147">The email address of the staff member.</span></span> <span data-ttu-id="84392-148">这可以随着业务，相同的 Office 365 租户中或不同的电子邮件域中。</span><span class="sxs-lookup"><span data-stu-id="84392-148">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="84392-149">可使用此电子邮件地址，如果**sendConfirmationsToOwner**属性设置为 true 的企业计划策略。</span><span class="sxs-lookup"><span data-stu-id="84392-149">This email address can be used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span> <span data-ttu-id="84392-150">必需。</span><span class="sxs-lookup"><span data-stu-id="84392-150">Required.</span></span>|
|<span data-ttu-id="84392-151">id</span><span class="sxs-lookup"><span data-stu-id="84392-151">id</span></span>|<span data-ttu-id="84392-152">字符串</span><span class="sxs-lookup"><span data-stu-id="84392-152">String</span></span>| <span data-ttu-id="84392-153">员工成员，GUID 格式的 ID。</span><span class="sxs-lookup"><span data-stu-id="84392-153">The ID of the staff member, in a GUID format.</span></span> <span data-ttu-id="84392-154">只读。</span><span class="sxs-lookup"><span data-stu-id="84392-154">Read-only.</span></span>|
|<span data-ttu-id="84392-155">role</span><span class="sxs-lookup"><span data-stu-id="84392-155">role</span></span>|<span data-ttu-id="84392-156">string</span><span class="sxs-lookup"><span data-stu-id="84392-156">string</span></span>| <span data-ttu-id="84392-157">企业中的人员成员角色。</span><span class="sxs-lookup"><span data-stu-id="84392-157">The role of the staff member in the business.</span></span> <span data-ttu-id="84392-158">可取值为：`guest`、`administrator`、`viewer`、`externalGuest`。</span><span class="sxs-lookup"><span data-stu-id="84392-158">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span> <span data-ttu-id="84392-159">必需。</span><span class="sxs-lookup"><span data-stu-id="84392-159">Required.</span></span>|
|<span data-ttu-id="84392-160">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="84392-160">useBusinessHours</span></span>|<span data-ttu-id="84392-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="84392-161">Boolean</span></span>|<span data-ttu-id="84392-162">True 的表示员工成员的可用性，作为业务**businessHours**属性中指定。</span><span class="sxs-lookup"><span data-stu-id="84392-162">True means the staff member's availability is as specified in the **businessHours** property of the business.</span></span> <span data-ttu-id="84392-163">False，则意味着可用性由员工成员的**workingHours**属性设置。</span><span class="sxs-lookup"><span data-stu-id="84392-163">False means the availability is determined by the staff member's **workingHours** property setting.</span></span>|
|<span data-ttu-id="84392-164">workingHours</span><span class="sxs-lookup"><span data-stu-id="84392-164">workingHours</span></span>|<span data-ttu-id="84392-165">[bookingWorkHours](bookingworkhours.md)集合</span><span class="sxs-lookup"><span data-stu-id="84392-165">[bookingWorkHours](bookingworkhours.md) collection</span></span>|<span data-ttu-id="84392-166">员工成员了可供预定的一周中每一天时间范围。</span><span class="sxs-lookup"><span data-stu-id="84392-166">The range of hours each day of the week that the staff member is available for booking.</span></span> <span data-ttu-id="84392-167">默认情况下，它们都初始化为业务的**工作时间**属性相同。</span><span class="sxs-lookup"><span data-stu-id="84392-167">By default, they are initialized to be the same as the **businessHours** property of the business.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84392-168">关系</span><span class="sxs-lookup"><span data-stu-id="84392-168">Relationships</span></span>
<span data-ttu-id="84392-169">无</span><span class="sxs-lookup"><span data-stu-id="84392-169">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="84392-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84392-170">JSON representation</span></span>

<span data-ttu-id="84392-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84392-171">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingstaffmember.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
