---
title: 使用在 Microsoft Graph 中 Microsoft 预订 API
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Priority
ms.openlocfilehash: def9260654baafe1953d629265c4b76a2afd2748
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845533"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="2e210-104">使用在 Microsoft Graph 中 Microsoft 预订 API</span><span class="sxs-lookup"><span data-stu-id="2e210-104">Use the Microsoft Bookings API in Microsoft Graph</span></span>

 > <span data-ttu-id="2e210-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2e210-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e210-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2e210-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="2e210-107">Microsoft 预订允许小型企业所有者管理客户的预定和通过少量设置的信息。</span><span class="sxs-lookup"><span data-stu-id="2e210-107">Microsoft Bookings lets small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="2e210-108">业务所有者可以提供一组服务的每个业务部门创建一个或多个企业版。</span><span class="sxs-lookup"><span data-stu-id="2e210-108">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="2e210-109">所有者可以设置人员，并指定每个员工成员执行的服务。</span><span class="sxs-lookup"><span data-stu-id="2e210-109">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="2e210-110">客户可以在联机或移动应用程序中的业务书籍特定服务的约会。</span><span class="sxs-lookup"><span data-stu-id="2e210-110">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="2e210-111">预订确保的约会时间保持最新的人员，业务和客户涉及。</span><span class="sxs-lookup"><span data-stu-id="2e210-111">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="2e210-112">以编程方式预订 API 中[bookingBusiness](bookingbusiness.md)涉及以下对象：</span><span class="sxs-lookup"><span data-stu-id="2e210-112">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="2e210-113">一个或多个[bookingStaffMember](bookingstaffmember.md)对象</span><span class="sxs-lookup"><span data-stu-id="2e210-113">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="2e210-114">一个或多个[bookingService](bookingservice.md)对象</span><span class="sxs-lookup"><span data-stu-id="2e210-114">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="2e210-115">一套[bookingAppointment](bookingappointment.md)实例</span><span class="sxs-lookup"><span data-stu-id="2e210-115">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="2e210-116">一组[bookingCustomer](bookingcustomer.md)对象</span><span class="sxs-lookup"><span data-stu-id="2e210-116">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="2e210-117">使用预订 REST API</span><span class="sxs-lookup"><span data-stu-id="2e210-117">Using the Bookings REST API</span></span>

