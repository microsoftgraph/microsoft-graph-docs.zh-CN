---
title: 使用 Microsoft Graph 中的 Microsoft Bookings API
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Priority
author: angelgolfer-ms
ms.prod: bookings
doc_type: conceptualPageType
ms.openlocfilehash: 6159d830656ed898de1e91a4866c74f145cfa0a4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508022"
---
# <a name="use-the-microsoft-bookings-api-in-microsoft-graph"></a><span data-ttu-id="53217-104">使用 Microsoft Graph 中的 Microsoft Bookings API</span><span class="sxs-lookup"><span data-stu-id="53217-104">Use the Microsoft Bookings API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="53217-105">Microsoft Bookings 可让小型企业所有者以最少量的设置管理客户预订和信息。</span><span class="sxs-lookup"><span data-stu-id="53217-105">Microsoft Bookings lets small business owners manage customer bookings and information with minimal setup.</span></span> <span data-ttu-id="53217-106">企业所有者可以创建一个或多个企业，每个企业都提供一组服务。</span><span class="sxs-lookup"><span data-stu-id="53217-106">A business owner can create one or more businesses, with each business offering a set of services.</span></span> <span data-ttu-id="53217-107">所有者可以设置员工，并指定每名员工执行的服务。</span><span class="sxs-lookup"><span data-stu-id="53217-107">The owner can set up staff members, and specify the services that each staff member performs.</span></span> <span data-ttu-id="53217-108">客户可以通过在线或移动应用预约该企业中的特定服务。</span><span class="sxs-lookup"><span data-stu-id="53217-108">A customer can book an appointment for a specific service in that business in an online or mobile app.</span></span> <span data-ttu-id="53217-109">Bookings 可确保为企业、员工和相关客户保持最新的约会时间。</span><span class="sxs-lookup"><span data-stu-id="53217-109">Bookings ensures that the appointment time is kept up-to-date for the business, staff members, and customers involved.</span></span>

<span data-ttu-id="53217-110">就编程而言，Bookings API 中的 [bookingBusiness](bookingbusiness.md) 涉及以下对象：</span><span class="sxs-lookup"><span data-stu-id="53217-110">Programmatically, a [bookingBusiness](bookingbusiness.md) in the Bookings API involves the following objects:</span></span>
 
- <span data-ttu-id="53217-111">一个或多个 [bookingStaffMember](bookingstaffmember.md) 对象</span><span class="sxs-lookup"><span data-stu-id="53217-111">One or more [bookingStaffMember](bookingstaffmember.md) objects</span></span>
- <span data-ttu-id="53217-112">一个或多个 [bookingService](bookingservice.md) 对象</span><span class="sxs-lookup"><span data-stu-id="53217-112">One or more [bookingService](bookingservice.md) objects</span></span>
- <span data-ttu-id="53217-113">一组 [bookingAppointment](bookingappointment.md) 实例</span><span class="sxs-lookup"><span data-stu-id="53217-113">A set of [bookingAppointment](bookingappointment.md) instances</span></span>
- <span data-ttu-id="53217-114">一组 [bookingCustomer](bookingcustomer.md) 对象</span><span class="sxs-lookup"><span data-stu-id="53217-114">A set of [bookingCustomer](bookingcustomer.md) objects</span></span>

## <a name="using-the-bookings-rest-api"></a><span data-ttu-id="53217-115">使用 Bookings REST API</span><span class="sxs-lookup"><span data-stu-id="53217-115">Using the Bookings REST API</span></span>

<span data-ttu-id="53217-116">第一次客户预约之前，请完成以下步骤。</span><span class="sxs-lookup"><span data-stu-id="53217-116">Walk through the following steps before booking customer appointments for a business the first time.</span></span> <span data-ttu-id="53217-117">确保为相应的操作提供适当的[访问令牌](/graph/auth-overview)。</span><span class="sxs-lookup"><span data-stu-id="53217-117">Make sure you provide the appropriate [access tokens](/graph/auth-overview) for the corresponding operations.</span></span>