<span data-ttu-id="2e210-118">预订第一次的业务的客户约会之前逐步完成以下步骤。</span><span class="sxs-lookup"><span data-stu-id="2e210-118">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="2e210-119">请确保您为相应的操作提供适当的[访问令牌](/graph/auth-overview)。</span><span class="sxs-lookup"><span data-stu-id="2e210-119">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="2e210-120">确保业务具有的[Office 365 企业高级版](https://products.office.com/en-us/business/office-365-business-premium)订阅。</span><span class="sxs-lookup"><span data-stu-id="2e210-120">Make sure the business has an [Office 365 Business Premium](https://products.office.com/en-us/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="2e210-121">创建新**bookingBusiness**通过将 POST 操作发送到的实体集。</span><span class="sxs-lookup"><span data-stu-id="2e210-121">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="2e210-122">至少应指定客户将看到新的业务的名称：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2e210-122">At minimum, you should specify a name for the new business that customers will see: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="2e210-123">POST 响应中返回新**bookingBusiness**的**id**属性用于继续[自定义](../api/bookingbusiness-update.md)业务设置，并添加员工和业务的服务。</span><span class="sxs-lookup"><span data-stu-id="2e210-123">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="2e210-124">添加业务的人员成员：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2e210-124">Add individual staff members for the business: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Dana Swope",
    "emailAddress": "danas@contoso.com",
    "role": "externalGuest"
}
```
4. <span data-ttu-id="2e210-125">定义由业务提供每个服务：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2e210-125">Define each service offered by the business: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="2e210-126">发布的企业，可以让客户和业务运算符启动预订约会的计划页：<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2e210-126">Publish the scheduling page for the business, to let customers and business operators start booking appointments: <!-- { "blockType": "ignored" } --></span></span>
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="2e210-127">通常，列出 Office 365 租户中的所有预订企业： 中<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="2e210-127">In general, to list all the booking businesses in the Office 365 tenant: <!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="2e210-128">常见用例</span><span class="sxs-lookup"><span data-stu-id="2e210-128">Common use cases</span></span> 

<span data-ttu-id="2e210-129">下表列出了业务预订 API 中的常见操作。</span><span class="sxs-lookup"><span data-stu-id="2e210-129">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="2e210-130">用例</span><span class="sxs-lookup"><span data-stu-id="2e210-130">Use cases</span></span>        | <span data-ttu-id="2e210-131">REST 资源</span><span class="sxs-lookup"><span data-stu-id="2e210-131">REST resources</span></span> | <span data-ttu-id="2e210-132">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2e210-132">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="2e210-133">创建、 获取、 更新或删除业务</span><span class="sxs-lookup"><span data-stu-id="2e210-133">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="2e210-134">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="2e210-134">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="2e210-135">BookingBusiness 方法</span><span class="sxs-lookup"><span data-stu-id="2e210-135">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="2e210-136">更新计划策略</span><span class="sxs-lookup"><span data-stu-id="2e210-136">Update the scheduling policy</span></span> | [<span data-ttu-id="2e210-137">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="2e210-137">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="2e210-138">更新 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="2e210-138">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="2e210-139">添加、 获取、 更新或删除员工成员</span><span class="sxs-lookup"><span data-stu-id="2e210-139">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="2e210-140">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="2e210-140">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="2e210-141">BookingStaffMember 方法</span><span class="sxs-lookup"><span data-stu-id="2e210-141">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="2e210-142">添加、 获取、 更新或删除服务</span><span class="sxs-lookup"><span data-stu-id="2e210-142">Add, get, update, or delete services</span></span> | [<span data-ttu-id="2e210-143">bookingService</span><span class="sxs-lookup"><span data-stu-id="2e210-143">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="2e210-144">BookingService 方法</span><span class="sxs-lookup"><span data-stu-id="2e210-144">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="2e210-145">公开或取消公开计划页</span><span class="sxs-lookup"><span data-stu-id="2e210-145">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="2e210-146">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="2e210-146">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="2e210-147">发布</span><span class="sxs-lookup"><span data-stu-id="2e210-147">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="2e210-148">取消发布</span><span class="sxs-lookup"><span data-stu-id="2e210-148">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="2e210-149">创建、 获取、 更新、 删除或取消约会</span><span class="sxs-lookup"><span data-stu-id="2e210-149">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="2e210-150">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="2e210-150">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="2e210-151">BookingAppointment 方法</span><span class="sxs-lookup"><span data-stu-id="2e210-151">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="2e210-152">获取约会中的日期范围</span><span class="sxs-lookup"><span data-stu-id="2e210-152">Get appointments in a date range</span></span> | [<span data-ttu-id="2e210-153">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="2e210-153">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="2e210-154">列表的预定 calendarView</span><span class="sxs-lookup"><span data-stu-id="2e210-154">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="2e210-155">获取货币</span><span class="sxs-lookup"><span data-stu-id="2e210-155">Get currency</span></span> | [<span data-ttu-id="2e210-156">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="2e210-156">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="2e210-157">BookingCurrency 方法</span><span class="sxs-lookup"><span data-stu-id="2e210-157">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |


## <a name="see-also"></a><span data-ttu-id="2e210-158">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2e210-158">See also</span></span>

- <span data-ttu-id="2e210-159">尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="2e210-159">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="2e210-160">请参阅[一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。</span><span class="sxs-lookup"><span data-stu-id="2e210-160">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
- <span data-ttu-id="2e210-161">了解如何在 Microsoft Graph 中选择[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e210-161">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>