1. <span data-ttu-id="53217-118">确保企业具有 [Office 365 商业高级版](https://products.office.com/zh-CN/business/office-365-business-premium)订阅。</span><span class="sxs-lookup"><span data-stu-id="53217-118">Make sure the business has an [Office 365 Business Premium](https://products.office.com/zh-CN/business/office-365-business-premium) subscription.</span></span>
2. <span data-ttu-id="53217-119">通过向实体集发送 POST 操作来创建新的 **bookingBusiness**。</span><span class="sxs-lookup"><span data-stu-id="53217-119">Create a new **bookingBusiness** by sending a POST operation to the entity set.</span></span> <span data-ttu-id="53217-120">至少应为新企业指定客户将看到的名称：</span><span class="sxs-lookup"><span data-stu-id="53217-120">At minimum, you should specify a name for the new business that customers will see:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Contoso"
}
```
<span data-ttu-id="53217-121">使用 POST 响应中返回的新 **bookingBusiness** 的 **id** 属性继续[自定义](../api/bookingbusiness-update.md)企业设置，并为企业添加员工和服务。</span><span class="sxs-lookup"><span data-stu-id="53217-121">Use the **id** property of the new **bookingBusiness** returned in the POST response to continue to [customize](../api/bookingbusiness-update.md) business settings, and add staff members and services for the business.</span></span>

3. <span data-ttu-id="53217-122">为企业添加各个员工：</span><span class="sxs-lookup"><span data-stu-id="53217-122">Add individual staff members for the business:</span></span>
<!-- { "blockType": "ignored" } -->
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
4. <span data-ttu-id="53217-123">定义企业提供的每项服务：</span><span class="sxs-lookup"><span data-stu-id="53217-123">Define each service offered by the business:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/services
Authorization: Bearer {access token}
Content-Type: application/json

{
    "displayName":"Bento"
}
```
5. <span data-ttu-id="53217-124">发布企业的日程安排页面，让客户和企业经营者开始预约：</span><span class="sxs-lookup"><span data-stu-id="53217-124">Publish the scheduling page for the business, to let customers and business operators start booking appointments:</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/publish
Authorization: Bearer {access token}
```

<span data-ttu-id="53217-125">通常，若要列出 Office 365 租户中的所有预订企业：</span><span class="sxs-lookup"><span data-stu-id="53217-125">In general, to list all the booking businesses in the Office 365 tenant:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses
Authorization: Bearer {access token}
```

## <a name="common-use-cases"></a><span data-ttu-id="53217-126">常见用例</span><span class="sxs-lookup"><span data-stu-id="53217-126">Common use cases</span></span> 

<span data-ttu-id="53217-127">下表列出了 Bookings API 中的常见企业操作。</span><span class="sxs-lookup"><span data-stu-id="53217-127">The following table lists the common operations for a business in the Bookings API.</span></span>

| <span data-ttu-id="53217-128">用例</span><span class="sxs-lookup"><span data-stu-id="53217-128">Use cases</span></span>        | <span data-ttu-id="53217-129">REST 资源</span><span class="sxs-lookup"><span data-stu-id="53217-129">REST resources</span></span> | <span data-ttu-id="53217-130">另请参阅</span><span class="sxs-lookup"><span data-stu-id="53217-130">See also</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="53217-131">创建、获取、更新或删除企业</span><span class="sxs-lookup"><span data-stu-id="53217-131">Create, get, update, or delete a business</span></span> | [<span data-ttu-id="53217-132">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="53217-132">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="53217-133">bookingBusiness 的方法</span><span class="sxs-lookup"><span data-stu-id="53217-133">Methods of bookingBusiness</span></span>](bookingbusiness.md#methods) |
| <span data-ttu-id="53217-134">更新日程安排策略</span><span class="sxs-lookup"><span data-stu-id="53217-134">Update the scheduling policy</span></span> | [<span data-ttu-id="53217-135">bookingSchedulingPolicy</span><span class="sxs-lookup"><span data-stu-id="53217-135">bookingSchedulingPolicy</span></span>](bookingschedulingpolicy.md) | [<span data-ttu-id="53217-136">更新 bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="53217-136">Update a bookingBusiness</span></span>](../api/bookingbusiness-update.md) |
| <span data-ttu-id="53217-137">添加、获取、更新或删除员工</span><span class="sxs-lookup"><span data-stu-id="53217-137">Add, get, update, or delete staff members</span></span> | [<span data-ttu-id="53217-138">bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="53217-138">bookingStaffMember</span></span>](bookingstaffmember.md) | [<span data-ttu-id="53217-139">bookingStaffMember 的方法</span><span class="sxs-lookup"><span data-stu-id="53217-139">Methods of bookingStaffMember</span></span>](bookingstaffmember.md#methods)  |
| <span data-ttu-id="53217-140">添加、获取、更新或删除服务</span><span class="sxs-lookup"><span data-stu-id="53217-140">Add, get, update, or delete services</span></span> | [<span data-ttu-id="53217-141">bookingService</span><span class="sxs-lookup"><span data-stu-id="53217-141">bookingService</span></span>](bookingservice.md) | [<span data-ttu-id="53217-142">bookingService 的方法</span><span class="sxs-lookup"><span data-stu-id="53217-142">Methods of bookingService</span></span>](bookingservice.md#methods)  |
| <span data-ttu-id="53217-143">发布或取消发布日程安排页面</span><span class="sxs-lookup"><span data-stu-id="53217-143">Publish or unpublish the scheduling page</span></span> | [<span data-ttu-id="53217-144">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="53217-144">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="53217-145">发布</span><span class="sxs-lookup"><span data-stu-id="53217-145">publish</span></span>](../api/bookingbusiness-publish.md) <br> [<span data-ttu-id="53217-146">取消发布</span><span class="sxs-lookup"><span data-stu-id="53217-146">unpublish</span></span>](../api/bookingbusiness-unpublish.md) |
| <span data-ttu-id="53217-147">创建、获取、更新、删除或取消约会</span><span class="sxs-lookup"><span data-stu-id="53217-147">Create, get, update, delete, or cancel an appointment</span></span> | [<span data-ttu-id="53217-148">bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="53217-148">bookingAppointment</span></span>](bookingappointment.md) | [<span data-ttu-id="53217-149">bookingAppointment 的方法</span><span class="sxs-lookup"><span data-stu-id="53217-149">Methods of bookingAppointment</span></span>](bookingappointment.md#methods)  |
| <span data-ttu-id="53217-150">获取某个日期范围内的约会</span><span class="sxs-lookup"><span data-stu-id="53217-150">Get appointments in a date range</span></span> | [<span data-ttu-id="53217-151">bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="53217-151">bookingBusiness</span></span>](bookingbusiness.md) | [<span data-ttu-id="53217-152">列出 Bookings 日历视图</span><span class="sxs-lookup"><span data-stu-id="53217-152">List Bookings calendarView</span></span>](../api/bookingbusiness-list-calendarview.md) |
| <span data-ttu-id="53217-153">获取货币</span><span class="sxs-lookup"><span data-stu-id="53217-153">Get currency</span></span> | [<span data-ttu-id="53217-154">bookingCurrency</span><span class="sxs-lookup"><span data-stu-id="53217-154">bookingCurrency</span></span>](bookingcurrency.md) | [<span data-ttu-id="53217-155">bookingCurrency 的方法</span><span class="sxs-lookup"><span data-stu-id="53217-155">Methods of bookingCurrency</span></span>](bookingcurrency.md#methods) |


## <a name="see-also"></a><span data-ttu-id="53217-156">另请参阅</span><span class="sxs-lookup"><span data-stu-id="53217-156">See also</span></span>

- <span data-ttu-id="53217-157">尝试 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中的 API。</span><span class="sxs-lookup"><span data-stu-id="53217-157">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- <span data-ttu-id="53217-158">请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。</span><span class="sxs-lookup"><span data-stu-id="53217-158">See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
- <span data-ttu-id="53217-159">了解如何在 Microsoft Graph 中选择[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53217-159">Learn how to choose [permissions](/graph/permissions-reference) in Microsoft Graph.</span></span>
